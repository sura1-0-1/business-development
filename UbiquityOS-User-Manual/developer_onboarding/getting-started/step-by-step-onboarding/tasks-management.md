# Submit Solutions

### **Creating a Draft Pull Request and Starting Work on a Task**

This guide outlines the step-by-step procedure for creating a Draft Pull Request (PR) and starting work on a GitHub task. Following this process ensures proper task assignment, context tracking, and work deliverable auditing.

### **Step 1: Fork the Repository**

1. Navigate to the repository on GitHub.
2. Click on the **Fork** button at the top right corner of the page.
3. This creates a personal copy of the repository under your GitHub account.

<figure><img src="../../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

### **Step 2: Clone the Forked Repository**

1. Open your terminal or command line.
2.  Clone your forked repository using the command:

    ```bash
    clone https://github.com/<your-username>/<repository-name>.git
    ```
3.  Navigate into the cloned repository:

    ```bash
    cd <repository-name>
    ```

### **Step 3: Create a New Branch**

<figure><img src="../../../.gitbook/assets/image (9).png" alt="" width="348"><figcaption></figcaption></figure>

1.  Create a branch for your task

    ```bash
    git checkout -b <branch-name>
    ```

    Replace `<branch-name>` with a descriptive name (e.g., `fix-bug-123`).

### **Step 4: Open a Draft Pull Request.**

1.  Commit and push your initial changes to the branch:

    ```bash
    git add .
    git commit -m "Initial commit for task"
    git push origin <branch-name>
    ```
2. Open GitHub and navigate to your forked repository.
3. Click **Compare & pull request**.
4. In the **Pull Request** form:
   * Set the PR title and description.
   *   Include the issue link in the description with the format:

       ```plaintext
       Resolves <URL-to-the-issue>
       ```

       Replace `<URL-to-the-issue>` with the actual issue URL.

<figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

1. Select **Create Draft Pull Request** (not a standard PR).

### **Step 5: Work on the Task**

1. Make frequent commits as you work on the task to keep the organization updated.
2.  Push your commits regularly:

    ```bash
    git push origin <branch-name>
    ```

**Tip:** Ensure all builds and tests pass before pushing your changes.

### **Step 6: Mark PR as Ready for Review**

When your work is complete go to the draft PR on GitHub and click **Ready for review** to mark it as complete.

<figure><img src="../../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

### **⇒  During the Review Process**

1. **Do Not Force Push** \
   Avoid using `git push --force` once the review process starts. Force pushing deletes commit history, which slows down reviews.
2. **Tag the Task Creator if Necessary** \
   If a reviewer hasn’t picked up your PR within 24 hours, tag the task creator in a comment to request a review.

**Review and Completion**

1. Address reviewer feedback promptly by committing changes to the same branch.
2. Once approved, the PR can be merged into the main branch by a maintainer or based on organizational protocols.
