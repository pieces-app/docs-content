---
title: Pieces MCP + Goose Integration
path: /mcp/goose
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with Goose lets you use Pieces Long-Term Memory directly through the Goose CLI, enhancing your coding workflow with deep contextual awareness.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with Goose
metaDescription: Discover how to integrate Pieces Model Context Protocol (MCP) with Goose. Access Long-Term Memory within your IDE for enhanced, context-aware productivity.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/MCP/goose_mcp.png"
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/goose_mcp/mcp_goose.png" alt="" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp/get-started) with Goose is a powerful way to bring your daily workflow context directly into your command line or desktop interface.

With this integration, you'll have a *command-line AI assistant* that knows more about your coding activities than just the current project.

You can ask Pieces about bug fixes in your code discussed in your team channel, inquire about similar code you've worked on, or prompt it to double-check that your new code meets the criteria your coworker suggested—and much more.

Learn how to integrate the Pieces MCP into Goose by following the steps below.

## Prerequisites

There are **\[2]** primary prerequisites for integrating Pieces with Goose as an MCP—an active instance of **PiecesOS** and the fully-enabled **Long-Term Memory (LTM-2.7)** engine.

<Steps>
  <Step title="Install & Run PiecesOS">
    Make sure that PiecesOS is installed and running. This is *required* for the MCP server to communicate with your personal repository of workflow data and pass context through to the Goose interface.
  </Step>

  <Step title="Enable Long-Term Memory">
    For the MCP server to interact with your workflow context, you must enable the Long-Term Memory Engine (LTM-2.7) through the Pieces Desktop App or the [PiecesOS Quick Menu](/products/core-dependencies/pieces-os/quick-menu) in your toolbar.
  </Step>

  <Step title="Install Goose">
    If you haven't installed Goose yet, follow the <a target="_blank" href="https://block.github.io/goose/docs/getting-started/installation/">installation instructions</a>.
  </Step>
</Steps>

### Installing PiecesOS & Configuring Permissions

Follow the detailed set-up instructions below for a detailed guide on setting up and configuring PiecesOS to correctly pass captured workflow context to the Pieces MCP server.

<pos-download-guide />

### SSE Endpoint

To use Pieces MCP with Goose, you'll need the Server-Sent Events (SSE) endpoint from PiecesOS:

```scss
http://localhost:39300/model_context_protocol/2024-11-05/sse
```

<Callout type="alert">
  Keep in mind that the **specific port** (i.e., `39300`) PiecesOS is running on **may vary**.
</Callout>

To find the up-to-date SSE endpoint with the active instance of POS (including the current port number), open the PiecesOS Quick Menu and expand the **Model Context Protocol (MCP) Servers** tab.

There, you can copy the SSE endpoint with one click, which includes the active PiecesOS port number.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_pos_new.png" alt="" align="center" fullwidth="true" />

You can also find this in the Pieces Desktop App by opening the [Settings](/products/desktop/configuration) view and clicking **Model Context Protocol (MCP)**.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_pfd_new.png" alt="" align="center" fullwidth="true" />

## Setting Up Goose with Pieces MCP

Follow the steps below to set up Pieces MCP with Goose, either through the command line or desktop application.

Make sure you have the latest version of Goose installed to ensure compatibility with Pieces MCP.

<Callout type="alert">
  You will need to go through additional set-up steps (such as setting up your LLM provider) which involves setting up your host, choosing your model, using your API key, and more.

  Read the <a target="_blank" href="https://block.github.io/goose/docs/getting-started/installation/">official, open-source documentation</a> on completing these set-up steps.
</Callout>

### via CLI

Setting up the Pieces MCP through the Goose Command Line Interface is straightforward.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/goose_mcp/set_up_mcp_server.gif" alt="" align="center" fullwidth="true" />

<Steps>
  <Step title="Run the Configuration Command">
    Open your terminal (macOS/Linux) or CMD (Windows) and run:

    ```bash
    goose configure
    ```
  </Step>

  <Step title="Choose ‘Add Extension’">
    From the list of available options, choose `Add Extension`.
  </Step>

  <Step title="Choose ‘Remote Extension’">
    Select `Remote Extension` from the list of extension types.
  </Step>

  <Step title="Give it a Name">
    Name your extension `Pieces` or something similar.
  </Step>

  <Step title="Enter the SSE Endpoint URL">
    From PiecesOS, the Desktop App, or this documentation, obtain the Pieces MCP SSE endpoint URL and paste it into your terminal.

    ```bash
    http://localhost:39300/model_context_protocol/2024-11-05/sse
    ```

    <Callout type="tip">
      Adjust the port number if your local instance of PiecesOS runs on a different one.
    </Callout>
  </Step>

  <Step title="Set the Tool Timeout">
    You’ll be prompted to enter a value for timing out the tool in case of an error or repeated *hangtime*. The default value is `300`—you can enter that value, or another.
  </Step>

  <Step title="Optional Configurations">
    Lastly, you’ll be prompted to add a description or additional environment variables—these are not required. Select `No` to both if you want to proceed.
  </Step>

  <Step title="Success!">
    You’ll now see a message like `Added Pieces Extension` or similar, depending on the name you’ve attributed to the extension. You can use `goose list extensions` to verify and check the list of integrated extensions within Goose.
  </Step>
