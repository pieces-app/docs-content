---
title: Editing
path: /extensions-plugins/jetbrains/drive/edit-update
visibility: PUBLIC
status: PUBLISHED
description: Editing snippets and saving your changes is simple with the Pieces for JetBrains Plugin.
metaTitle: Editing & Managing Saved Snippets in JetBrains with Pieces Drive
metaDescription: Edit and update your saved code snippets easily in Pieces for JetBrains to maintain an up-to-date and organized library.
---

## How to Edit Snippets

You can edit several types of metadata when editing saved materials, as well as the saved piece of code itself.

To edit a snippet:

<Steps>
  <Step title="Open the Pieces Drive">
    Open the Pieces Drive via the JetBrains sidebar.
  </Step>

  <Step title="Start Editing the Snippet">
    Locate a snippet you want to edit and select `Edit` from the quick menu, or right-click the snippet and choose `Edit` from the menu.
  </Step>

  <Step title="Edit your Snippet">
    Make changes, then save using `⌘+s` (macOS) or `ctrl+s` (Windows/Linux).

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/using_snippets/edit_and_update/editing_snippet.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

<Callout type="tip">
  After saving, the editor will automatically return to the main snippet view, with your changes applied instantly.
</Callout>

## Actions from the Pieces Drive View

A tool menu with Pieces features will appear when you left-click on a saved snippet in the Pieces Drive. Some options relate to the [Pieces Copilot](/products/extensions-plugins/jetbrains/copilot), while others handle [material management](/products/extensions-plugins/jetbrains/drive) actions.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/using_snippets/edit_and_update/edit_selected_material.png" alt="" align="center" fullwidth="true" />

### Pieces Copilot Actions

To access the material management view, choose a snippet from Pieces Drive. You can select various Copilot-focused actions from here, as listed in the table below.

***

| `Add to Copilot Context` | Adds the snippet to the context of your existing Copilot Chat conversation.                                                 |
| ------------------------ | --------------------------------------------------------------------------------------------------------------------------- |
| `Ask Copilot`            | This triggers the input modal, which lets you type a prompt directly into the field without changing your active file view. |
| `Insert at Cursor`       | Inserts the code snippet at the point of your cursor inside your active file.                                               |
| `Shareable Links`        | Shows shareable links that have been generated for that snippet, if applicable.                                             |

***

### Material Management Actions

Below the Pieces Copilot actions, you can quickly change a snippet's name, description, classification, and other enriched metadata. Check the table below for details.

***

| `Annotations`            | Add, adjust or delete annotations for the snippet.                                          |
| ------------------------ | ------------------------------------------------------------------------------------------- |
| `Related Links`          | Add or remove links to the snippet’s metadata.                                              |
| `Tags`                   | Add or remove tags to the snippet’s metadata.                                               |
| `Reclassify`             | Set your custom snippet classification.                                                     |
| `Edit Selected Material` | Edit the content of the snippet.                                                            |
| `Rename`                 | Change the name (title) of the snippet as it appears in your repository of saved materials. |
| `Delete`                 | Delete the snippet.                                                                         |

***

## Additional Tools while Editing

*Layers upon layers of functionality*—that's the aim of all Pieces plugins and extensions.

When you edit a snippet (find it in the Pieces Drive menu and click `Edit`), you can access all Pieces features, even though you're not in your main file view.

Instead, the `Edit` view *becomes* your main file, so you can [generate code comments, debug, add it to context, and more.](/products/extensions-plugins/jetbrains/copilot)