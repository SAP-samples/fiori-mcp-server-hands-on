# Add Object Page for Booking Details

1. Create a new chat.

    <img src="../ex1.0/images/new-task.png" alt="new task" width="60%"/>

2. Download the [bookings-object-page.png](../../bookings-object-page.png) image to your local disk.

    ![download](./images/download-image.png)

3. Upload the image to the Copilot context.

    ![context](../ex1.0/images/context.png)

4. Enter the following prompt in the task input:
    ```
    Create a booking detail object page based on the Image attached to the context.

    Create implementation plan first, then proceed with confirmation.
    Consult MCP servers.
    ```

5. Execute the task.

    ![second object page](./images/imp-plan.png)

6. Confirm the implementation plan by responding with "Yes" or "Proceed".

    ![booking object page](./images/execute-booking-objpage.png)

7. After completion, navigate to the Travel object page and click on a row in the bookings table to open the booking object page. Verify the booking object page appears correctly in the application preview.

    ![booking object page](./images/booking-objpage.png)

## Troubleshoot

- Booking Extras table does not appear below General Information section.
    Execute the prompt: `Change section layout to page for booking object page`.
- The booking table doesn't have navigation to object page. Execute the prompt `Ensure manifest configuration for new object page`.
- Section **Booking Extras** is missing in the booking object page. Execute the prompt: `booking extras table section is missing`.
- The Booking Extras table has no data. Execute the prompt: `add mock data for booking extras`.
- Error `Composition in draft-enabled entity can't lead to another entity with "@odata.draft.enabled" (in entity:"TravelService.Travel"/element:"Bookings")`. Copy and paste error message to Copilot to fix the issue.

## Summary

Congratulations, you have completed all exercises!
