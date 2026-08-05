---
title: Pieces MCP + Claude Integration
path: /mcp/claude-desktop
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with Claude Desktop and Claude Code lets you use Pieces Long-Term Memories captured by PiecesOS without any third-party applications.
metaTitle: Pieces MCP + Claude Desktop & Code | Setup Guide
metaDescription: Discover different ways to configure the Pieces MCP to provide your workflow context to Claude Desktop and Claude Code, allowing you to work smarter.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/MCP/claude_desktop_mcp.jpg"
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/pieces_mcp_claude_desktop/pieces_mcp_for_claude_desktop_banner.jpg" alt="Pieces MCP for Claude Desktop banner" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp) with Claude Desktop or Claude Code is a powerful way to bring your workflow context directly into your AI assistant.

With this integration, you'll have a Claude agent that knows more about your projects than just the files you copy and paste.

You can ask questions about prior work, like *"What decision did I make in last week's sprint review?"* and instantly reuse that context without searching through notes or commits.

Learn how to integrate the Pieces MCP into Claude Desktop or Claude Code by following the steps below.

<Callout type="info">
  It is imperative that you download and/or update <a target="_blank" href="https://claude.ai/download">Claude Desktop</a> to the latest, most up-to-date version to ensure compatibility with Pieces MCP.
</Callout>

## Prerequisites

There are **two** main things you need to do to connect Pieces with Claude as an MCP:

<Steps>
  <Step title="Install & Run PiecesOS">
    Ensure PiecesOS is installed and running. This lets the MCP server connect with your workflow data and share context with Claude.

    If you don't have [PiecesOS](/products/core-dependencies/pieces-os/manual-installation), you can download it with the [Pieces Desktop App](/products/desktop/download) or get it separately [here](https://pieces.app/download).
  </Step>

  <Step title="Enable Long-Term Memory">
    To let the MCP server use your workflow context, you need to turn on the Long-Term Memory Engine (LTM-2.7) through the Pieces Desktop App or [the PiecesOS Quick Menu in your toolbar.](/products/core-dependencies/pieces-os/quick-menu)
  </Step>
</Steps>

## Installing PiecesOS & Configuring Permissions

Follow the instructions below for a detailed guide on setting up and configuring PiecesOS to correctly pass captured workflow context to the Pieces MCP server.

<pos-download-guide />

## Setting up Pieces MCP for Claude Desktop

Connecting Claude Desktop used to mean installing extra tools on your machine. Pieces now includes everything you need on macOS, Windows, and Linux. Pick Claude Desktop, click `Connect`, and Pieces writes the setup for you.

The recommended path is one-click setup in Pieces Desktop. Advanced options (Pieces CLI or editing a config file by hand) are below if you need them.

### One-Click Setup via Pieces Desktop (Recommended)

Connect Claude Desktop from *MCP Connections* in Pieces Desktop. Pieces configures Claude for you using a connection helper that ships inside PiecesOS; nothing else to install.

<Steps>
  <Step title="Open MCP Settings">
    In Pieces Desktop, click your `User Profile` in the top left, then hover over `Settings` and select `MCP`.
  </Step>

  <Step title="Find MCP Connections">
    Scroll down to the *MCP Connections* section. You'll see a list of supported clients with `Connect` buttons.
  </Step>

  <Step title="Quit Claude Desktop if it is running (Linux)">
    On Linux, especially Snap or Flatpak installs, quit Claude Desktop before connecting. If Claude is still running, it can overwrite the settings Pieces just saved. Pieces notices when Claude Desktop is already open and walks you through quitting first.
  </Step>

  <Step title="Click Connect">
    Click the `Connect` button next to **Claude Desktop**. Pieces saves the connection settings for you. You do not need to install anything else.
  </Step>

  <Step title="Restart Claude Desktop">
    When the new settings need a restart, Pieces shows a *Restart Claude Desktop* prompt. Click `Restart Claude Desktop now` to relaunch Claude, or `Got it` if you will restart yourself. Once connected, a green checkmark appears next to Claude Desktop in the MCP Connections list.
  </Step>
</Steps>

