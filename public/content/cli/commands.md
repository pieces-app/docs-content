---
title: Commands
path: /cli/commands
visibility: PUBLIC
status: PUBLISHED
---

## Pieces CLI Commands

Reference for every command available in the Pieces CLI, grouped by what you're trying to do.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/commands/pieces_help.png" alt="" align="center" fullwidth="true" />

> The `pieces help` menu listing every command and flag.

## Quick Reference

Run any command with the `pieces` prefix from a regular terminal (e.g., `pieces ask "..."`), or drop the prefix when you're inside `pieces run` loop mode. Type `pieces help` (or `help` inside loop mode) to view this list anytime.

| Command | Description |
| --- | --- |
| `run` | Start the CLI in loop mode |
| `list` | List materials in your Pieces Drive |
| `list apps` | List registered applications |
| `list models` | List configured AI models |
| `create` | Create a material from clipboard |
| `modify` | Update the current material's content |
| `edit` | Rename or reclassify the current material |
| `share` | Generate a shareable link for a material |
| `delete` | Delete the current material |
| `execute` | Run a saved bash material |
| `ask` | Send a question to Conversational Search |
| `search` | Fuzzy-search materials and chats |
| `chats` | List all past conversations |
| `chat` | Show or switch conversations |
| `config` | View or edit CLI configuration |
| `commit` | Commit to GitHub with an auto-generated message |
| `login` | Log in to your Pieces account |
| `logout` | Log out of your Pieces account |
| `open` | Open PiecesOS or its Applet |
| `clear` | Clear the terminal screen |
| `version` | Show installed CLI and PiecesOS versions |
| `help` | Display the help menu |
| `onboarding` | Walk through first-run setup |
| `feedback` | Send feedback to the Pieces team |
| `contribute` | Contribute to the CLI project |

## Materials

Manage saved code, text, and bash materials in your Pieces Drive.

<AccordionGroup>
  <Accordion title="list">
    List every material in your Pieces Drive (alias: `drive`).

    ```bash
    pieces list
    ```
  </Accordion>

  <Accordion title="list apps">
    List every application registered with PiecesOS.

    ```bash
    pieces list apps
    ```
  </Accordion>

  <Accordion title="create">
    Create a new material from whatever's currently on your clipboard.

    ```bash
    pieces create
    ```
  </Accordion>

  <Accordion title="modify">
    Replace the content of the most recently selected material.

    ```bash
    pieces modify
    ```
  </Accordion>

  <Accordion title="edit">
    Rename or change the classification of the most recently selected material.

    ```bash
    pieces edit
    ```
  </Accordion>

  <Accordion title="share">
    Generate a shareable URL for the most recently selected material. The CLI prints the URL and prompts you to open it in your browser.

    ```bash
    pieces share
    ```
  </Accordion>

  <Accordion title="delete">
    Delete the most recently selected material.

    ```bash
    pieces delete
    ```
  </Accordion>

  <Accordion title="execute">
    Run a saved bash material directly from the terminal.

    ```bash
    pieces execute
    ```
  </Accordion>
</AccordionGroup>

## AI & Search

Send questions to *Conversational Search*, search across your data, and pick which model responds.

<AccordionGroup>
  <Accordion title="ask">
    Send a question to *Conversational Search*. Append flags to attach context from your Drive or local files.

    ```bash
    pieces ask "How do I parse JSON in Python?"
    ```

    Optional flags:

    - `-m`, `--materials` — attach saved materials by index (e.g., `-m 1 2`)
    - `-f`, `--file` — attach files or folders by absolute or relative path

    ```bash
    pieces ask "Refactor this function" -f ./src/utils.py
    ```
  </Accordion>

  <Accordion title="search">
    Fuzzy-search materials and past chats.

    ```bash
    pieces search "auth middleware"
    ```

    Optional `--mode` flags:

    - `--mode ncs` — Neural Code Search (semantic)
    - `--mode fts` — Full-Text Search (literal)

    ```bash
    pieces search "auth middleware" --mode ncs
    ```
  </Accordion>

  <Accordion title="list models">
    Show every AI model configured for `ask`, and switch which one is active.

    ```bash
    pieces list models
    ```
  </Accordion>
