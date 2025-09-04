---
title: Edit & Update
path: /extensions-plugins/visual-studio-code/drive/edit-update
visibility: PUBLIC
status: PUBLISHED
description: Edit, update, and reuse saved code that's stored in your Pieces Drive for use within your Visual Studio Code project.
metaTitle: How to Modify & Manage Code Snippets in VS Code with Pieces Drive
metaDescription: Easily edit and update your code snippets in the Pieces for VS Code Extension, keeping your library organized and up to date.
---

## Editing

Maintaining an up-to-date library of code snippets in the <a target="_blank" href="https://marketplace.visualstudio.com/items?itemName=MeshIntelligentTechnologiesInc.pieces-vscode">Pieces for VS Code Extension</a> is made easy through seamless editing.

## How to Edit Snippets

To modify an existing snippet, follow these steps:

<Steps>
  <Step title="Open the Pieces Drive">
    Open the Pieces Drive via the VS Code sidebar
  </Step>

  <Step title="Start Editing the Snippet">
    Locate a snippet you want to edit and select `Edit` from the quick menu or right click the snippet and select `Edit` from the menu
  </Step>

  <Step title="Edit your Snippet">
    Make your changes, then save using `⌘+s` (macOS) or `ctrl+s` (Windows/Linux)

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/using_snippets/edit_and_update/editing_snippet.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

<Callout type="tip">
  After saving, the editor will automatically return to the main snippet view, with your changes applied instantly.
</Callout>

## Actions from the Pieces Drive View

When you left-click on a saved snippet in the Pieces Drive, you are presented with a tool menu filled with Pieces functionalities—some of which are related to the [Pieces Copilot](/products/extensions-plugins/visual-studio-code/copilot), and others which are designated [material management](/products/extensions-plugins/visual-studio-code/drive) actions.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/using_snippets/search_and_reuse/right_click_options_from_drive.png" alt="" align="center" fullwidth="true" />

### Pieces Copilot Actions

To access the material management view, select one of the snippets from Pieces Drive. From this view, you can select a number of Copilot-centric actions—view them in the table below.

***

| `Add to Copilot Context` | Adds the snippet to the context of your existing Copilot Chat conversation.                                         |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------- |
| `Ask Copilot`            | Triggers the input modal and lets you type a prompt directly into the field without changing your active file view. |
| `Insert at Cursor`       | Inserts the code snippet at the point of your cursor inside your active file.                                       |
| `Shareable Links`        | Shows shareable links that have been generated for that snippet, if applicable.                                     |

***

### Material Management Actions

Below the Pieces Copilot actions, you can easily change a snippet’s name, description, classification, and other enriched metadata—view them in the table below.

***

| `Annotations`            | Add, adjust or delete annotations for the snippet.                                          |
| ------------------------ | ------------------------------------------------------------------------------------------- |
| `Related Links`          | Add or remove links to the snippet’s metadata.                                              |
| `Tags`                   | Add or remove tags to the snippet’s metadata.                                               |
| `Reclassify`             | Set your own custom snippet classification.                                                 |
| `Edit Selected Material` | Edit the content of the snippet.                                                            |
| `Rename`                 | Change the name (title) of the snippet as it appears in your repository of saved materials. |
| `Delete`                 | Delete the snippet.                                                                         |

***

## Additional Tools while Editing

*Layers upon layers of functionality*—that’s the goal of all Pieces plugins and extensions.

When you edit a snippet (by locating it in the Pieces Drive menu and clicking `Edit`), every single bit of Pieces functionality is available to you, even though you are in a view that’s removed from your main file.

Instead, the `Edit` view *becomes* your main file, so you can [generate code comments, debug, add it to context, and more.](/products/extensions-plugins/visual-studio-code/copilot)

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/using_snippets/edit_and_update/comments_inside_editing_snippet_view.gif" alt="" align="center" fullwidth="true" />