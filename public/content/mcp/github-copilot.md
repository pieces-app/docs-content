---
title:  Pieces MCP + GitHub Copilot
path: /mcp/github-copilot
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP (Model Context Protocol) integration with GitHub Copilot allows you to leverage Pieces Long-Term Memory (LTM) directly within the Visual Studio Code editor, enhancing your coding workflow with seamless contextual information retrieval.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with GitHub Copilot
metaDescription: Discover how to integrate Pieces Model Context Protocol (MCP) with GitHub Copilot. Access Long-Term Memory within your IDE for enhanced, context-aware productivity.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/MCP/github_mcp.png"
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_gh_copilot/mcp-2-1.png" alt="" align="center" fullwidth="true" />

***

## Get Started

Connecting [Pieces MCP](/products/mcp/get-started) to **GitHub Copilot** enhances context-aware coding by linking your current task with past work.

This integration allows GitHub Copilot to provide insights like past implementations and peer-reviewed solutions.

You can ask context-rich questions, and Copilot can find answers from your local development history without searching through commits or messages.

Follow the steps below to integrate the Pieces MCP with GitHub Copilot for smarter, personalized AI assistance.

## Prerequisites

There are **\[2]** prerequisites for integrating Pieces with GitHub Copilot as an MCP—an active instance of **PiecesOS** and the fully-enabled **Long-Term Memory** engine.

