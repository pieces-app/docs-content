---
title: Searching
path: /obsidian/drive/search-reuse
visibility: PUBLIC
status: PUBLISHED
description: The Pieces for Obsidian Plugin makes finding saved snippets quick and seamless, helping you stay productive without breaking your workflow.
metaTitle: How to Search & Retrieve Code Snippets in Obsidian with Pieces Drive
metaDescription: Easily search and reuse saved snippets in Pieces Drive for Obsidian, ensuring quick access to the right code at the right time.
---

## Finding Saved Materials

To locate your snippets, use the Pieces Sidebar menu.

### via Pieces Sidebar

To locate your snippets, use the Pieces Sidebar menu or the search feature:

<Steps>
  <Step title="Open the Pieces Sidebar">
    Open the Pieces plugin from the Obsidian sidebar.
  </Step>

  <Step title="Navigate to Saved Materials">
    Click on **Saved Materials** in the menu to display a list of your saved. materials
  </Step>

  <Step title="Open a Snippet">
    Click on your desired snippet to view its content, associated metadata, and quick actions.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/obsidian_plugin_assets/using_snippets/search_reuse/copy_paste_snippet_OBS.gif" alt="" align="center" fullwidth="true" />

### via Search Feature

If you know exactly what you’re looking for, you can search for specific snippets:

<Steps>
  <Step title="Click the Search Bar">
    Open the search bar at the top of the Pieces Sidebar.
  </Step>

  <Step title="Enter Your Query">
    Type in your search query.
  </Step>

  <Step title="Navigate the Results">
    Scroll through the results or use the arrow keys to find your desired snippet.
  </Step>

  <Step title="Open the Snippet">
    Click on the snippet to open it and view its content, associated metadata, and quick actions.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/obsidian_plugin_assets/using_snippets/search_reuse/search_process.gif" alt="" align="center" fullwidth="true" />

<Callout type="tip">
  To narrow down your search, you can use tags, descriptions, names, types, or even languages themselves.
</Callout>

## Adding Filters to Your Search

Saved snippets being viewed in the Pieces Drive Sidebar can be sorted and filtered to narrow down your search results.

### Filtering Snippets

<Steps>
  <Step title="Click the Search Bar">
    Click on the search bar at the top of the Pieces Drive Sidebar.
  </Step>

  <Step title="Use Quick Filters">
    Apply quick filters such as `Titles`, `Annotations`, or `Content` that appear below the search bar.
  </Step>

  <Step title="Filter by Tags or Keywords">
    Enter specific tags or keywords in the search bar to refine the displayed snippets.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/obsidian_plugin_assets/using_snippets/search_reuse/filtering_snippets.gif" alt="" align="center" fullwidth="true" />

### Sorting Snippets

<Steps>
  <Step title="Click the Sorting Icon">
    Click the icon at the top of the sidebar (e.g., clock icon for recent). The icon changes based on the selected sorting method.
  </Step>

  <Step title="Choose Sorting Order">
    Select your preferred sorting order, such as `Recent`, `Suggested`, `Alphabetical`, or `Language`.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/obsidian_plugin_assets/using_snippets/search_reuse/sorting_snippets.gif" alt="" align="center" fullwidth="true" />

## Viewing and Reusing Saved Snippets

[Saved snippets](/products/obsidian/drive/save-snippets) can be viewed alongside their saved metadata by opening them directly from the Pieces Sidebar and clicking on them in the Pieces Drive once they’ve been found.

From this view, you can use Quick Actions, copy the snippet, or insert it at the cursor in your editor. Click `Open Markdown Preview` to **see the snippet in markdown preview mode,** or click on the snippet for a quick overview.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/obsidian_plugin_assets/using_snippets/search_reuse/mardown_preview_mode_OBS.png" alt="" align="center" fullwidth="true" />

From this view, you can use the `Pieces Actions` button at the bottom of the snippet to copy it, edit it, update annotations, generate a shareable link, toggle the visibility of the Pieces Actions buttons, or highlight and right-click to copy, or use `⌘+c` (macOS) or `ctrl+c` (Windows/Linux) to copy to your clipboard.

### via Pieces Sidebar

You can view snippets by opening the Pieces Drive Sidebar in Obsidian by clicking the Pieces icon on the left-hand side of your screen.

Once in the sidebar, you can insert a snippet into your note by clicking the `Insert at Cursor` button.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/obsidian_plugin_assets/using_snippets/search_reuse/insert_at_cursor_copy_paste_snippet_OBS.gif" alt="" align="center" fullwidth="true" />

You can also right-click a snippet and select `Copy to Clipboard`, allowing you to paste it anywhere you need.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/obsidian_plugin_assets/using_snippets/search_reuse/copy_to_clipboard_OBS.png" alt="" align="center" fullwidth="true" />

### Previewing Saved Snippets

When using the Pieces Drive Sidebar in Obsidian, you can click on the **three vertical dots** on a saved code snippet to **delete** it, or select from 6 additional options:

***

| `View Preview`     | `Start Copilot Chat`      | `Copy to Clipboard`     |
| ------------------ | ------------------------- | ----------------------- |
| `Insert at cursor` | `Generate Shareable Link` | `Open Markdown Preview` |

***

## Real-Time Snippet Streaming

Every product within the Pieces Suite utilizes [PiecesOS](/products/core-dependencies/pieces-os) to gather information regarding the context of your snippets.

When you modify a snippet in the <a target="_blank" href="/products/desktop">Pieces for Developers Desktop App</a>—like changing its name or description, tags, or any other metadata—those updates are automatically shown in your <a target="_blank" href="https://obsidian.md/plugins?search=pieces-for-developers">Pieces for Obsidian Plugin</a> without the need for refreshing.

<Callout type="tip">
  If your snippets aren’t updating immediately, refer to the [troubleshooting guide](/products/obsidian/troubleshooting) for instructions on refreshing your snippet list.
</Callout>