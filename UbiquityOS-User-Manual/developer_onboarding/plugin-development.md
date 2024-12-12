# Plugin-Development



**Plugins** are at the heart of Ubiquibot’s extensibility, allowing developers to build custom functionalities that enhance automation, streamline workflows, and provide tailored solutions for various organizational needs. Plugin development revolves around leveraging the power of the Ubiquibot kernel to respond to GitHub events, execute commands, or handle complex tasks with precision and efficiency.&#x20;

Developing plugins for Ubiquibot opens the door to customizing and extending the platform to meet specific workflows and automation needs. This manual is designed to guide developers through the process of creating, testing, and deploying plugins seamlessly integrated with the Ubiquibot kernel.

### **Prerequisites**

1. Familiarize yourself with the Ubiquibot kernel, its operations, and interactions.
2. Understand how to define and validate plugin settings within Ubiquibot configurations.
3. Ensure you have `yarn` or `bun` installed on your local machine.

This Guide provides a step-by-step guide for developers to create and deploy a plugin for the **Ubiquibot** **platform**. Follow these instructions to ensure your plugin integrates seamlessly with the Ubiquibot kernel.

### **Getting Started**

1.  **Setup Repository**:

    Use the Ubiquibot plugin template to create a new repository. and clone the repository to your local machine.
2.  **Install Dependencies**:

    Run one of the following commands to install dependencies:

```
yarn install
# or
bun install
```

### **Creating a New Plugin**

#### **1. Determine Plugin Type**

* **Worker Plugin:** Use this type for slash commands requiring faster response times.
* **Action Plugin:** Suitable for longer-running tasks triggered by GitHub events.

#### **2. Update Configuration Files**

*   **`compute.yml`**:

    Add your plugin’s name and unique `id`.
*   **`context.ts`**:

    Define the events your plugin will handle. Example:

    ```
    export const events = ["issues.opened", "pull_request.merged"];
    ```
*   **`manifest.json`**:

    Provide a detailed description of your plugin for better documentation.
*   **`plugin-inputs.ts`**:

    Define the settings your plugin expects to receive from the kernel. Example:

    ```
    export interface PluginInputs {
      configurableResponse: string;
      customStringsUrl: string;
    }
    ```

#### **3. Configure Plugin Settings**

Your configuration in `.ubiquibot-config.yml` should look like this:

```
plugins:
  - name: hello-world
    id: hello-world
    uses:
      - plugin: http://localhost:4000
        with:
          configurableResponse: "Hello, is it me you are looking for?"
          customStringsUrl: "https://example.com/strings.json"
```

#### **4. Implement Plugin Logic**

Add your custom logic to `plugin.ts`.&#x20;

Example:

```
export const handleEvent = async (context: PluginContext) => {
  const response = context.settings.configurableResponse;
  console.log(response);
};
```

### **Testing Your Plugin**

#### **1. Testing Worker Plugins**

*   Start the worker locally:

    ```
    yarn worker
    # or
    bun worker
    ```
*   Trigger the worker using a POST request:

    ```
    await fetch("http://localhost:4000/", {
      method: "POST",
      headers: {
        "Content-Type": "application/json",
      },
      body: JSON.stringify({
        stateId: "",
        eventName: "",
        eventPayload: "",
        settings: "",
        ref: "",
        authToken: "",
      }),
    });
    ```

#### **2. Testing Action Plugins**

1. Ensure the kernel is running and listening for events.
2. Trigger an event in the repository where the kernel is installed (e.g., opening an issue).
3. Verify logs and output in the GitHub Actions tab.

#### **3. Local Testing Using Nektos Act**

* Use [Nektos Act](https://github.com/nektos/act) to run GitHub Actions workflows locally.

***

### **Deploying Your Plugin**

#### **1. Deploying Worker Plugins**

1. Use Worker Deploy and Worker Delete workflows in GitHub Actions.
2. Set up a Cloudflare account and add the following secrets:
   * `CLOUDFLARE_ACCOUNT_ID`
   * `CLOUDFLARE_API_TOKEN`

#### **2. Deploying Action Plugins**

1. Push your changes to the repository.
2. Ensure the kernel is configured to dispatch events to your plugin.

