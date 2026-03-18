# Getting Started - Set up your AI Development Environment

As a participant of the hands-on tutorial, you should already be setup with access to the SAP Business Application Studio landscape below which you can use as your development environment.

## Access SAP Business Application Studio (SBAS)

1. Open https://lcapteched.eu10.build.cloud.sap/lobby in a new browser window or tab, which will ask you to login.

2. Open the [Login File for SBAS](../../SBASLogin.txt) and pick the login data for your assigned number.

3. Enter the data in the SBAS browser window or tab to complete your login.

    <img src="./images/ex0img23.png" alt="Cline browser" width="60%"/>

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

## Configure Cline (AI Client)

1. Open **Cline**.

    <img src="./images/ex0img22.png" alt="cline" width="30%"/>

2. Choose **Bring my own API Key**.

    <img src="./images/ex0img7.png" alt="cline choose api key" width="70%"/>

3. Select API Provider **SAP AI Core** and choose the model **anthropic--claude-4.5-sonnet**.

    <img src="images/ex0img8.png" alt="image" width="40%"/>

4. Cline is now ready to go.

5. Close all Cline notifications.

    <img src="images/ex0img9.png" alt="image" width="40%"/>

6. Disable Browser Tool Usage:

    * In the **Cline Settings**, click on the **Browser** section.
    * Verify the option **Disable browser tool usage** is selected.

        <img src="./images/ex0img15.png" alt="disable browser" width="40%"/>

## Finalize Configuration of MCP Servers

1. In the Cline panel, click the **MCP Servers** icon in the top-right corner.

2. Click on **Configure**.

3. Check that **fiori-mcp**, **cds-mcp** and **Framelink_Figma_MCP** are listed.

    ![Cline MCP server setting](./images/ex0img24b.png)

4. Click on **Configure MCP Servers** to open the configuration file.

5. Insert the **personal access token** that you created in the previous exercise at the marked position.

    ![Cline MCP server setting](./images/ex0img25.png)

6. Wait until the status of the three MCP servers shows **green** again. You can use the refresh icon or the restart button, if displayed, to restart each server if problems occur.

7. Click on **Done** to complete this step.

## Enable Auto-Approve settings for Cline

1. Open the **Auto-approve** settings.

    <img src="./images/ex0img21.png" alt="auto approve" width="40%"/>

2. Enable auto-approval for **file modifications** from Cline.

2. Enable auto-approval for **MCP server usage**.

    <img src="./images/ex0img21a.png" alt="auto approve" width="40%"/>

## Summary

You have successfully set up your AI development environment with SAP Business Application Studio and configured Cline.

Continue to - [Exercise 2.0 - Create CAP Project and Fiori List Report App based on Figma Design](../ex2.0/README.md)

