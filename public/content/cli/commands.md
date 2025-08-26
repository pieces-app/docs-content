---
title: Commands
path: /cli/commands
visibility: PUBLIC
status: PUBLISHED
---

## Pieces CLI Commands

Below is a table containing all the commands available for use in the Pieces CLI.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/commands/pieces_help.png" alt="" align="center" fullwidth="true" />

### Command Table

You can easily access these commands through the **help menu** using the command `help` within the Pieces CLI. If you’re not within the Pieces CLI, you can use `pieces help`.

When you’re within the terminal and use the `pieces run` command, you don’t have to prefix the commands with “pieces”.

## Individual Commands

### run

Start the CLI in loop mode—you only need to type flags or commands.

```bash
run
```

### list

List all materials in your Pieces Drive (alias: drive).

```bash
list
```

### list apps

List all registered applications.

```bash
list apps
```

### list models

List available AI models and switch which one ask uses.

```bash
list models
```

### create

Create a new material from whatever’s on your clipboard.

```bash
create
```

### modify

Update the content of the current material.

```bash
modify
```

### edit

Change the name or classification of the current material.

```bash
edit
```

### share

To share a snippet, enter the `pieces share` command. After the snippet has been shared, its URL will appear within the terminal, and the CLI will prompt you to open the snippet in a browser.

```bash
share
```

### delete

Delete the current (or most recent) material.

```bash
delete
```

### execute

Run a Pieces bash material.

```bash
execute
```

### clear

Clear the terminal screen.

```bash
clear
```

### config

Show your current Pieces CLI configuration.

```bash
config
```

### config –editor \<editor\_name>

Set your preferred code editor (e.g., vim, code).

```bash
config -editor ...
```

### install

Type `pip install pieces-cli`, or if you prefer to use Conda, type `conda install pieces-cli`.

```bash
pip install pieces-cli
```

As long as Python is set up correctly, Pieces CLI will install.

```bash
conda install pieces-cli
```

### open

Open PiecesOS or its helper Applet.

```bash
open
```

### ask \<your\_question\_here>

Send a question to Pieces Copilot.

```bash
ask ...
```

### -m, –materials

Attach saved items by index (e.g., -m 1 2).

```bash
-m ...
```

```bash
-materials ...
```

### -f, –file 

Attach files or folders (absolute or relative paths).

```bash
-f ...
```

```bash
-file ...
```

### chats

List all your past conversations.

```bash
chats
```

### chat

Show messages in your current conversation.

```bash
chat
```

### chat  \<number>

Switch to and display a specific conversation by its number.

```bash
chat ...
```

### -n

Start a new conversation.

```bash
-n
```

### -d

Delete the conversation you’re currently in.

```bash
-d
```

### -r 

Rename your current conversation (e.g., -r “Project Ideas”).

```bash
-r ...
```

### search 

Fuzzy-search your materials and chats.

```bash
search ...
```

### –mode ncs

Use Neural Code Search for your query.

```bash
-mode ncs
```

### –mode fts

Use Full-Text Search for your query.

```bash
-mode fts
```

### commit

Commit changes to GitHub and auto-generate the message; add `-p` or `–push` to push immediately.

```bash
commit ...
```

### login

Log in to your Pieces Cloud account.

```bash
login
```

### logout

Log out of your Pieces Cloud account.

```bash
logout
```

### version

Show versions of PiecesOS and the CLI tool.

```bash
version
```

### help

Display the help message.

```bash
help
```

### onboarding

Walk through the initial setup process.

```bash
onboarding
```

### feedback

Send feedback directly to the Pieces team.

```bash
feedback
```

### contribute

Contribute code or ideas to the CLI project.

```bash
contribute
```
