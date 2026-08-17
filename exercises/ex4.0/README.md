# Add Object Page for Booking Details

1. Create a new chat.

    <img src="../ex2.0/images/new-task.png" alt="close task" width="60%"/>

2. Enter the following prompt in the task input (don't execute yet):
    ```
    Create a booking detail object page based on the Figma design from this link
    <insert_link_here>

    Create implementation plan first, then proceed with confirmation.
    Consult MCP servers.
    ```

3. In the web browser tab with your Figma Design, select **Screen 3 - Object Page**, right-click on it, and select **Copy/Paste as** → **Copy link to selection**.

4. Insert the link into the prompt text.

5. Press `Enter` to start the task.

6. Copilot will execute the task.
    ![booking object page](./images/execute-booking-objpage.png)

7. After completion, check the booking object page in the application preview.

    ![booking object page](./images/booking-objpage.png)

## Troubleshoot

- The booking table doesn't have navigation. Remind the LLM to add the new page to the app.
- Error `Composition in draft-enabled entity can't lead to another entity with "@odata.draft.enabled" (in entity:"TravelService.Travel"/element:"Bookings")`. Copy and paste the above error message, and Copilot will fix the issue.
- Section **Booking Extras** is missing in the booking object page. Execute the prompt: `booking extras table section is missing`.
- The Booking Extras table has no data. Execute the prompt: `add mock data for booking extras`.

## Summary

Congratulations, you have completed all exercises!
