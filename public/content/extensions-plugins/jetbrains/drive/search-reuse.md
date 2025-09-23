---
title: Searching
path: /extensions-plugins/jetbrains/drive/search-reuse
visibility: PUBLIC
status: PUBLISHED
description: You can find your saved code snippets easily with the Pieces for JetBrains Plugin by utilizing a few different search methods.
metaTitle: Searching & Reusing Code Snippets in JetBrains with Pieces Drive
metaDescription: Quickly search and reuse your saved code snippets in Pieces for JetBrains, ensuring seamless productivity without breaking your workflow.
---

## Finding Saved Snippets

To locate your snippets, open a file in VS Code and use one of two methods: searching with the **Pieces Drive** menu or with **Search Everywhere**.

### via Pieces Drive

If you want to access your saved snippets directly within the JetBrains IDE, you can:

<Steps>
  <Step title="Locate Pieces Drive">
    Open the `Pieces Drive` from the JetBrains sidebar.
  </Step>

  <Step title="Filter, Search, and Explore">
    Once the `Pieces Drive` is open, you have access to a wide range of options that allow you sort through your snippets.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/using_snippets/search_and_reuse/searching_snippets_drive.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

### via Search Everywhere

Whether you’re on macOS, Windows or Linux, you must double-press the `Shift` key twice to open up the Search Everywhere menu.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair_2/via_search_everywhere.png" alt="" align="center" fullwidth="true" />

Once the menu is open, switch to the `Pieces` tab, then enter a search query to search your entire Pieces repository for any snippet you’ve saved.

After you’ve located a snippet, you can press `Enter` to open it in a new window and view the snippet’s code and saved context.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/using_snippets/search_and_reuse/searching_for_snippet.gif" alt="" align="center" fullwidth="true" />

You can also press `shift+shift` again and search while remaining in the Search Everywhere menu’s `All` tab, but the `Pieces` tab is the de facto home for seeing only saved snippet search results.

<Callout type="info">
  The default behavior for the **Search Everywhere** feature can be changed to whatever keymapping you prefer—l<a target="_blank" href="/products/extensions-plugins/jetbrains/commands">earn more about this here.</a>
</Callout>

## Adding Filters to your Search

You can filter saved snippets in the Pieces Drive using snippet tags, coding languages, and titles.

To filter through your snippets:

<Steps>
  <Step title="Open Pieces Drive">
    Open `Pieces Drive` via the JetBrains Sidebar.
  </Step>

  <Step title="Select the Search Bar">
    Select the search bar at the top of the Pieces Drive.
  </Step>

  <Step title="Choose the Filter Option">
    After clicking on the search bar, you’ll have the option to quickly filter by `Titles`, `Annotations`, or `Content`.
  </Step>

  <Step title="Enter your Query">
    Using the filter, enter a search query in the search bar.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/using_snippets/search_and_reuse/filtering_snippets.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

When you’ve finished entering your filters, the Pieces Explorer will only display the snippets that match your filters. You can clear this by clicking the siphon icon with an `x` over it.

<Callout type="tip">
  For any tags you don’t want to set, you can leave them blank by just pressing `return` (macOS) or `enter` (Windows/Linux).
</Callout>

## Viewing and Reusing Saved Snippets

[Saved snippets](/products/extensions-plugins/jetbrains/drive/save-snippets) can be viewed alongside their saved metadata by opening up them up directly from the Pieces Drive—either by pressing `enter` on a highlighted snippet, or by double-clicking it.

This opens up the **snippet in markdown preview mode** in a separate window.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair_2/viewing_and_reusing.png" alt="" align="center" fullwidth="true" />

From the opened markdown preview, you can then select `Copy to Clipboard` in the top-left corner of the snippet’s embedded code box or use the `⌘+c` (macOS) or `ctrl+c` (Windows/Linux) shortcut after selecting the section.

### via Right-Click Menu

The Pieces for JetBrains Plugin offers several actions when you right-click a snippet in the Pieces Drive menu.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/using_snippets/search_and_reuse/pieces_drive_right_click.png" alt="" align="center" fullwidth="true" />

This menu offers several material management and Pieces Copilot-related actions. [Read more about them here](/products/extensions-plugins/jetbrains/drive/edit-update#actions-from-the-editing-view) or see the expanded table below.

### via Pieces Sidebar

You can view snippets by opening up the Pieces sidebar in your JetBrains IDE and clicking the `Pieces Drive Icon` on the left-hand side of your screen.

Once in the sidebar, you can insert a snippet and place it exactly where you want it in your code by clicking `Insert at Cursor`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/using_snippets/search_and_reuse/copy_to_clipboard_drive.png" alt="" align="center" fullwidth="true" />

You can also right-click a snippet and select `Copy` to copy it to the clipboard, allowing you to paste it anywhere you need.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/using_snippets/search_and_reuse/copy_to_clipboard_drive.png" alt="" align="center" fullwidth="true" />

### Previewing Saved Snippets

While using the Pieces Drive sidebar, you can click on one of the snippets in the snippets list to view its code before selecting the snippet.

***

| `Add to Copilot Context` | `Ask Copilot`     | `Copy`        |
| ------------------------ | ----------------- | ------------- |
| `Insert at Cursor`       | `Shareable Links` | `Annotations` |
| `Links`                  | `Tags`            | `Reclassify`  |
| `Edit`                   | `Rename`          | `Delete`      |

***

## Real Time Snippet Streaming[​](/products/extensions-plugins/jetbrains#real-time-snippet-streaming)

Each product in the Pieces Suite uses [PiecesOS](/products/core-dependencies/pieces-os) to get information about your snippets' context.

When you update a snippet in the [Pieces Desktop App](/products/desktop)—such as a name or description, tags or any of the other metadata—those changes are also reflected in your Pieces Drive without refreshing.

<Callout type="tip">
  If your snippets are not updating right away, see the [troubleshooting guide](/products/extensions-plugins/jetbrains/troubleshooting) to details on how to refresh your snippet list.
</Callout>
