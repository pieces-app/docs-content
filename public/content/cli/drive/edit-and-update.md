---
title: Edit & Update
path: /cli/drive/edit-and-update
visibility: PUBLIC
status: PUBLISHED
---

## Editing

Keeping an up-to-date library of code snippets in the Pieces CLI is easy with seamless editing.

## How to Edit Snippets

Follow the steps below to edit a saved material in the Pieces CLI.

<Steps>
  <Step title="Open a Terminal">
    Opening a terminal on your device depends on your platform: Open your OS’ search bar and enter `terminal`(macOS/Linux) or `CMD`(Windows).
  </Step>

  <Step title="Open the Pieces Drive">
    Launch the Pieces CLI by typing `pieces run` in your terminal.

    Access your saved snippets with the `list` command.

    Use your mouse wheel or arrow keys to scroll and select a snippet by pressing `return` (macOS) or `enter` (Windows/Linux).
  </Step>

  <Step title="Enter Modify Command">
    After selecting your desired snippet, enter the `modify` command. This will open your selected snippet in your desired IDE.

    Any changes made and saved within your IDE will update the Pieces Drive automatically, allowing you to use the changed snippet immediately.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_drive/edit_update/editing_saving.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

## How to Rename Snippets

With the Pieces CLI, you can rename saved materials and have those changes apply universally throughout your Pieces Drive—follow the steps below to learn how.

<Steps>
  <Step title="Locate a Snippet">
    In your terminal, type `pieces run` to enter the Pieces CLI. This will switch you to Pieces CLI run mode, where you can type `list`.

    Use your mouse wheel or arrow keys to scroll and select a snippet by pressing `return` (macOS) or `enter` (Windows/Linux).
  </Step>

  <Step title="Enter the Edit Command">
    After selecting a snippet, you can type `edit`.

    This will open a new prompt for you to change the name and classification for the snippet.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_drive/edit_update/edit_command.png" alt="" align="center" fullwidth="true" />

    When you’re complete, the snippet will update across your Pieces Drive automatically.
  </Step>
</Steps>
