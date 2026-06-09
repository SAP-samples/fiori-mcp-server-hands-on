# Add Custom Section with RichTextEditor Building Block

1. Create a new chat.

    <img src="../ex1.0/images/new-task.png" alt="new task" width="60%"/>

2. Enter the following prompt in the task input:
    ```
    Your task is to visualize the description field of the trip as a rich text editor on the object page of the travel management app. Implement in two steps:
     1. Add a custom section at the last position of the object page
     2. Use the rich text editor building block in the new section to show the description field. Ensure each button group for the Rich text editor has an ID
    Create implementation plan first, then proceed with confirmation.
    Consult MCP servers.

    ```

3. Execute the task.

    ![buildingblock](./images/imp-plan.png)

4. Confirm the implementation plan by responding with "Yes" or "Proceed".

    ![buildingblock](./images/buildingblock-imp-plan.png)

5. After completion, verify that the travel description section is visible on the travel object page.

6. Click the **Edit** button in the top right corner.

7. In the travel description section, select some text and apply bold formatting.

8. Click **Save** and verify that the object has been saved successfully.

    ![buildingblock](./images/buildingblock.png)

## Troubleshoot

1. No **Edit** button on the travel object page. Execute the prompt:
    ```
    Enable draft mode for travel entity
    ```

## Summary

You have successfully added a custom section with a RichTextEditor building block to the travel object page.

Continue to - [Exercise 3.0 - Add Object Page for Booking Details](../ex3.0/README.md)
