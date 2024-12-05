# UbiquityOS Plugin Installer

## Overview

This document provides a guide on how to use the UbiquityOS Plugin Installer. This was hand-coded on an airplane ride with no internet.

This guide provides detailed instructions on how to develop, configure, and deploy plugins within the UbiquityOS platform.

### Steps

1. **Set Up Your Environment**

   - Ensure you have Node.js and Yarn installed.
   - Clone the repository and navigate to the project directory.

2. **Install Dependencies**
   ```sh
   yarn install
   ```
3. **Configure Supabase**

- Replace the hardcoded SUPABASE_URL and SUPABASE_KEY in build/esbuild-build.ts with your Supabase URL and key.

- Optionally, use a .env file and access the variables using process.env.

4. **Start the Development Server**

   ```sh
    yarn start
   ```

   - Visit localhost:8080 in your browser.
   - Log in to see the organizations you own.

5. **Manage Plugins**
   - Select an organization.
   - Choose a configuration (dev | prod).
   - Select a plugin to edit, add, or remove.
   - Push changes to GitHub.

### Plan as of 16 September 2024

- This only views the manifest you pass in.
- There is a hardcoded table header which is intended to be the origin URL of the manifest file.
- Currently, you need to pass in the manifest, but we should pass in a URL and the UI should fetch the manifest from the URL instead.

### Add & Remove Config

- A simple answer could be to create an API (GitHub Actions?) that just asks ChatGPT to refactor the `.ubiquibot-config.yml` and push the commit. Refactoring via LLM seems pretty straightforward in my experience.
- The optimized answer is to parse the YML file, and target the config based on its URL/location. Then edit the YML file using traditional code and push the commit using the user's credentials (there is a "GitHub Sign In" button).

### Remarks

- The remove or add buttons should display intelligently. Given that I admin two organizations that use the bot, it's a bit tricky. To start, perhaps it makes sense to display both, but we should figure out a solution that's simple to implement.

## How To Use

Pass the manifest in the `?manifest=` query parameter for the UI to parse it.

Example:

```
?manifest={%22name%22:%22Start%20|%20Stop%22,%22description%22:%22Assign%20or%20un-assign%20yourself%20from%20an%20issue.%22,%22ubiquity:listeners%22:[%22issue_comment.created%22,%22issues.assigned%22,%22pull_request.opened%22%20],%22commands%22:{%22start%22:{%22ubiquity:example%22:%22/start%22,%22description%22:%22Assign%20yourself%20to%20the%20issue.%22},%22stop%22:{%22ubiquity:example%22:%22/stop%22,%22description%22:%22Unassign%20yourself%20from%20the%20issue.%22}}}
```

The browser automatically URI encodes it:

```json
{
  "name": "Start | Stop",
  "description": "Assign or un-assign yourself from an issue.",
  "ubiquity:listeners": [
    "issue_comment.created",
    "issues.assigned",
    "pull_request.opened"
  ],
  "commands": {
    "start": {
      "ubiquity:example": "/start",
      "description": "Assign yourself to the issue."
    },
    "stop": {
      "ubiquity:example": "/stop",
      "description": "Unassign yourself from the issue."
    }
  }
}
```

Example from `command-start-stop/manifest.json`

## How to Run

1. Clone the repository.
2. Run `yarn` to install dependencies.
3. OAuth: Obtain your GitHub OAuth App client ID and secret from your OAuth app settings, and set the callback URL to match the one given by Supabase when enabling GitHub provider OAuth.
4. Replace the hardcoded `SUPABASE_URL` and `SUPABASE_KEY` in `build/esbuild-build.ts` with your Supabase URL and key (Optionally use `.env` and use `process.env` instead).
5. Run `yarn start` and visit `localhost:8080` in your browser.
6. Once logged in, you should see the orgs that you own.
7. Select an org > select a config (dev | prod) > select a plugin > edit/add/remove > push to GitHub.
