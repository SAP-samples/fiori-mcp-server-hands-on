# Build a Full-Stack SAP Fiori Elements App on a CAP project using AI

## Overview

AI can carry a lot of the repetitive work in SAP development, if you let it drive the right tools. In this tutorial you do exactly that: you talk to an AI assistant in plain language, and it builds a CAP service and a SAP Fiori Elements app on top of it, then helps you enhance both.

Two MCP servers do the heavy lifting: the CAP MCP server handles the backend, and the MCP server for SAP Fiori generates and enhances the app. That server helps in more than one way, and you meet each along the way: change tools that apply edits, a doc search that returns matching documentation snippets, and SAP Fiori development skills that package a whole task. You start from a travel booking scenario, build a CAP service with CDS models, generate a List Report and Object Page, and then extend the UI and the service step by step, all through natural-language prompts.

You will gain comprehensive knowledge of AI-assisted full-stack development, and learn how to kickstart your SAP Fiori Elements application development.

## Using AI during App Development

We are using GitHub Copilot as AI coding assistant within VS Code and Anthropic Claude Sonnet/Opus LLM (Large Language Model) throughout the exercises. When developing SAP Fiori applications with LLMs, you may encounter situations where a prompt is not executed as intended, or technical errors occur when calling MCP server tools. Knowing how to approach these issues systematically can save time and prevent disruption. GitHub Copilot and the chosen LLM are powerful assistants for problem resolution.

## Exercises

Begin your exercises here. At the end of each section, there is a link to continue to the next section.

- [Getting Started - Set up your AI Development Environment](./exercises/ex0/)

- [Exercise 1 - Create CAP Project and Fiori List Report App based on Image](./exercises/ex1.0/)
    - [Exercise 1.1 Enable automatic data loading in List Report](./exercises/ex1.1/)
    - [Exercise 1.2 Add new column destination to list report table](./exercises/ex1.2/)
    - [Exercise 1.3 Add Analytical chart to list report page](./exercises/ex1.3/)

- [Exercise 2 - Modify travel object page based on Image](./exercises/ex2.0/)
    - [Exercise 2.1 Add Custom Section with RichTextEditor Building Block](./exercises/ex2.1/)

- [Exercise 3 - Add Object Page for Booking Details](./exercises/ex3.0/)

## Contributing
If you wish to contribute code, offer fixes or improvements, please send a pull request. Due to legal reasons, contributors will be asked to accept a DCO when they create the first pull request to this project. This happens in an automated fashion during the submission process. SAP uses [the standard DCO text of the Linux Foundation](https://developercertificate.org/).

## License
Copyright (c) 2026 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSE) file.