<Steps>
  <Step title="Install & Run PiecesOS">
    Make sure that PiecesOS is installed and running. This is *required* for the MCP server to communicate with your personal repository of workflow data and pass context through to the GitHub Copilot chat agent.

    If you do not have PiecesOS, you can download it alongside the [Pieces Desktop App](/products/desktop/download) or [install it standalone](/products/core-dependencies/pieces-os/manual-installation#manual-download--installation) here.
  </Step>

  <Step title="Enable Long-Term Memory">
    For the MCP server to interact with your workflow context, you must enable the Long-Term Memory Engine (LTM-2.5) through the Pieces Desktop App or the [PiecesOS Quick Menu](/products/core-dependencies/pieces-os/quick-menu) in your toolbar.
  </Step>
</Steps>

### Installing PiecesOS & Configuring Permissions

Follow the detailed set-up instructions below for a detailed guide on setting up and configuring PiecesOS to correctly pass captured workflow context to the Pieces MCP server.

<pos-download-guide />

### SSE Endpoint

To use Pieces MCP with GitHub Copilot, you first need the Server-Sent Events (SSE) endpoint from PiecesOS:

```markdown
http://localhost:39300/model_context_protocol/2024-11-05/sse
```

<Callout type="alert">
  Keep in mind that the **specific port** (i.e., `39300`) PiecesOS is running on **may vary**.
</Callout>

To find the current SSE endpoint with the active instance of POS (including the current port number), open the PiecesOS Quick Menu and expand the **Model Context Protocol (MCP) Servers** tab.

There, you can copy the SSE endpoint with one click, which includes the active PiecesOS port number.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_pos_new.png" alt="" align="center" fullwidth="true" />

You can also do this in the Pieces Desktop App by opening the **Settings** view and clicking **Model Context Protocol (MCP).**

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_pfd_new.png" alt="" align="center" fullwidth="true" />

## Setting Up GitHub Copilot

You can now use the Pieces MCP with both Visual Studio Code and Visual Studio Code (Insider Edition).

Follow the steps below to get started—or watch the video below for a set-up tutorial and live demo.

<Embed src="https://www.youtube.com/watch?v=QT9J8XSKMM8" />

### via Visual Studio Code UI

Adding the Pieces MCP in the built-in MCP menu is the easiest method to setting up your Pieces MCP server and allows you to have the best experience while using the Pieces MCP.

<Steps>
  <Step title="Open the Command Palette">
    Open Visual Studio Code and launch the Command Palette by pressing `Cmd+Shift+P` on macOS or `Ctrl+Shift+P` on Windows/Linux.
  </Step>

  <Step title="Add a New MCP Server">
    In the Command Palette, type **MCP: Add Server** and select the command when it appears.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_gh_copilot/mcp_add_server_dropdown.png" alt="" align="center" fullwidth="true" />
  </Step>

  <Step title="Choose the Server Type">
    Select `HTTP (sse)` as the server type when requested.
  </Step>

  <Step title="Enter the SSE URL">
    Paste your SSE URL into the provided field.

    For Pieces, use:

    ```plaintext
    http://localhost:39300/model_context_protocol/2024-11-05/sse
    ```

    <Callout type="info">
      Remember to grab the specific SSE URL (with the *active* PiecesOS port) from either the PiecesOS or Pieces Desktop App MCP menu.
    </Callout>
  </Step>

  <Step title="Enter a MCP Server Name">
    When prompted to add a new MCP server, enter a name for your server, such as ‘Pieces\` or something easy to remember.

    Then, you can select the `User Settings` option to save the MCP server configuration in your VS Code user settings, so it can be accessed globally across different workspaces—or choose `Workspace Settings` to use it explicitly in your open project.
  </Step>

  <Step title="Save Your Configuration">
    Save your configuration. Your VS Code `settings.json` file should now include an entry similar to the example below:

    ```json
    {
      "mcpServers": {
        "Pieces": {
          "url": "http://localhost:39300/model_context_protocol/2024-11-05/sse"
        }
      }
    }
    ```

    Your GitHub Copilot chat, as long as the chat mode is in *Agent* mode, will now see Pieces as an MCP and automatically utilize the `ask_pieces_ltm` tool on-query.
  </Step>
</Steps>

### via Global MCP Configuration

You can manually add the MCP to your MCP settings `.JSON` by following the steps below.

<Steps>
  <Step title="Open the Visual Studio Code Settings">
    Click the **Settings Icon** on the bottom left of your IDE and select `Settings` from the list.
  </Step>

  <Step title="Search for MCP">
    In the VS settings, search for MCP in the search bar at the top of the page. The MCP section will appear—then, select `Edit in settings.json`.
  </Step>

  <Step title="Add the MCP Server Config .JSON">
    Replace the entire file, assuming you have no others, with the PiecesOS MCP server `.json`.

    ```json
    {
      "mcpServers": {
        "Pieces": {
          "url": "http://localhost:39300/model_context_protocol/2024-11-05/sse"
        }
      }
    }
    ```
  </Step>

  <Step title="Save the File">
    Save the configuration.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_gh_copilot/mcp_settings.png" alt="" align="center" fullwidth="true" />

    Your GitHub Copilot chat, as long as it’s in Agent mode, will now see PiecesOS as an MCP.
  </Step>
</Steps>

## Using Pieces MCP Server in GitHub Copilot

Once integrated, you can utilize Pieces LTM directly in Visual Studio Code.

<Steps>
  <Step title="Open GitHub Copilot Chat">
    Launch the GitHub Copilot chat interface in Visual Studio Code by clicking the Copilot icon, or by using `⌘+ctrl+i` (macOS) `ctrl+alt+i` (Windows/Linux).

    Change the Copilot mode from *Ask* to *Agent*.
  </Step>

  <Step title="Start Prompting">
    Enter your prompt, and click the **send** icon or press `return` (macOS) or `enter` (Windows/Linux) to send your query to the Copilot.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_gh_copilot/chatting_with_mcp.gif" alt="" align="center" fullwidth="true" />

    <Callout type="alert">
      Do not add the `ask_pieces_ltm` tool as *context* to the conversation. If you are running the chat in *Agent* mode—which is required for the Pieces MCP integration to operate successfully—it will automatically utilize this tool.
    </Callout>
  </Step>
</Steps>

<Card title="Hey!" image="https://cdn.hashnode.com/res/hashnode/image/upload/v1744223593411/98b96d7f-4ba7-456f-a8a5-b9c2bfffd92a.png">
  Check out this [MCP-specific prompting guide](/products/mcp/prompting) if you want to effectively utilize the Long-Term Memory Engine (LTM-2.5) with your new Pieces MCP server.
</Card>

## Troubleshooting Tips

If you’re experiencing issues integrating Pieces MCP with GitHub Copilot, follow these troubleshooting steps:

1. **Verify PiecesOS Status**: Ensure [PiecesOS is actively running](/products/core-dependencies/pieces-os/troubleshooting) on your system. MCP integration requires PiecesOS to be operational.

2. **Confirm LTM Engine Activation**: Make sure the [Long-Term Memory Engine (LTM-2.5) is enabled in PiecesOS](/products/core-dependencies/pieces-os/quick-menu#ltm-2-engine), as this engine aggregates context necessary for Cursor to retrieve accurate results.

3. **Use Agent Mode in Chat**: Cursor must be in *Agent*, not *Ask*, to access the `ask_pieces_ltm` tool. Switch to Agent to enable full MCP integration. Make sure *not to add* the `ask_pieces_ltm` tool as context—instead, rely solely on the *Agent* chat mode.

4. **Single MCP Instance:** Make sure that you aren’t testing multiple instances of the Pieces MCP server in different IDEs. This cross-contamination conflict with the SSE and several MCP instances running on the same port can cause issues in different development environments.

5. **Check MCP Server Status**: If you’re encountering messages such as “Sorry, I can’t do this,” your MCP server may not be properly configured or running.

6. **Go to** `settings.json` **in Visual Studio Code:** Confirm the MCP server status shows "running" (it may say "start" or "pause" otherwise). Restart the server if necessary and inspect terminal outputs for error messages.

7. **Review Configuration Details**: Double-check the MCP endpoint URL and the port number in your VS Code MCP configuration menu to ensure accuracy. You can find the current SSE endpoint URL in the Pieces Desktop App under **Settings** → **Model Context Protocol (MCP)**, or in the PiecesOS Quick Menu. It is usually formatted as:

```scss
http://localhost:{port_number}/model_context_protocol/{version}/sse
```

***

You're now ready to improve your workflow with powerful context retrieval using Pieces MCP, seamlessly integrated into Visual Studio Code with GitHub Copilot. Happy coding!