<Callout type="tip">
  Snap and Flatpak installs are supported. As long as Claude Desktop points at the PiecesOS executable, the MCP connection works with no additional install.
</Callout>

<Callout type="info">
  To disconnect later, click the `⋮` menu next to the connected client and select **Disconnect**, or click the red `✕` next to the connection entry.
</Callout>

### Advanced: Manual Configuration (Direct MCP Command)

This method edits Claude Desktop’s MCP configuration file to point at a CLI command that starts the Pieces MCP server. Use one-click setup above unless you need a custom path.

<Callout type="info">
  With this method, the Claude MCP config points to the Pieces CLI executable and runs `pieces mcp start` whenever Claude starts. This is different from using the CLI to configure Claude directly (the next advanced method).
</Callout>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/pieces_mcp_claude_desktop/claude_manual_config.png" alt="Claude Desktop manual MCP configuration process" align="center" fullwidth="true" />

<Steps>
  <Step title="Install the Pieces CLI">
    Make sure the [Pieces CLI](/products/cli) is installed.

    In your terminal, run the following commands:

    ```powershell
    py -m pip install --upgrade pip
    py -m pip install pieces-cli
    ```

    Next, confirm that the installation was successful:

    ```powershell
    pieces --version
    ```
  </Step>

  <Step title="Locate the Pieces CLI Executable">
    The executable path depends on your OS and Python installation method.

    For example:

    1. **Windows →** `C:\Users\<YourUser>\AppData\Local\Programs\Python\Python3XX\Scripts\pieces`

    2. **macOS →** `usr/local/bin/pieces`

    3. **Linux →** `home/<YourUserNameHere>/.local/bin/pieces`
  </Step>

  <Step title="Locate or Create the Claude Desktop Config File">
    Claude Desktop stores its MCP configuration in a user-specific location for each OS.

    Depending on your platform, this might be:

    1. **Windows →** `C:\Users\<YourUser>\AppData\Roaming\Claude\claude_desktop_config.json`

    2. **macOS →** `~/Library/Application Support/Claude/claude_desktop_config.json`

    3. **Linux →** `~/.config/Claude/claude_desktop_config.json`

    If the file exists → open it in a text editor.\
    If it doesn’t exist → create it manually in that directory.
  </Step>

  <Step title="Add MCP Server Configuration">
    Paste the following JSON into your Claude config file, adjusting the path to your `pieces` executable for your OS:

    ```json
    {
      "mcpServers": {
        "pieces": {
          "command": "/Users/<YourUser>/venv/bin/pieces",
          "args": [
            "--ignore-onboarding",
            "mcp",
            "start"
          ]
        }
      }
    }
    ```

    **Path examples by OS:**
    * **macOS/Linux** — `/Users/<YourUser>/venv/bin/pieces` or `~/.local/bin/pieces`
    * **Windows** — `C:\Users\<YourUser>\AppData\Local\Programs\Python\Python3XX\Scripts\pieces.exe`
  </Step>

  <Step title="Save & Restart Claude Desktop">
    Fully quit and reopen Claude Desktop.
  </Step>

  <Step title="Enable Pieces MCP">
    Start prompting Claude. If properly set up, you will be prompted by Claude to enable and allow (on a case-by-case basis, or via `always allow`) Claude to pass prompts through the `ask_pieces_ltm` tool.

    This utility communicates with PiecesOS and your local repository of saved workflow context.
  </Step>
</Steps>

### Advanced: Using the Pieces CLI

This method uses the Pieces CLI to automatically set up and configure Pieces MCP for Claude Desktop.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/pieces_mcp_claude_desktop/generic_cli_shot.png" alt="Pieces CLI automatic MCP setup command" align="center" fullwidth="false" />

