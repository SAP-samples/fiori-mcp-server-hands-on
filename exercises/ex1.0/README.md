# Create CAP Project and Fiori List Report App based on Image

In this exercise you will create a CAP project and a SAP Fiori List Report application from a reference screenshot.

1. Drag and drop the image [manage-travels-list-report.png](../../manage-travels-list-report.png) from the `Images` folder into the Copilot Chat window to attach it as context.

    ![drop](./images/drop-image.png)

2. Copy and paste the following prompt into the chat input and execute it:

    ```
    Extract data from the attached Image. Do not inspect any other image files in the workspace.
    ```

3. Verify that the extracted data matches the image.

    ![extracted data](./images/extracted-data.png)

4. Copy and paste the following prompt into the chat input and execute it to generate the CAP project:

    ```
    /cap-developer Generate CAP NodeJs project based on extracted data.
    - Include technical key and business key for all entities.
    - Use USD as currency throughout the application.
    - Apply criticality for travel status
    ```

5. Copilot generates the CAP project by applying the guidelines defined in the `cap-developer` skill.

    ![cap-project-generation](./images/cap-project-generation.png)

6. Click **Allow** when prompted to run Bash commands.

7. Review the files and content created by Copilot, then click **Keep** to accept them.

8. Confirm that the CAP project has been successfully created in your workspace.

9. Copy and paste the following prompt into the chat input and execute it to generate the SAP Fiori app:

    ```
    /sap-fiori-app-development Generate SAP Fiori app based on cap project and
    - SAP Fiori app should match extracted data from the image (table columns, filters etc.)
    - Use UI5 version 1.148.12
    - Use USD as currency throughout the application
    - Consult available MCP servers.
    ```

10. Copilot generates the SAP Fiori app by applying the guidelines defined in the `sap-fiori-app-development` skill.

    ![fiori-app-generation](./images/fiori-app-generation.png)

11. To run the application, click the **Insert into Terminal** button when Copilot presents the watch command.

    ![run preview](./images/preview-command.png)

    The application will open in your browser, displaying a travel list report application that matches similar to the uploaded screenshot.

    ![application preview](./images/application-preview.png)

## Troubleshoot

1. Application preview does not open automatically in the browser:

    - Stop any running processes using `Ctrl+C`, then delete all terminal windows, including any hidden ones.

        ![close terminal](./images/close-terminal.png)

    **Option 1:**
    
    - Right-click on the Fiori app and select the watch script. **Important:** Keep the application preview terminal running—do not close it.

        ![preview app](./images/preview-application.png)

        ![watch travel](./images/watch-travel.png)

    **Option 2:**
    
    - You can start the watch script manually:
        - Open the **package.json** file.
        - Right-click on the **watch** script and select **Run Script**.

        ![watch script](./images/watch-script.png)

2. `ENOSPC: System limit for number of file watchers reached`

    ![system limit error](./images/system-limit-error.png)

    Add the following script to the **package.json** file:

    ```
    "cds": {
        "watch": {
            "excludes": [
                "**/node_modules",
                "**/target",
                "db/data.sqlite"
            ]
        }
    }
    ```
    ![package json](./images/package-json-entry.png)

3. If HTTP port 4004 is already in use, press `Enter` to restart preview with a different port number.

> [!NOTE]
> Ensure that you either use 4004 or the system-assigned port for the preview. Check terminal instances and delete any duplicate processes running to preview the application.

4. If the application prompts for authentication, use username: `dummy` and password: `dummy`.

## Summary

You have successfully created a CAP project with a Fiori List Report application based on the Image.

Continue to - [Exercise 1.1 - Enable automatic data loading in List Report](../ex1.1/README.md)
