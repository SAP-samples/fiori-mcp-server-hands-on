# Modify travel object page based on Image

1. Create a new chat.

    <img src="../ex1.0/images/new-task.png" alt="new task" width="60%"/>

2. Drag and drop the image [manage-travels-object-page.png](../../manage-travels-object-page.png) from the images folder into the Copilot Chat window to attach it as context.

3. Copy and paste the following prompt into the task input and execute the task:
    ```
    Extract data from the attached Image. Do not inspect any other image files in the workspace.
    ```
    ![extract image](./images/extract-image.png)

4. Verify that the extracted data matches the image.

    ![extracted data](./images/extracted-data.png)

5. Copy and paste the following prompt into the task input and execute the task:
    ```
    Modify the travel object page based on the extracted data:

    - Reorganize the General Information section into subsections as shown in the image.
    - Align all fields, sections, and structure precisely with the image.
    - Add a bookings table section below, displaying flight booking details.
    - Generate mock data for the bookings table.

    Create an implementation plan first, then proceed after confirmation.
    
    ```

6. Copilot prepares an implementation plan.

    <img src="./images/imp-plan.png" alt="copilot" width="60%"/>

7. Confirm the implementation plan by responding with "Yes" or "Proceed".

    ![travel object page](./images/execute-objpage.png)

8. After completion, verify the object page in the application preview:
    - Verify the object page header contains both title and description.
    - Make sure the fields in the **General Information** section are arranged as per the Image uploaded to the context.

    ![travel object page](./images/travel-objpage.png)

## Troubleshoot

- The booking table does not appear below General Information section.
    Execute the prompt: `Change section layout to page for travel object page`.

- If the object page title is not visible, execute the prompt: `Object page title not visible`

    ![no title](./images/objpage-no-title.png)

## Summary

You have successfully modified the travel object page based on the Image, including the bookings table section.

Continue to - [Exercise 2.1 - Add Custom Section with RichTextEditor Building Block](../ex2.1/README.md)
