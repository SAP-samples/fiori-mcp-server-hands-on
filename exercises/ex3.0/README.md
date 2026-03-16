# Modify travel object page based on Image

1. Close previous task.

    <img src="../ex2.0/images/close-task.png" alt="close task" width="60%"/>

2. Select **Plan mode**.

    ![plan mode](../ex2.0/images/plan-mode.png)

3. Enter the following prompt in the task input (don't execute yet):
    ```
    Modify the travels object page based on the figma design from this link
    <insert_link_here>
    
    The object page shall include a bookings table section.
    Add mock data for the bookings table.
    ```

4. In the web browser tab with your Figma design, select **Screen 2 - Object Page**, right-click on it, and select **Copy/Paste as** → **Copy link to selection**.

5. Insert the link into the prompt text.

6. Press `Enter` to start the task.

7. Cline will generate an **Implementation Plan**.

8. Review the plan once it's ready.

9. Switch to **Act mode**.

10. Cline will execute the implementation plan.

11. After completion, verify the object page in the application preview:
    - Verify object page header contains both title and description.
    - Make sure fields in the **General Information** are arranged as per image.

    ![travel object page](./images/travel-objpage.png)

## Troubleshoot

1. Update the Object Page Title and Description based on the image. Use the following prompt:
    ```
    Set the travel description as the object page title and display the travel title below it.
    ```

2. Some fields in the **General Information** section are missing. Use the following prompt:
    ```
    Arrange or add fields in the General Information section as shown in the image @/travel-object-page.png.
    ```

## Summary

You have successfully modified the travel object page based on the Figma design, including the bookings table section.

Continue to - [Exercise 3.1 - Add Custom Section with RichTextEditor Building Block](../ex3.1/README.md)
