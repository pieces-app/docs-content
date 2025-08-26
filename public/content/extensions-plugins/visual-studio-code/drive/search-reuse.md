---
title: Search & Reuse
path: /extensions-plugins/visual-studio-code/drive/search-reuse
visibility: PUBLIC
status: PUBLISHED
description: The Pieces for VS Code Extension makes finding saved snippets quick and seamless, helping you stay productive without breaking your workflow.
metaTitle: How to Search & Retrieve Code Snippets in VS Code with Pieces Drive
metaDescription: Quickly find saved code snippets with the Pieces for VS Code Extension, ensuring seamless search and productivity without workflow disruptions.
---

## Locate Materials in Pieces Drive

To locate your snippets, open a file in VS Code and use one of two methods—searching with the Pieces Drive menu, or with keyboard shortcuts.

## How to Search for Saved Materials

You can search for snippets of code and other materials saved to your Pieces Drive right from within the editor. You can also apply search filters to help narrow down results.

### via Pieces Drive

If you want to access your saved snippets directly within the VS Code editor, you can:

<Steps>
  <Step title="Locate Pieces Drive">
    Open the `Pieces Drive` from the VS Code sidebar
  </Step>

  <Step title="Filter, Search, and Explore">
    Once the `Pieces Drive` is open, you have access to a wide range of options that allow you sort through your snippets

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/using_snippets/search_and_reuse/opening_a_snippet.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

### via Search Feature

You can also use `Pieces: Search Pieces` to find specific snippets—this is where you’ll **enter a specific query**, which is useful when you know exactly what you want:

<Steps>
  <Step title="Open the Command Palette">
    Open the **Command Palette** using `⌘+shift+p` (macOS) or `ctrl+shift+p` (Windows/Linux)
  </Step>

  <Step title="Enter the Command">
    Type `Pieces: Search Pieces`
  </Step>

  <Step title="Enter your Search Query">
    Enter your search query, **scrolling or using the arrow keys** to navigate the list
  </Step>

  <Step title="Choose your Desired Snippet">
    Press `return` (macOS) or `enter` (Windows/Linux) on your desired snippet to open it and it’s saved metadata in a new tab

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/using_snippets/search_and_reuse/search_snippets.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

<Callout type="tip">
  You can search with tags, descriptions, names, types, or even languages themselves to narrow down your search.
</Callout>

## Adding Filters to your Search

Saved Snippets being viewed in the Pieces Drive can be filtered down by snippet tags, coding languages, and snippet titles.

To filter through your snippets:

<Steps>
  <Step title="Open Pieces Drive">
    Open `Pieces Drive` via the VS Code sidebar
  </Step>

  <Step title="Select the Search Bar">
    Select the search bar at the top of the Pieces Drive
  </Step>

  <Step title="Choose the Filter Option">
    After clicking on the search bar, you’ll have the option to quick filter by `Titles`, `Annotations`, or `Content`
  </Step>

  <Step title="Enter your Query">
    Using the filter, enter a search query in the search bar

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/using_snippets/search_and_reuse/filtering_snippets.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

When you’ve finished entering your filters, the Pieces Explorer will only display the snippets that match your filters. You can clear this by clicking the siphon icon with an `x` over it.

<Callout type="tip">
  For any tags you don’t want to set, you can leave them blank by just pressing `return` (macOS) or `enter` (Windows/Linux).
</Callout>

## Viewing and Reusing Saved Snippets

<a target="_blank" href="/products/extensions-plugins/visual-studio-code/drive/save-snippets">Saved snippets</a> can be viewed alongside their saved metadata by opening up them up directly from the Pieces Drive or by clicking on them once they’ve been found using the `Pieces: Search Pieces` function from the dropdown list. You can also right click on the editor and select `Search Pieces` in the right-click options.

After opening a snippet, the **snippet in markdown preview mode** opens up in a separate window.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/using_snippets/search_and_reuse/opened_markdown_snippet.png" alt="" align="center" fullwidth="true" />

From this view, you can then highlight the code and right-click to copy the code to your clipboard, or use the `⌘+c` (macOS) or `ctrl+c` (Windows/Linux) shortcut.

### via Right-Click Menu

The Pieces for VS Code Extension provides a host of actions that appear once you right-click a snippet from within the Pieces Drive menu.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/using_snippets/search_and_reuse/right_click_menu_drive.png" alt="" align="center" fullwidth="true" />

There are a number of available material management and Pieces Copilot-related actions available on this menu, [which you can read more about here](/products/extensions-plugins/visual-studio-code/drive/edit-update#actions-from-the-editing-view)—or view an expanded table of them below.

### via Pieces Sidebar

You can view snippets by opening up the Pieces Drive sidebar in your VS Code by clicking the Pieces Drive icon on the left-hand side of your screen.

Once in the sidebar, you can insert a snippet and place it exactly where you want it in your code by clicking `Insert at `Cursor.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/using_snippets/search_and_reuse/insert_at_cursor.gif" alt="" align="center" fullwidth="true" />

You can also right-click a snippet and select `Copy` to copy it to the clipboard, allowing you to paste it anywhere you need.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/using_snippets/search_and_reuse/drive_copy_to_clipboard.png" alt="" align="center" fullwidth="true" />

### Previewing Saved Snippets

While using the `Pieces: Search Pieces` function, you can click on one of the snippets on the dropdown list to view it’s code before selecting the snippet.

***

| `Add to Copilot Context` | `Ask Copilot`     | `Copy`        |
| ------------------------ | ----------------- | ------------- |
| `Insert at Cursor`       | `Shareable Links` | `Annotations` |
| `Links`                  | `Tags`            | `Reclassify`  |
| `Edit`                   | `Rename`          | `Delete`      |

***

## Real-Time Snippet Streaming

Every product within the Pieces Suite utilizes <a target="_blank" href="/products/core-dependencies/pieces-os">PiecesOS</a> to gather information regarding the context of your snippets.

When you modify a snippet in the <a target="_blank" href="/products/desktop">Pieces for Developers Desktop App</a>—like changing its name or description, tags, or any other metadata—those updates are automatically shown in your Pieces Drive without the need for refreshing.

<Callout type="tip">
  If your snippets aren’t updating immediately, refer to the [troubleshooting guide](/products/extensions-plugins/visual-studio-code/troubleshooting) for instructions on how to refresh your snippet list.
</Callout>