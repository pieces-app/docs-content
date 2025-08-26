---
title: Generative AI Conversations
path: /cli/copilot/chat
visibility: PUBLIC
status: PUBLISHED
---

## Accessing Copilot Chat in your Terminal

There are two ways to manage your Copilot chats in the Pieces CLI.

### Starting a New Copilot Chat

To quickly start a conversation with Pieces Copilot:

<Steps>
  <Step title="Open a Terminal">
    Opening a terminal on your device depends on your platform: Open your OS’ search bar and enter `terminal` (macOS/Linux) or `CMD` (Windows).
  </Step>

  <Step title="Enter Ask Command">
    You can launch Pieces CLI by typing `pieces run`., Then, you can type `ask query`, where `query` is your question.

    If you’re not in Pieces CLI, in your terminal, you can type `pieces ask query`, replacing `query` with your question.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_copilot/chat/ask_pieces.gif" alt="" align="center" fullwidth="true" />
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

    Pieces Copilot will load material #4 as context.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_copilot/chat/pieces_context_chat.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

### via File Path

Use a folder of specific file as context for Pieces Copilot by initiating the conversation at a specified path.

<Steps>
  <Step title="Select Your File or Folder">
    Decide which file (or directory) you want Copilot to reference.
  </Step>

  <Step title="Open a Terminal">
    Opening a terminal on your device depends on your platform: Open your OS’ search bar and enter `terminal`(macOS/Linux) or `CMD`(Windows).
  </Step>

  <Step title="Ask with a File">
    Use the `-f` flag and the path, `pieces ask "How does this component render?" -f src/components/Button.jsx`.

    Pieces Copilot will read that file before answering.
  </Step>

  <Step title="Provide Multiple Contexts">
    Mix flags to supply more than one source `pieces ask "Compare this code to the design spec" -m 2 -f design/specs.md`.

    Copilot loads material #2 and `specs.md` before generating its response.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_copilot/chat/adding_file.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

## Pieces MCP

The Pieces MCP offers several useful commands within the Pieces CLI, from setting up the MCP to learning more about it. Discover the different commands:

### Setup

Automatically sets up MCP for VS Code, Goose, or Cursor.

<Steps>
  <Step title="Enter MCP Command">
    Within the Pieces CLI, enter `mcp setup` this will open up a new MCP setup menu.
  </Step>

  <Step title="Select MCP Platform">
    In the new window, select one of the three options that appear:

    * VS Code

    * Goose

    * Cursor

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_copilot/chat/selecting_mcp_option.png" alt="" align="center" fullwidth="true" />

    After selecting the environment you plan to set up Pieces MCP with, you’ll be prompted with the next set of questions.
  </Step>

  <Step title="Select Workspace">
    The new menu will have you select a workspace:

    * `User Settings` — Make the MCP available in any project you work on within VS Code.

    * `Workspace Settings` — Save the MCP locally to the current project you’re working on.

    When you select the workspace you want to set up, Pieces CLI will automatically add the configuration for you and guide you through using Pieces MCP within the platform you chose.
  </Step>
</Steps>

### List

The `mcp list` command displays the current implementations of Pieces MCP on your development platforms.

Currently, the Pieces CLI supports integration with [GitHub Copilot](/products/mcp/github-copilot), [Goose](/products/mcp/goose), and [Cursor](/products/mcp/cursor).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_copilot/chat/mcp_list.png" alt="" align="center" fullwidth="true" />

### Docs

The `mcp docs` command displays all of the [mcp documentation](/products/mcp/get-started) correlated with the supported development environments with the Pieces CLI and Pieces MCP.

### Repair

The `mcp repair` command checks how the Pieces MCP is set up in the platforms supported by Pieces CLI.

If it finds any issues, it will automatically fix them and ask you to type `y` for yes or `n` for no. Then, press `return` (macOS) or `enter` (Windows/Linux) to confirm your choice.

### Status

Running `mcp status` within the Pieces CLI will automatically check all implemented platforms to make sure the Pieces MCP implementation is running correctly.

If it finds that an implementation is broken, it will ask if you want to auto-repair the MCP server.

Type `y` for yes or `n` for no, and press `return` (macOS) or `enter` (Windows/Linux) to confirm your choice.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_copilot/chat/finish_setup_mcp.png" alt="" align="center" fullwidth="true" />

## Improving Code Consistency & Standardization

The Pieces Copilot enhances code quality by identifying inconsistencies and providing practical suggestions for standardization.

### Naming Inconsistencies

Suppose functions across your workspace use inconsistent naming patterns (e.g., `authenticateUser` in `authHandler.go` vs. `retrieveUserProfile` in `userHandler.go`).

In that case, Pieces Copilot can suggest adopting a standardized naming convention for better readability and maintainability, like this:

```c
func authenticateUser(ctx context.Context, credentials Credentials) (User, error) {
    if credentials.Username == "" || credentials.Password == "" {
        return User{}, errors.New("missing credentials")
    }
}
```

### Inconsistent Error Handling

If error-handling strategies differ across files (e.g., structured errors in `authService.go` vs. inconsistent handling in `userService.go`), Pieces Copilot can help unify the approach:

```c
func LoginUser(credentials Credentials) (string, error) {
    token, err := authenticate(credentials)
    if err != nil {
        return "", fmt.Errorf("login failed: %w", err)
    }
    return token, nil
}
```
