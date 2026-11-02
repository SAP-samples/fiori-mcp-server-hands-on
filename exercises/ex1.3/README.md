# Add an analytical column chart to the List Report

1. Create a new chat.

    <img src="../ex1.0/images/new-task.png" alt="new task" width="60%"/>

2. Enter the prompt in the task input:
    ```
    /sap-fiori-analytical-chart
    Add an analytical column chart to the List Report (ALP) 
    that displays the sum of total price per destination. 
    Show analytical chart above table.
    ```

3. Execute the prompt. Copilot will consult the skill on how to implement analytical charts.

4. After completion, verify that the analytical chart and table are displayed on the list report page. 

    ![analytical chart](./images/analytical-chart.png)

## Troubleshooting

- If the chart is not visible on the list report page, execute the following prompt: `In Manifest, views.paths must be at the settings level, not inside controlConfiguration`

- If you see `[50017] - Invalid data binding`, execute the following prompt: `/sap-fiori-analytical-chart verify analytical chart implementation`

- If you see `Invalid data - Some measures have different units` because test data might have mixed currencies, execute the following prompt: `Some measures have different units. Use Dollar as currency throughout the application`

## Summary

You have successfully added an analytical column chart displaying average price per destination to the List Report page.

Continue to - [Exercise 2.0 - Modify travel object page based on Image](../ex2.0/README.md)
