# Getting Started - Setting up your AI Development Environment

As a particpant of the hands-on, you should already be setup with access to the SAP Business Application Studio landscape below which you can use as your development environment.

## Accessing SAP Business Application Studio (SBAS)

Navigate to https://lcapteched.eu10.build.cloud.sap/lobby

Enter SBAS login credentials provided to you during the hands-on.

<img src="./images/ex0img23.png" alt="Cline browser" width="60%"/>

## Accessing the Dev Space Manager

On the SAP Build landing page, click button **Switch Product** in the top right corner and select **Dev Space Manager**.<br>
![Access Dev Space Manager](images/ex0img0.png)

## Opening the Development Space

Make sure development space "AgenticAppDevelopment" has status running. If stopped, click the start button. <br>
![Restart Dev Space](images/ex0img4a.png)

### Note: For this hands-on session, please use only the "AgenticAppDevelopment" development space.

Once running, click on the development space name to open it. This can take some time.<br>

![Enter Dev Space](images/ex0img4.png)

Click **OK** in the popup window to accept the tracking settings in the newly created dev space.

![image](images/ex0img5.png)

## Open your project folder

Open the explorer icon from the left hand side:

![image](images/ex0img10.png)

And select **Open Folder** button

![image](images/ex0img11.png)

Select the **Projects** folder from the drop down

![image](images/ex0img12.png)

Click **OK** and your window will reload

![image](images/ex0img13.png)

Enable Clipboard access to SBAS instance for chrome browser.

![image](images/ex0img28.png)

Download image [process travels](./images/process-travels.png).

![download](./images/ex0img25.png)

Drag and drop image(process-travels.png) to Explorer.

![explorer](./images/ex0img26.png)

## Configure Cline (AI Client)

1. Open Cline

  <img src="./images/ex0img22.png" alt="cline" width="30%"/>

2. choose `Bring my own API Key`.

  <img src="./images/ex0img7.png" alt="cline choose api key" width="70%"/>

3. select API Provider `SAP AI Core`, selectmodel `anthropic--claude-sonnet-4`.

  <img src="images/ex0img8.png" alt="image" width="40%"/>

4. Click on `Lets Go` button.
5. Close all cline notifications.

  <img src="images/ex0img9.png" alt="image" width="40%"/>

6. **Disable Browser Tool Usage**

   - In the **Cline Settings**, Click on the **Browser** section.
   - Check the option **Disable browser tool usage**.

  <img src="./images/ex0img15.png" alt="disable browser" width="40%"/>

## Restart MCP Servers

1. In the Cline panel, Click the **MCP Servers** icon in the top-right corner.
   - Click on Configure.
   - Restart both `fiori-mcp` and `cds-mcp` servers

  ![Cline MCP server setting](./images/ex0img24.png)

## Enable Auto-Approve settings for Cline

  - Enable auto-approval for file modifications from Cline.  
  - Enable auto-approval for MCP server usage. 

  <img src="./images/ex0img21.png" alt="auto approve" width="40%"/>
  <img src="./images/ex0img21a.png" alt="auto approve" width="40%"/>

## Summary

With the setup procedure done, you now have completed:

- Access to SAP Business Application Studio
- Configure Cline

Continue to - [Exercise 2 - Generate CAP Project and Fiori List Report App based on Image](../ex1.0/README.md)

## TroubleShoot:
No Dev space available in BAS - [Create new dev space and install cline extension manually](README2.md)