<Steps>
  <Step title="Install the Pieces CLI">
    Run the following commands to install the Pieces CLI if you haven’t already done so.

    ```powershell
    -m pip install --upgrade pip
    py -m pip install pieces-cli
    ```
  </Step>

  <Step title="Run the Automatic Setup Command">
    Run:

    ```powershell
    pieces mcp setup
    ```

    A platform selection menu appears with these options: *VS Code*, *Cursor*, *Claude Desktop*, *Windsurf*, *Claude Code*, *Raycast*, and *Warp*. Use the arrow keys to navigate, hover over *Claude Desktop* or *Claude Code*, then press `return` (macOS) or `enter` (Windows/Linux) to auto-install the MCP.
  </Step>

  <Step title="Restart Claude Desktop">
    Once the command completes, restart Claude Desktop and confirm that the Pieces MCP server is connected.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/pieces_mcp_claude_desktop/cli_mcp_setup_claude_desktop.png" alt="Successful Pieces MCP setup in Claude Desktop" align="center" fullwidth="true" />
  </Step>
</Steps>

## Adding Pieces MCP to Claude Code

Configure Pieces MCP for Claude Code to make it available across all your projects.

<Callout type="info">
  This section is specifically for Claude Code and does not work with Claude Desktop. For Claude Desktop, use the methods above.
</Callout>

<Steps>
  <Step title="Run the Claude Code MCP Add Command">
    In your terminal, run the following command:

    ```bash
    claude mcp add --scope user pieces --transport http http://localhost:39300/model_context_protocol/2025-03-26/mcp
    ```

    The `--scope user` flag makes Pieces MCP available globally across all your Claude Code projects, rather than just the current directory.
  </Step>

  <Step title="Start Using Pieces MCP in Claude Code">
    Open any project in Claude Code and start asking context-aware questions about your workflow, such as:

    * *"What patterns did I use in my last React component?"*
    * *"Show me the authentication flow I implemented yesterday."*
  </Step>
</Steps>

<Callout type="info">
  Claude Code will use the `ask_pieces_ltm` tool to pull relevant context from PiecesOS.
</Callout>

## Using Pieces MCP Server

Once integrated, you can utilize Pieces LTM directly in Claude Desktop or Claude Code.

1. **Start a Conversation**\
   Launch a new conversation in Claude Desktop or open a project in Claude Code.

2. **Prompt with Context**\
   Ask Claude questions about prior work or files (e.g., *"What was I doing for work yesterday?"*).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/pieces_mcp_claude_desktop/what_have_i_been_working_on.png" alt="Claude asking what user was working on" align="center" fullwidth="true" />

3. **Verify MCP Tools Are Active**\
   If configured correctly, Claude will automatically use the `ask_pieces_ltm` tool to pull relevant context.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/pieces_mcp_claude_desktop/general_claude_desktop_output_1.png" alt="Claude Desktop using Pieces MCP tool output" align="center" fullwidth="true" />

## Troubleshooting

If you're experiencing issues integrating [Pieces MCP](/products/mcp) with Claude Desktop or Claude Code:

1. **Verify PiecesOS Status**\
   Ensure PiecesOS is actively running on your system.

2. **Confirm LTM Engine Activation**\
   [Long-Term Memory (LTM-2.7)](/products/core-dependencies/pieces-os/quick-menu#ltm-2-engine) must be enabled in PiecesOS.

3. **Restart Claude Desktop**\
   After one-click Connect, use `Restart Claude Desktop now` in the Pieces prompt (or fully quit and reopen Claude) so the new config loads.

4. **Linux: Quit Claude Before Connecting**\
   If Connect fails or the connection disappears on Linux, quit Claude Desktop completely, connect again from *MCP Connections*, then restart Claude. See [Linux troubleshooting](/products/meet-pieces/troubleshooting/linux) for Snap and Flatpak notes.

5. **Single MCP Instance**\
   Avoid running multiple Pieces MCP instances in different apps simultaneously.

6. **Check MCP Server Status in Claude**\
   Use the Developer Console (`Ctrl+Shift+I`) to confirm connection messages.

7. **Review Advanced Configuration**\
   If you used a manual JSON edit, ensure paths are correct.\
   If you used the Pieces CLI, rerun:

   ```powershell
   pieces mcp setup
   ```

***

You’re now ready to enhance your Claude Desktop experience with the Pieces MCP, enabling powerful, context-aware conversations and seamless access to your workflow history.