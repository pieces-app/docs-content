---
title: Get Started
path: /cli/tui/get-started
visibility: PUBLIC
status: PUBLISHED
description: Get started with the Pieces CLI Text User Interface (TUI) for an interactive terminal experience.
metaTitle: Get Started with Pieces TUI
metaDescription: Learn how to set up and use the Pieces CLI Text User Interface (TUI) for managing materials and interacting with Pieces Copilot.
---

<pieces-pro-cta />

## TUI Prerequisites

Before you can use the Pieces CLI Text User Interface (TUI), you'll need:

* **Python 3.xx:** [Python](https://www.python.org/downloads/) is required to be installed on your development machine.

* **PiecesOS:** The core engine that powers all Pieces tools. [Learn more about PiecesOS](/products/core-dependencies/pieces-os).


* **Pieces CLI:** The command-line interface that powers the TUI. [Learn how to install the Pieces CLI](/products/cli/get-started).

<Callout type="alert">
  PiecesOS must be installed to use the Pieces CLI and ensure it works properly.

  We also suggest using the Pieces Desktop App for better functionality.
</Callout>

### Sign in Required

Pieces requires all users to sign in before using any plugins or extensions. You'll be prompted to authenticate if you haven't already. For help, see our [sign-in guide](/products/meet-pieces/sign-into-pieces).

## Installing the TUI

The TUI is included with the Pieces CLI installation, but requires a one-time setup step on first launch. Once you have the CLI installed, you can set up and access the TUI.

On your first launch, you'll need to run `pieces tui install` to download and set up the TUI components. This is a one-time setup process.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/tui/installing_pieces_tui2.gif" alt="" align="center" fullwidth="true" />

<Callout type="info">
  If you haven't installed the Pieces CLI yet, follow the [CLI installation guide](/products/cli/get-started) first.
</Callout>

## Launching the TUI

To start using the TUI, follow these simple steps:

<Steps>
  <Step title="Open Your Terminal">
    Open your terminal application:
    * **Windows:** Press `win+r`, type `cmd` or `powershell`, and press `enter`
    * **macOS:** Press `cmd+space`, type `terminal`, and press `return`
    * **Linux:** Press `ctrl+alt+t` or search for "Terminal" in your applications
  </Step>

  <Step title="Launch the TUI">
    After installation, launch the TUI with:

    ```bash
    pieces tui
    ```

    This will launch the interactive Text User Interface.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/tui/launching_pieces_tui.gif" alt="" align="center" fullwidth="true" />
  </Step>

  <Step title="Start Interacting">
    Once the TUI loads, you'll see the main interface with:
    * A sidebar for navigation
    * A chat area for conversations with Copilot
    * Keyboard shortcuts for quick access
  </Step>
</Steps>

### Navigation Shortcuts

Use these keyboard shortcuts to navigate efficiently:

* `tab`: Navigate between interface elements
* `shift+ctrl+w`: Switch to Workstream view
* `ctrl+e`: Toggle edit mode in Workstream
* `ctrl+s`: Save changes
* `esc`: Return to previous view or exit current mode

## Your First TUI Session

Let's walk through your first interaction with the TUI to get you comfortable with the interface.

### Starting a Conversation with Copilot

<Steps>

  <Step title="Launch the TUI">
    Open your terminal and run `pieces tui`
  </Step>

  <Step title="Begin Typing">
    Once the interface loads, you can start typing directly in the chat area at the bottom of your terminal.
  </Step>

  <Step title="Get Copilot Response">
    Press `return` (macOS) or `enter` (Windows/Linux) to send your question. Copilot will open a new chat and respond if not already in a chat.
  </Step>
</Steps>
<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/tui/old_pieces_chat.png" alt="" align="center" fullwidth="true" />

<Callout type="tip">
  **New Chat Button:** You can start a fresh conversation anytime by clicking the "+new chat" button at the top of the left sidebar. This creates a new chat session while keeping your previous conversations accessible.
</Callout>

### Exploring Workstream Activities

<Steps>
  <Step title="Switch to Workstream View">
    Use `shift+ctrl+w` to navigate to the Workstream section.
  </Step>

  <Step title="Browse Activities">
    Use arrow keys to navigate through your workstream activities in the left sidebar.
  </Step>

  <Step title="Open Workflow Activity">
    Press `return` (macOS) or `enter` (Windows/Linux) to open the selected workflow.
    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/tui/workstream_selected.png" alt="" align="center" fullwidth="true" />

  </Step>

  <Step title="View Content">
    Select an activity to view its content in read mode.
  </Step>

  <Step title="Edit if Needed">
    Press `ctrl+e` to switch to edit mode and make changes.
  </Step>
</Steps>

## Uninstalling

Follow the steps below to uninstall the TUI.

<Steps>
  <Step title="Open a Terminal">
    Opening a terminal on your device depends on your platform: Open your OS' search bar and enter `terminal` (macOS/Linux) or `CMD` (Windows).
  </Step>

  <Step title="Run Uninstall Command">
    Choose your OS:

    <Tabs>
      <Tab label="Windows">
        Uninstall on Windows:

        ```bash
        py -m pip uninstall pieces-cli
        ```
      </Tab>
      <Tab label="macOS">
        Uninstall with Homebrew on macOS:

        ```bash
        brew uninstall pieces-cli
        ```
      </Tab>
      <Tab label="Linux">
        Uninstall with pip3 on Linux:

        ```bash
        pip3 uninstall pieces-cli
        ```
      </Tab>
    </Tabs>

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/tui/uninstall_pieces_cli.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

<Callout type="info">
  If you also want to uninstall PiecesOS, [follow these steps](/products/core-dependencies/pieces-os/manual-installation#uninstalling-piecesos).
</Callout>


