---
title: Pieces MCP + Claude Desktop Integration
path: /mcp/claude-desktop
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with Claude Desktop lets you use Pieces Long-Term Memories captured by PiecesOS without any third-party applications.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with Claude Desktop
metaDescription: Discover 2 different ways to configure the Pieces MCP to provide your workflow context to Claude Desktop, allowing you to work smarter.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/MCP/claude_desktop_mcp.jpg"
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/pieces_mcp_claude_desktop/pieces_mcp_for_claude_desktop_banner.jpg" alt="" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp/get-started) with Claude Desktop is a powerful way to bring your workflow context directly into your AI assistant.

With this integration, you'll have an in-Desktop Claude agent that knows more about your projects than just the files you copy and paste.

You can ask questions about prior work, like *“What decision did I make in last week’s sprint review?”* and instantly reuse that context without searching through notes or commits.

Learn how to integrate the Pieces MCP into Claude Desktop by following the steps below.

<Callout type="info">
  It is imperative that you download and/or update <a target="_blank" href="https://claude.ai/download">Claude Desktop</a> to the latest, most up-to-date version to ensure compatibility with Pieces MCP.
</Callout>

## Prerequisites

There are **two** main things you need to do to connect Pieces with Claude Desktop as an MCP: have an active instance of PiecesOS running and and turn on the Long-Term Memory engine.

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

## Setting Up Claude Desktop

There are **two methods** to set up the Pieces MCP for Claude Desktop—either configuring the server connection manually with a direct command, or using the [Pieces CLI ](/products/cli)to configure it automatically.

### Method 1: Manual Configuration (Direct MCP Command)

This method involves editing Claude Desktop’s MCP configuration file to point directly to a CLI command that starts the Pieces MCP server.

<Callout type="info">
  With this method, the Claude MCP config points to the Pieces CLI executable and runs `pieces mcp start` whenever Claude starts. This is different from using the CLI to configure Claude directly (Method 2).
</Callout>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/pieces_mcp_claude_desktop/claude_manual_config.png" alt="" align="center" fullwidth="true" />

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
    Paste the following JSON, adjusting the path to your `pieces.exe` if different:

    ```powershell
    jsonCopyEdit{
      "mcpServers": {
        "Pieces": {
          "command": "C:\\Users\\<YourUser>\\AppData\\Local\\Programs\\Python\\Python313\\Scripts\\pieces.exe",
          "args": [
            "--ignore-onboarding",
            "mcp",
            "start"
          ]
        }
      }
    }
    ```
  </Step>

  <Step title="Save & Restart Claude Desktop">
    Fully quit and reopen Claude Desktop.
  </Step>

  <Step title="Enable Pieces MCP">
    Start prompting Claude—if properly set up, you will be prompted by Claude to enable and allow (on a case-by-case basis, or via `always allow`) Claude to pass prompts through the `ask_pieces_ltm` tool.

    This utility communicates with PiecesOS and your local repository of saved workflow context.
  </Step>
</Steps>

### Method 2: Using the Pieces CLI to Configure Automatically

This method uses the Pieces CLI to automatically set up and configure Pieces MCP for Claude Desktop.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/pieces_mcp_claude_desktop/generic_cli_shot.png" alt="" align="center" fullwidth="false" />

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
    pieces mcp setup --claude
    ```

    This will:

    * Detect your Claude Desktop MCP config location.

    * Insert the correct `mcpServers` entry for Pieces.

    * Point Claude directly to the MCP server without requiring manual JSON edits.
  </Step>

  <Step title="Restart Claude Desktop">
    Once the command completes, restart Claude Desktop and confirm that the Pieces MCP server is connected.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/pieces_mcp_claude_desktop/cli_mcp_setup_claude_desktop.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

## Using Pieces MCP Server in Claude Desktop

Once integrated, you can utilize Pieces LTM directly in Claude Desktop.

1. **Open a Claude Chat**\
   Launch a new conversation in Claude Desktop.

2. **Prompt with Context**\
   Ask Claude questions about prior work or files (e.g., *“What was I doing for work yesterday?”*).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/pieces_mcp_claude_desktop/what_have_i_been_working_on.png" alt="" align="center" fullwidth="true" />

3. **Verify MCP Tools Are Active**\
   If configured correctly, Claude will automatically use the `ask_pieces_ltm` tool to pull relevant context.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/pieces_mcp_claude_desktop/general_claude_desktop_output_1.png" alt="" align="center" fullwidth="true" />

## Troubleshooting

If you’re experiencing issues integrating [Pieces MCP](/products/mcp/get-started) with Claude Desktop:

1. **Verify PiecesOS Status**\
   Ensure PiecesOS is actively running on your system.

2. **Confirm LTM Engine Activation**\
   [Long-Term Memory (LTM-2.7)](/products/core-dependencies/pieces-os/quick-menu#ltm-27-engine) must be enabled in PiecesOS.

3. **Single MCP Instance**\
   Avoid running multiple Pieces MCP instances in different apps simultaneously.

4. **Check MCP Server Status in Claude**\
   Use the Developer Console (`Ctrl+Shift+I`) to confirm connection messages.

5. **Review Configuration**\
   If using *Method 1*, ensure your JSON paths are correct.\
   If using *Method 2*, rerun:

   ```powershell
   pieces mcp setup --claude
   ```

***

You’re now ready to enhance your Claude Desktop experience with the Pieces MCP, enabling powerful, context-aware conversations and seamless access to your workflow history.