---
title: Searching Pieces Drive
path: /extensions-plugins/visual-studio/drive/search-reuse
visibility: PUBLIC
status: PUBLISHED
description: The Pieces for Visual Studio Extension lets you quickly find saved snippets, keeping you productive without interrupting your workflow.
metaTitle: How to Search & Retrieve Code Snippets in Visual Studio with Pieces Drive
metaDescription: Quickly find and reuse saved snippets in Visual Studio with Pieces Drive, helping you stay productive without interruptions.
---

## Finding Saved Snippets

In Visual Studio, you can locate your snippets in two main ways.

### via Pieces Sidebar

To locate your snippets, use the Pieces Sidebar menu or the search feature:

<Steps>
  <Step title="Open the Pieces Drive">
    There are three main ways to search your Pieces Drive via the Pieces Sidebar

    **via Right-Click Menu**

    Right-click in your editor window, hover over `Pieces`, and select `Search Pieces Drive`.

    **via Keyboard Shortcut**

    1. You can quickly open the search bar menu by pressing `alt+m`, letting go, and then quickly pressing the `f` key.

    Once you’ve opened the search bar, you can enter your search query to search for a specific snippet.
  </Step>

  <Step title="Open a Snippet">
    Click on the snippet to see its content, metadata, and quick actions.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/using_snippets/saving_snippets/opening_snippet_markdown.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

### via Search Feature

If you know exactly what you’re looking for, you can search for specific snippets:

<Steps>
  <Step title="Click the Search Bar">
    Open the search bar at the top of the Pieces Drive Sidebar.
  </Step>

  <Step title="Enter Your Search Query">
    Type your search query into the search box.
  </Step>

  <Step title="Navigate the Results">
    Scroll through the results or use the arrow keys to select your desired snippet.
  </Step>

  <Step title="Open the Snippet">
    Click on the snippet to open it and view its content, metadata, and quick actions.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/using_snippets/saving_snippets/searching_snippets.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

<Callout type="tip">
  Search using tags, descriptions, names, types, or languages to narrow your results.
</Callout>

## Adding Filters to Your Search

To refine your search results, you can sort and filter saved snippets in the Pieces Drive Sidebar.

### Filtering Snippets

<Steps>
  <Step title="Click on the Search Bar">
    Click the search bar at the top of the Pieces Drive Sidebar.
  </Step>

  <Step title="Use Quick Filters">
    Apply quick filters like `Titles`, `Annotations`, or `Content` that show up below the search bar.
  </Step>

  <Step title="Filter by Tags or Keywords">
    Enter specific tags or keywords in the search bar to narrow down the snippets shown.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/using_snippets/saving_snippets/filtering_snippets.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

### Sorting Snippets

<Steps>
  <Step title="Click the Sorting Icon">
    Click the icon at the top of the Pieces Drive sidebar (like the clock icon for recent). The icon changes depending on the sorting method you choose.
  </Step>

  <Step title="Choose Sorting Order">
    Choose your sorting order: `Recent`, `Suggested`, `Alphabetical`, or `Language`.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/using_snippets/saving_snippets/sorting_snippets.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

## Viewing and Reusing Saved Snippets

[Saved snippets](/products/extensions-plugins/visual-studio/drive/save-snippets) can be viewed with their metadata by opening them directly from the Pieces Sidebar. Just click on them once you find them.

From this view, use Quick Actions to copy the snippet or insert it at your cursor in the editor. Click `Open Markdown Preview` to **see the snippet in markdown preview mode,** or click on the snippet for a quick overview.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/using_snippets/using_snippets_MAIN/opened_markdown_snippet.png" alt="" align="center" fullwidth="true" />

From this view, you can highlight and right-click to copy, or use `ctrl+c` to copy to your clipboard.

### via Pieces Sidebar

In the Pieces Drive sidebar, you can insert a snippet into your note by clicking the `Insert at Cursor` button.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/using_snippets/saving_snippets/inserting_snippet_via_drive.gif" alt="" align="center" fullwidth="true" />

You can right-click a snippet and select `Copy to Clipboard` to paste it wherever you need.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/using_snippets/search_resuse/hovering_over_copy_to_clipboard.png" alt="" align="center" fullwidth="true" />

### Previewing Saved Snippets

When using the Pieces Drive sidebar in Visual Studio, click on the **three vertical dots** on a saved code snippet to **delete** it or choose from 6 other options:

***

| `View Preview`     | `Start Copilot Chat`      | `Copy to Clipboard`     |
| ------------------ | ------------------------- | ----------------------- |
| `Insert at cursor` | `Generate Shareable Link` | `Open Markdown Preview` |

***

## Real-Time Snippet Streaming

Every product in the Pieces Suite uses [PiecesOS](/products/core-dependencies/pieces-os) to collect information about the context of your snippets.

When you change a snippet in the [Pieces for Developers Desktop App](/products/desktop)—such as its name, description, tags, or any other metadata—those updates automatically appear in your [Pieces for Visual Studio Extension](https://marketplace.visualstudio.com/items?itemName=MeshIntelligentTechnologiesInc.PiecesVisualStudio) without needing to refresh.

<Callout type="info">
  If your snippets aren’t updating immediately, refer to the [troubleshooting guide](/products/extensions-plugins/visual-studio/troubleshooting) for instructions on refreshing your snippet list.
</Callout>