</Steps>

<Card title="For macOS Users:" image="/assets/icons/platform_logos/macos_logo.png">
  You may see an error message when configuring Goose, like:

  > <mark>Warning: Goose installed, but /Users/you/.local/bin is not in your PATH…</mark>

  You can fix this issue by adding `export PATH=”$HOME/.local/bin:$PATH”` to your your `~/.zshrc` or `~/.bashrc`.

  Then, reload with `source ~/.zshrc` and start a Goose session by using `goose` from anywhere.
</Card>

## Using Pieces MCP with Goose

Once the integration is set up, you can start using Pieces Long-Term Memory through Goose.

### Starting a Conversation

<Steps>
  <Step title="Open up a Goose Chat">
    Simply type `goose` in your terminal to start a new conversation:

    ```bash
    goose
    ```

    This will open a prompt where you can interact with Goose, which now has access to your Pieces Long-Term Memory.
  </Step>

  <Step title="Start Prompting">
    You can now start interacting with the Pieces MCP server.

    Try using this prompt:

    ```plaintext
    I need a status update for what I was working on yesterday. Create a report with 5 bullet points based off the most important activities, and give each one a brief description. Use time stamps to accurately report how long I spent working on group of tasks/topics.
    ```

    <Callout type="alert">
      This prompt is formulated for users already familiar with PiecesOS who use the Long-Term Memory Engine.\
      \
      If you are a first-time user, it is recommended that you launch PiecesOS and enable LTM, then allow some time for data capture before using this prompt for a desirable output.
    </Callout>

    Here’s a response using that exact same prompt inside of Goose using the Pieces MCP integration:

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/goose_mcp/example_convo_demo_prompt.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

<Card title="Hey!" image="/assets/icons/platform_logos/pieces_logo.png">
  Check out this [MCP-specific prompting guide](/products/mcp/prompting) if you want to effectively utilize the Long-Term Memory Engine (LTM-2.7) with your new Pieces MCP server.
</Card>

## Toggling & Removing Pieces MCP

To remove the Pieces MCP for Goose, you can follow the same process you otherwise would for removing any Goose extension.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/goose_mcp/remove_mcp_server.gif" alt="" align="center" fullwidth="true" />

<Steps>
  <Step title="Enter the Configuration Settings">
    Open up your terminal and type `goose configure`, then press `return` (macOS) or `enter` (Windows/Linux).
  </Step>

  <Step title="Extension Toggling">
    Use your keyboard’s **up** and **down** arrow keys to navigate down to `Toggle Extensions`.
  </Step>

  <Step title="Un-Toggle your Pieces MCP Server">
    Using arrow keys to navigate the list, press `space` (macOS/Windows/Linux) when the carrot is pointing towards your targeted extension.

    Then, press `return` (macOS) or `enter` (Windows/Linux) to confirm changes.
  </Step>

  <Step title="Re-enter the Configuration Settings">
    Use `goose configure` to re-enter the configuration menu.
  </Step>

  <Step title="Removing Extensions">
    Use your arrow keys to navigate to `Remove Extensions`, then, using the same `space` and `enter/return` process, first *toggle* then *confirm* your removal of the Pieces MCP extension.
  </Step>
</Steps>

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with Goose, follow these troubleshooting steps:

1. **Verify PiecesOS Status:** Ensure [PiecesOS is actively running](/products/core-dependencies/pieces-os) on your system. MCP integration requires PiecesOS to be operational.

2. **Confirm LTM Engine Activation:** Make sure the [Long-Term Memory Engine (LTM-2.7) is enabled in PiecesOS](/products/core-dependencies/pieces-os/quick-menu#ltm-2-engine), as this engine aggregates context necessary for Goose to retrieve accurate results.

3. **Single MCP Instance:** Make sure that you aren't testing multiple instances of the Pieces MCP server in different IDEs. This *cross-contamination conflict* with the SSE and several MCP instances running on the same port can cause issues in different development environments.

4. **Check MCP Server Status:** If you're encountering messages such as "Sorry, I can't do this," your MCP server may not be properly configured or running.

5. **Verify Port Configuration:** Double-check the MCP endpoint URL and the port number in your Goose configuration to ensure accuracy. You can find the current SSE endpoint URL in the Pieces Desktop App under **Settings → Model Context Protocol (MCP)**, or in the PiecesOS Quick Menu. It is usually formatted as:

```plaintext
http://localhost:{port_number}/model_context_protocol/{version}/sse
```

6. **Mac PATH Issues:** If you're having trouble with Goose CLI on macOS, try manually adding it to your PATH:

```bash
export PATH="$HOME/.local/bin:$PATH"
```

7. **Restart Services:** If problems persist, try restarting both PiecesOS and Goose, then reconfigure the extension with the current port number.

8. **Use the Correct Mode:** You can experience a blockage of LTM data if you are using *any other chat mode* than **Auto** mode. Make sure to use `goose configure` to change chat modes to avoid issues.

***

You're now set to enhance your workflow with powerful context retrieval through Pieces MCP integrated seamlessly into Goose. Happy coding!