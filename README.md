# Expo CLI Error: SDK Version Mismatch or Corrupted Installation

This repository demonstrates a common Expo CLI error related to SDK version mismatches or corrupted installations.  The `expoBug.js` file shows an example project setup that may trigger the error, and the `expoBugSolution.js` file provides solutions and how to reproduce the problem.

## Reproducing the Issue

1. **Clone the repository:** `git clone ...`
2. **Navigate to the project directory:** `cd ...`
3. **Attempt to run Expo commands:**  `expo start`, `expo build:ios`, or `expo prebuild`.  You might encounter errors indicating an SDK version mismatch or problems with Expo modules.

## Solution

The `expoBugSolution.js` file demonstrates how to resolve these issues.  It details:

*   **Updating Expo CLI:**  Ensure you have the latest version using `npm install -g expo-cli` (or `yarn global add expo-cli`).
*   **Checking package.json:** Verify the Expo SDK version in your project's `package.json` matches what you expect. Use `expo upgrade` to update the SDK and dependencies to align with your CLI.
*   **Cleaning the project:**  Sometimes, removing `node_modules` and re-installing packages (`npm install` or `yarn install`) can clear up unexpected issues.
*   **Creating a new project:** If problems persist, create a fresh new Expo project with the `expo init` command and transfer over your code.  This helps to rule out corrupted dependencies or local configuration.