</AccordionGroup>

## Conversations

Browse, switch between, and manage your *Conversational Search* threads.

<AccordionGroup>
  <Accordion title="chats">
    List every past conversation, numbered for quick switching.

    ```bash
    pieces chats
    ```
  </Accordion>

  <Accordion title="chat">
    Show messages in your current conversation, or switch to another by number.

    ```bash
    pieces chat
    pieces chat 3
    ```

    Conversation-management flags (use inside the active chat):

    - `-n` — start a new conversation
    - `-d` — delete the current conversation
    - `-r "<name>"` — rename the current conversation

    ```bash
    pieces chat -r "Project Ideas"
    ```
  </Accordion>
</AccordionGroup>

## Configuration

View and edit CLI settings, including which code editor opens your config file.

<AccordionGroup>
  <Accordion title="config">
    Print your current Pieces CLI configuration to the terminal.

    ```bash
    pieces config
    ```
  </Accordion>

  <Accordion title="config --editor">
    Open your config file in the editor of your choice (e.g., `vim`, `code`). Changes save immediately.

    ```bash
    pieces config --editor code
    ```
  </Accordion>
</AccordionGroup>

## Account & Git

Sign in to Pieces Cloud and commit code to GitHub with an auto-generated message.

<AccordionGroup>
  <Accordion title="login">
    Log in to your Pieces Cloud account.

    ```bash
    pieces login
    ```
  </Accordion>

  <Accordion title="logout">
    Log out of your Pieces Cloud account.

    ```bash
    pieces logout
    ```
  </Accordion>

  <Accordion title="commit">
    Commit staged changes to GitHub with an auto-generated commit message. Add `-p` or `--push` to push immediately after.

    ```bash
    pieces commit
    pieces commit --push
    ```
  </Accordion>
</AccordionGroup>

## Setup & System

Install the CLI, launch the loop, and access help, version, and feedback utilities.

<AccordionGroup>
  <Accordion title="install">
    Install the CLI with `pip` (or `conda`, if you prefer). Python must be set up correctly.

    ```bash
    pip install pieces-cli
    ```

    ```bash
    conda install pieces-cli
    ```
  </Accordion>

  <Accordion title="run">
    Start the CLI in loop mode—type commands and flags directly without the `pieces` prefix.

    ```bash
    pieces run
    ```
  </Accordion>

  <Accordion title="open">
    Launch PiecesOS or its helper Applet.

    ```bash
    pieces open
    ```
  </Accordion>

  <Accordion title="clear">
    Clear the terminal screen.

    ```bash
    pieces clear
    ```
  </Accordion>

  <Accordion title="version">
    Display installed versions of PiecesOS and the CLI.

    ```bash
    pieces version
    ```
  </Accordion>

  <Accordion title="help">
    Display the help menu—the same one shown at the top of this page.

    ```bash
    pieces help
    ```
  </Accordion>

  <Accordion title="onboarding">
    Walk through first-run setup interactively.

    ```bash
    pieces onboarding
    ```
  </Accordion>

  <Accordion title="feedback">
    Send feedback directly to the Pieces team.

    ```bash
    pieces feedback
    ```
  </Accordion>

  <Accordion title="contribute">
    Open the contribution flow for the open-source CLI project.

    ```bash
    pieces contribute
    ```
  </Accordion>
</AccordionGroup>

***

## Next Steps

Want to see these commands in context? Read about [Conversational Search](/products/cli/copilot) for `ask`, `search`, and `chat`, [Pieces Drive](/products/cli/drive) for material commands, or the full [Configuration](/products/cli/configuration) walkthrough.
