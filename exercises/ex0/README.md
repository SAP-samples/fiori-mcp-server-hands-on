# Getting Started - Set up your AI Development Environment

As a participant of the hands-on tutorial, you should already be setup with access to the SAP Business Application Studio landscape below which you can use as your development environment.

## Access SAP Business Application Studio (SBAS)

1. Open https://lcapteched.eu10.build.cloud.sap/lobby in a new browser window or tab, which will ask you to login.

2. Open the [Login File for SBAS](../../SBASLogin.txt) and pick the login data for your assigned number.

3. Enter the data in the SBAS browser window or tab to complete your login.

    <img src="./images/ex0img23.png" alt="login" width="60%"/>

## Access the Dev Space Manager

1. On the SAP Build landing page, click the **Switch Product** button in the top right corner and select **Dev Space Manager**.

    ![Access Dev Space Manager](images/ex0img0.png)

## Open the Development Space

1. Make sure that the development space **AgenticAppDevelopment** has the status running. If stopped, click the **start** button.

    ![Restart Dev Space](images/ex0img4a.png)


> [!NOTE]
> For this hands-on session, please use only the **AgenticAppDevelopment** development space.

2. Once running, click the development space name to open it. This can take some time.

    ![Enter Dev Space](images/ex0img4.png)

3. Click **OK** in the popup window to accept the tracking settings in the newly created dev space.

    ![image](images/ex0img5.png)

## Install SAP Fiori MCP Server
- Open new terminal

    ![image](images/open-terminal.png)

- execute command `npm i -g @sap-ux/fiori-mcp-server`

    ![image](images/install-fiori-mcp.png)

## Verify MCP servers

- Verify below listed mcp servers are installed

    ![mcp servers](./images/mcp-servers.png)
    

## Open your project folder

1. Select the **explorer icon** on the left side.

    ![image](images/ex0img10.png)

2. Select **Open Folder**.

    ![image](images/ex0img11.png)

3. Select the **projects** folder from the drop down.

    ![image](images/ex0img12.png)

4. Click **OK** and your window will reload.

    ![image](images/ex0img13.png)

5. Enable **Clipboard access** for the SBAS instance in the Chrome browser.

    ![image](images/ex0img28.png)

6. Download Image [manage-travels-list-report.png](../../manage-travels-list-report.png) to your local disk.

7. Drag and drop downloaded image to project explorer

    ![image](images/project-explorer.png)

## Configure Github Copilot (AI Client)

1. Open **Github Copilot**.

    ![copilot](./images/ex0img32.png)

2. Select model **Claude Sonnet 4.5**.

    ![copilot](./images/ex0img34.png)


## Summary

You have successfully set up your AI development environment with SAP Business Application Studio and configured github Copilot.

Continue to - [Exercise 1.0 - Create CAP Project and Fiori List Report App based on Image](../ex1.0/README.md)

