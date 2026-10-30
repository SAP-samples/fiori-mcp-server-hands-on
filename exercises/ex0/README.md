# Getting Started - Set up your AI Development Environment

As a participant of the hands-on tutorial, you will use **Visual Studio Code** on your local machine as your development environment.

## Install Visual Studio Code

1. Download and install Visual Studio Code from the official site: https://code.visualstudio.com/.

2. Launch VS Code once installation is complete.

## Install Prerequisites

Install the following tools so that VS Code can build and run the SAP Fiori / CAP projects used in this tutorial.

### Node.js (LTS)

1. Download and install the latest **LTS** version of Node.js from https://nodejs.org/.

2. Verify the installation from a terminal:

    ```bash
    node --version
    npm --version
    ```

### SAP Fiori tools - Extension Pack

1. In VS Code, open the **Extensions** view (`Ctrl+Shift+X` / `Cmd+Shift+X`).

2. Search for **SAP Fiori tools - Extension Pack** and click **Install**.

    This extension pack bundles the SAP Fiori generators, Application Modeler, Guided Development, XML/annotation tooling, and more.

3. Reload VS Code if prompted.

## Configure GitHub Copilot (AI Client)

GitHub Copilot Chat is a built-in extension in VS Code and part of standard VS Code installation. You only need to sign in and pick a model.

1. Sign in with your personal or work GitHub account.
2. Open Copilot Chat.
3. Click the model dropdown at the bottom of the chat panel.
4. Select any Claude **Sonnet** or **Opus** model version of your choice.

## Install Plugin from Copilot Marketplace

To let GitHub Copilot create and modify SAP Fiori Elements applications, install the `sap-ux-fiori-tools` plugin:

1. In VS Code, open the Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`) and run **Chat: Plugins**.
2. Search for **sap-ux-fiori-tools**.
3. Click **Install**.

    ![sap-fiori-tools-plugin](./images/sap-fiori-tools-plugin.png)

    > **Note:** This plugin installs both the MCP server for SAP Fiori and the skills needed for Fiori app development.

4. **Disable the built-in MCP Server** to avoid duplicate configurations:
    - Open the Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`) and run **Preferences: Open User Settings**.
    - Search for **SAP Fiori MCP**.
    - Uncheck **SAP UX Fiori Tools > MCP Server: Enable** to disable the MCP Server provided by the SAP Fiori Tools - Application Modeler extension.

    ![disable-user-setting](./images/disable-user-setting.png)

## Install CAP MCP Server

To enable AI assistance for CAP (Cloud Application Programming Model) development, install the CAP MCP server:

1. In VS Code, open the Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`) and run **MCP: Browse MCP Servers**.
2. In the MCP servers search box, type **cap mcp server**.
3. Click **Install** to add the CAP MCP server to your configuration.

    ![cap-mcp](./images/cap-mcp-server.png)

## Install Skills for CAP Development

To enhance AI assistance with CAP-specific development patterns and best practices, install the CAP developer skill:

1. Open the integrated terminal in VS Code.
2. Run the following command:

    ```bash
    npx skills add https://github.com/capire/skills.git
    ```

3. Follow the interactive prompts in the terminal and choose Project as the installation scope..

## Open your projects folder

In the next exercises you will use AI to **generate a new project** inside this projects folder — it should be empty at this point.

1. Create an empty local folder named `projects` anywhere on your local system (for example `~/user/projects` on macOS/Linux or `C:\user\projects` on Windows).

2. Download the **Images.zip** file and extract it into your `projects` folder:
    - Download [Images.zip](../../Images.zip)
    - Extract the contents into the `projects` folder
    - You should now have an `Images` subfolder containing the exercise images

3. In VS Code, choose **File > Open Folder…** and select the `projects` folder.

    ![explorer](./images/explorer.png)

4. If VS Code asks about trusting the folder, confirm **Yes, I trust the authors**.



## Summary

You have successfully set up your AI development environment with Visual Studio Code, installed the SAP Fiori tools - Extension Pack and Node.js, installed the **sap-ux-fiori-tools** Copilot plugin, and signed in to the built-in GitHub Copilot with a Claude **Sonnet** or **Opus** model of your choice.

Continue to - [Exercise 1.0 - Create CAP Project and Fiori List Report App based on Image](../ex1.0/README.md)

