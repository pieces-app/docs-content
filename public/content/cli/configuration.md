---
title: Configuration
path: /cli/configuration
visibility: PUBLIC
status: PUBLISHED
---

***

## Settings and Models

Configure the Pieces CLI by changing both language models and the code editor.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/configuration/available_models.png" alt="" align="center" fullwidth="true" />

> Available models and settings configuration interface

## Supported LLMs

The Pieces CLI supports 26 cloud-based language models that you can switch between.

We continually update and configure our plugins and extensions to ensure compatibility with the latest large language models (LLMs).

| Supported LLMs                | Supported LLMs   |
| ----------------------------- | ---------------- |
| Gemini-2.5 Flash Preview      | GPT-4o Mini      |
| o4 Mini                       | Gemini-1.5 Pro   |
| o3                            | Gemini-1.5 Flash |
| GPT-4.1                       | GPT-4o           |
| Gemini-2.0 Flash Lite         | Claude 3 Haiku   |
| Gemini-2.5 Pro Experimental   | Claude 3 Sonnet  |
| Gemini-2.5 Pro Preview        | Claude 3 Opus    |
| Claude 3.7 Sonnet             | GPT-4 Turbo      |
| o3 Mini                       | (Gemini)         |
| o1                            | GPT-3.5-turbo    |
| Gemini-2.0 Flash Experimental | GPT-4            |
| Claude 3.5 Sonnet             | Codey (PaLM2)    |
| Claude 3.5 Haiku              | (PaLM2)          |

[Read documentation on how to switch your Pieces Copilot Runtime (LLM)](/products/cli/copilot/llms-settings) utilized by the Pieces CLI.

## Settings Overview

A breakdown of each adjustable setting you can configure in the Pieces CLI, organized by section.

### List Applications

View all registered applications and verify which integrations are available.

Run `list apps` to see every application you've registered. This prints a table of app names and IDs so you can verify which integrations are available.

### List Models

Display all language models configured for the `ask` command.

Use `list models` to display all language models you've configured for the `ask` command. The output shows each model's name and index, and which is currently active.

### View Configuration

Print your current IDE selection for code editing.

Run `config` to print your current IDE selection for code editing.

### Edit Configuration

Open your config file in your preferred editor to adjust settings.

Execute `config --editor <editorName>` to open your config file in the editor of your choice. Simply adjust values (for example, change `timeout: 10` to `timeout: 20`) and save—your changes take effect immediately.

### Login

Authenticate with your Pieces Cloud account to sync materials and access private resources.

Run `login` to authenticate with your Pieces Cloud account. You'll be prompted for credentials in a web browser; once you're logged in, you can sync materials and access private resources in your [Pieces Drive](/products/cli/drive).

### Logout

Clear your saved credentials and end your session.

Use `logout` to clear your saved credentials and end your session. This is useful when switching accounts or working on a shared machine.

### Contribute

Start a contribution workflow to submit improvements to the CLI.

Kick off a contribution workflow with `contribute`. You'll be guided through describing your changes, and a pull-request template will open in your browser so you can submit improvements to the CLI.

### Install PiecesOS

Download and set up PiecesOS, which provides background services and a graphical dashboard.

Run `install` to download and set up the [PiecesOS](/products/core-dependencies/pieces-os), which provides background services, like Pieces Drive, and a graphical dashboard for non-CLI related tasks.

### Open PiecesOS

Launch the desktop app or helper Applet.

Use `open` to launch the desktop app or helper Applet. If it isn't already running, this command starts the service and brings up the GUI.

***

## Next Steps

For additional support resources, check out our [troubleshooting guide.](/products/cli/troubleshooting)
