[![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/fiori-mcp-server-hands-on)](https://api.reuse.software/info/github.com/SAP-samples/fiori-mcp-server-hands-on)

# Hands-on | Create great UX with AI, SAP Design System, SAP Fiori elements, and SAPUI5 

## Overview

In this hands-on tutorial you will work through a set of exercises that highlight the benefits and capabilities of the **SAP Design System**, the **Figma** design tool, and the **MCP servers by SAP and for Figma** to create and modify SAP Fiori applications with the help of AI coding assistants. 

You will gain comprehensive knowledge of AI assisted full-stack development, and learn how to use Figma and the SAP Design System to kickstart your SAP Fiori elements application development.

## Using AI during App Development

We are using Cline as AI client within SAP Business Application Studio (SBAS) and Anthropic claude-4.5-sonnet LLM (Large Language Model) throughout the exercises. When developing SAP Fiori applications with LLMs, you may encounter situations where a prompt is not executed as intended, or technical errors occur when calling MCP server tools. Knowing how to approach these issues systematically can save time and prevent disruption. Cline and the choosen LLM are powerful assistants for problem resolution.

### General steps in case of issues:

[Detailed steps and examples of resolving common issues](./exercises/troubleshoot/)

1. Verify connectivity:
    - Check if your machine has network access.
    - Confirm that the MCP server is up and running.

2. Approach errors systematically
    - Pause before panicking
        - Use natural pauses when the client asks for approval to inspect the current results and chat history.    
        - Stop execution with the "Cancel" button. You can always proceed from there with a new prompt
    - Identify the source: Check if the issue is:
        - CDS compiler error
        - SQLite/database error
        - Console/browser runtime error

3. Using the LLM to solve an issue
    - The LLM occasionally makes mistakes, or forgets required steps leading to error situations
    - But the LLM can read the terminal output and react to API reponses, and correct error visible there
    - Other issues, like from browser console output, can be resolved by copy-pasting the full error message into the chat and ask for a fix in a prompt
    - LLM works best when exact messages are provided rather than manual descriptions.

4. Use Restore Points if Needed
    - If a solution strategy does not work, you can always restore the files and chat to a previous checkpoint using Cline’s restore functionality.

5. Don’t be afraid to retry an exercise or step after restoring to a checkpoint.

## Exercises

Begin your exercises here. At the end of each section, there is a link to continue to the next section.

- [Exercise 1 - Open the Figma Design file in Figma](./exercises/ex1.0/)
  - [Exercise 1.1 - Adjust the buttons in the object page header](./exercises/ex1.1/)
  - [Exercise 1.2 - Add a form item in the object page](./exercises/ex1.2/)
  - [Exercise 1.3 - Edit the new form item in the object page](./exercises/ex1.3/)
  - [Exercise 1.4 - Create a personal access token](./exercises/ex1.4/)

- [Set up your AI Development Environment](./exercises/ex1.6/)

- [Exercise 2 - Create CAP Project and Fiori List Report App based on Image](./exercises/ex2.0/)
    - [Exercise 2.1 Enable automatic data loading in List Report](./exercises/ex2.1/)
    - [Exercise 2.2 Add new column destination to list report table](./exercises/ex2.2/)
    - [Exercise 2.3 Add Analytical chart to list report page](./exercises/ex2.3/)

- [Exercise 3 - Modify travel object page based on Image](./exercises/ex3.0/)
    - [Exercise 3.1 Add Custom Section with RichTextEditor Building Block](./exercises/ex3.1/)

- [Exercise 4 - Add Object Page for Booking Details](./exercises/ex4.0/)

## Contributing
If you wish to contribute code, offer fixes or improvements, please send a pull request. Due to legal reasons, contributors will be asked to accept a DCO when they create the first pull request to this project. This happens in an automated fashion during the submission process. SAP uses [the standard DCO text of the Linux Foundation](https://developercertificate.org/).

## License
Copyright (c) 2026 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSE) file.
