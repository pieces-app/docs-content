---
title: Editing
path: /extensions-plugins/visual-studio/drive/edit-update
visibility: PUBLIC
status: PUBLISHED
description: Keep your library of saved code snippets up-to-date easily with the seamless editing process between Visual Studio and the Pieces for Visual Studio Extension.
metaTitle: How to Manage Code Snippets in Visual Studio with Pieces Drive
metaDescription: Keep your saved code snippets up to date in Visual Studio with the Pieces Drive editing and modification tools.
---

## How to Edit Snippets

To modify code you’ve saved to your personal repository, you can use the Pieces Drive view in Visual Studio.

If you don’t have it open, use the command palette shortcut `ctrl+shift+p` and type Pieces Drive, then click it or press `enter` to open the view.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/using_snippets/edit_update/opening_pieces_drive_via_command_palette.gif" alt="" align="center" fullwidth="true" />

<Steps>
  <Step title="Locating a Snippet">
    Inside the Pieces Drive view, you can select the snippet you want to edit from the scrollable list of saved materials, or use the **Search Bar** to enter a query and locate your desired snippet.
  </Step>

  <Step title="Open the Snippet">
    To start editing the material saved from your repository, click the **Pencil Icon**. Hovering over this icon reveals an `Edit Selected Material` + `ctrl+e` tooltip.
  </Step>

  <Step title="Edit the Snippet">
    Once you click the **Pencil Icon,** your saved code will open in a new tab and automatically be redirected to that tab. Make your changes as needed.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/using_snippets/edit_update/edit_and_insert_snippet.gif" alt="" align="center" fullwidth="true" />
  </Step>

  <Step title="Save the Snippet">
    After making the desired changes to the code snippet, use `ctrl+s` to save the snippet, after which you will be returned to your active file.

    You’ll see a success message at the top of the active file indicating your changes have been made successfully.
  </Step>
</Steps>

### Material Management Actions

From within the Pieces Drive view, you can click the **three vertical dots** to review a `Quick Actions` tab that shows available metadata that you can view or directly adjust for that snippet.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/using_snippets/edit_update/editing_snippet_metadata.gif" alt="" align="center" fullwidth="true" />

You can view the table below for a comprehensive list of available actions.

***

| `Reclassify`            | Set your custom snippet classification.                                                                                                 |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| `Rename`                | Change the name (title) of the material as it appears in your Pieces Drive.                                                             |
| `Duplicate`             | Create a duplicate of the saved material—unmodified or modified to be more performant, readable, as a template, or in another language. |
| `Related Links`         | View, add, or remove related resources that provide additional context to the snippet.                                                  |
| `Tags`                  | Add or remove tags to the snippet’s metadata.                                                                                           |
| `Shareable Link`        | Generate or copy a shareable link for the saved material.                                                                               |
| `Annotations`           | View or edit the automatically generated description for that saved code.                                                               |
| `Anchors`               | Add associated files and directories to the material.                                                                                   |
| `Related People`        | Manage related code authors or coworkers.                                                                                               |
| `Sensitive Information` | Manually add or remove a sensitive information tag to the snippet, if not automatically generated.                                      |
| `Delete Piece`          | Remove this saved material from Pieces Drive.                                                                                           |

***

## Additional Tools while Editing

When you edit a saved snippet, you are opening a new file in Visual Studio to make those edits, which means that other Pieces functionalities, like functionalities provided by Pieces Copilot and Pieces Drive, are entirely available to you.

For example, when editing a snippet, right-clicking selected code will present you with the same toolbar and Pieces-related options (like `Save Current Selection to Pieces` or `Share Current Selection`).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/using_snippets/edit_update/showing_actions_in_edit_view.gif" alt="" align="center" fullwidth="true" />

This makes it easy to modify your saved code with the power that the Pieces for Visual Studio Extension gives you.