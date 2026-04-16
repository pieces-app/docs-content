---
title: Generative AI Conversations
path: /cli/copilot/chat
visibility: PUBLIC
status: PUBLISHED
---

## Accessing Copilot Chat in your Terminal

There are two ways to manage your Copilot chats in the Pieces CLI.

### Starting a New Copilot Chat

To quickly start a conversation with Conversational Search:

<Steps>
  <Step title="Open a Terminal">
    Opening a terminal on your device depends on your platform: Open your OS’ search bar and enter `terminal` (macOS/Linux) or `CMD` (Windows).
  </Step>

  <Step title="Enter Ask Command">
    You can launch Pieces CLI by typing `pieces run`., Then, you can type `ask query`, where `query` is your question.

    If you’re not in Pieces CLI, in your terminal, you can type `pieces ask query`, replacing `query` with your question.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_copilot/chat/ask_pieces.gif" alt="Using the ask command in Pieces CLI" align="center" fullwidth="true" />
  </Step>
</Steps>

### Opening Previous Chats

To resume or explore an earlier conversation:

* `chats`: Show all your conversations. The one highlighted in green is where new questions go by default.

* `chat`: Display the messages in your current conversation.

* `chat <number>`: Switch to conversation `<number>` and show its messages.

Use these flags with your `chat` command to manage conversations as you go:

* `chat --new`, `chat -n`: Create a new conversation and switch to it.

* `chat --delete`, `chat -d`: Delete the conversation you’re currently viewing.

* `chat --rename [name]`, `chat -r [name]`: Rename the conversation you’re viewing. If you don’t provide `[name]`, the assistant will suggest one.

[Read more about what commands are available in the Pieces CLI](/products/cli/commands).

## Contextualized Chats

You can narrow Copilot’s focus by feeding it specific materials or files when you ask a question.

### via Material Index

<Steps>
  <Step title="Open a Terminal">
    Opening a terminal on your device depends on your platform: Open your OS’ search bar and enter `terminal`(macOS/Linux) or `CMD`(Windows).
  </Step>

  <Step title="List your materials">
    Run `pieces list` to view all saved materials and note the **index** of the one you need.
  </Step>

  <Step title="Ask with a Material">
    Use the `-m` flag and that index when you ask: `pieces ask "Explain the data model here" -m 4`

    Conversational Search will load material #4 as context.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_copilot/chat/pieces_context_chat.gif" alt="Providing material context to Copilot" align="center" fullwidth="true" />
  </Step>
</Steps>

### via File Path

Use a folder of specific file as context for Conversational Search by initiating the conversation at a specified path.

<Steps>
  <Step title="Select Your File or Folder">
    Decide which file (or directory) you want Copilot to reference.
  </Step>

  <Step title="Open a Terminal">
    Opening a terminal on your device depends on your platform: Open your OS’ search bar and enter `terminal`(macOS/Linux) or `CMD`(Windows).
  </Step>

  <Step title="Ask with a File">
    Use the `-f` flag and the path, `pieces ask "How does this component render?" -f src/components/Button.jsx`.

    Conversational Search will read that file before answering.
  </Step>

  <Step title="Provide Multiple Contexts">
    Mix flags to supply more than one source `pieces ask "Compare this code to the design spec" -m 2 -f design/specs.md`.

    Copilot loads material #2 and `specs.md` before generating its response.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_copilot/chat/adding_file.png" alt="Adding multiple contexts to chat query" align="center" fullwidth="true" />
  </Step>
</Steps>

## Pieces MCP

The Pieces CLI bridges MCP to your development tools—no manual config editing required. Run `pieces mcp setup` from your terminal to get started.

### Setup

Run `pieces mcp setup` from your terminal to open an interactive menu and automatically configure Pieces MCP for your platform.

<Steps>
  <Step title="Run the setup command">
    In your terminal, run `pieces mcp setup`.
  </Step>

  <Step title="Select your platform">
    Use the arrow keys to select your MCP client and press Enter. Supported platforms:

    * VS Code
    * Cursor
    * Claude Desktop
    * Windsurf
    * Claude Code
    * Raycast
    * Warp

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_copilot/chat/selecting_mcp_option.png" alt="MCP platform selection menu" align="center" fullwidth="true" />

  </Step>

  <Step title="Follow the prompts">
    The CLI writes the correct configuration for your platform. For VS Code, you'll be asked to choose *User Settings* (MCP available in all projects) or *Workspace Settings* (MCP for the current project only). Other platforms use global config files.
  </Step>
</Steps>

<Callout type="tip">
  Ensure PiecesOS is running and LTM is enabled. Run `pieces mcp status` to verify your setup.
</Callout>

### List

The `mcp list` command displays the current implementations of Pieces MCP on your development platforms.

The Pieces CLI supports integration with [VS Code](/products/mcp/vs-code), [Cursor](/products/mcp/cursor), [Claude Desktop](/products/mcp/claude-desktop), [Windsurf](/products/mcp/windsurf), [Claude Code](/products/mcp/claude-code), [Raycast](/products/mcp/raycast), Warp, [GitHub Copilot](/products/mcp/github-copilot), and [Goose](/products/mcp/goose).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_copilot/chat/mcp_list.png" alt="MCP implementations list" align="center" fullwidth="true" />

### Docs

The `mcp docs` command displays all of the [mcp documentation](/products/mcp) correlated with the supported development environments with the Pieces CLI and Pieces MCP.

### Repair

The `mcp repair` command checks how the Pieces MCP is set up in the platforms supported by Pieces CLI.

If it finds any issues, it will automatically fix them and ask you to type `y` for yes or `n` for no. Then, press `return` (macOS) or `enter` (Windows/Linux) to confirm your choice.

### Status

Running `mcp status` within the Pieces CLI will automatically check all implemented platforms to make sure the Pieces MCP implementation is running correctly.

If it finds that an implementation is broken, it will ask if you want to auto-repair the MCP server.

Type `y` for yes or `n` for no, and press `return` (macOS) or `enter` (Windows/Linux) to confirm your choice.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_copilot/chat/finish_setup_mcp.png" alt="MCP setup completion confirmation" align="center" fullwidth="true" />

