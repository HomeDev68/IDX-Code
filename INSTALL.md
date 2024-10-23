# Installation Guide for IDX Code

This guide provides step-by-step instructions to build and package the IDX Code application.

## Prerequisites

Ensure you have the following installed on your system:
- Node.js
- npm

You can download and install them from [Node.js](https://nodejs.org/).

## Steps to Build and Package IDX Code

1. **Clone the Repository**

   Clone the repository and navigate to the project directory.

   ```sh
   git clone https://github.com/HomeDev68/IDX-Code.git
   cd IDX-Code
   ```

2. **Install Dependencies**

   Install the required dependencies by running:

   ```sh
   npm install
   ```

3. **Compile the Source Code**

   Compile the source code by running:

   ```sh
   npm run compile
   ```

4. **Build the Electron Application**

   To build the Electron application, run:

   ```sh
   npm run electron
   ```

5. **Package the Application**

   To package the application, run:

   ```sh
   npm run package
   ```

## Disabling Telemetry by Default

To disable telemetry by default, ensure the following changes are made:

1. In the `src/vs/platform/telemetry/common/telemetryService.ts` file, update the default value of the `TELEMETRY_SETTING_ID` configuration to `TelemetryConfiguration.OFF`.

2. In the `product.json` file, add or update the `disableTelemetry` property to `true`.

By following these steps, you will be able to build and package the IDX Code application with telemetry disabled by default.
