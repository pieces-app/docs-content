---
title: Search & Reuse
path: /cli/drive/search-reuse
visibility: PUBLIC
status: PUBLISHED
---

## Locate Materials in Pieces Drive

To find your snippets in Pieces CLI, you can use one of two methods: searching or manually checking the Pieces Drive list.

## How to Search for Saved Materials

From the terminal, you can search for code snippets and other materials stored in your Pieces Drive. Additionally, you can use search filters to refine your results.

### via Search Command

If you want to access your saved snippets directly within Pieces CLI, you can:

<Steps>
  <Step title="Open a Terminal">
    Accessing a terminal on your device varies by platform: Use your OS's search bar to type in `terminal` (for macOS/Linux) or `CMD` (for Windows).
  </Step>

  <Step title="Enter Search Command">
    Within your terminal, you can now enter `pieces search “query”`. This will start a new search using your query to search through your Pieces Drive.

    Alternatively, you can launch into Pieces CLI run mode with `pieces run`. This will enable you to just enter `search “query”`.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_drive/search_reuse/ncs_search_results.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

You can optionally add `--mode` followed by the search method you prefer:

* `ncs`: Performs a neural code search for your query.

* `fts`: Performs a full-text search for your query.

For example, `pieces search "query" --mode fts` will use the full-text search on your database with your query.

## Viewing and Reusing Saved Snippets

[Saved snippets](/products/cli/drive/saving-materials) can be viewed by opening them up directly from the Pieces Drive with `pieces list`, using your scroll wheel or arrow keys, and selecting the snippet with the `return` (macOS) or `enter` (Windows/Linux) key, all from within your terminal.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_drive/search_reuse/pieces_drive_list.png" alt="" align="center" fullwidth="true" />

In your terminal, you can also open snippets with the `pieces search “query” [optional: --mode ncs,fts]` command. If Pieces finds snippets that match your query, you will be presented with a list of snippets.

You can open a snippet from the list using your scroll wheel or arrow keys and select it with the `return` (macOS) or `enter` (Windows/Linux) key.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_drive/search_reuse/search_snippets.gif" alt="" align="middle" fullwidth="true" />

***

## Real-Time Snippet Streaming

Every product in the Pieces Suite uses [PiecesOS](/products/core-dependencies/pieces-os) to collect information about the context of your snippets.

When you change a snippet in the [Pieces Desktop App](/products/desktop)—such as its name, description, tags, or any other metadata—those updates automatically appear in your Pieces Drive without needing to refresh.

<Callout type="tip">
  If your snippets aren’t updating immediately, refer to the troubleshooting guide for guidance on refreshing your snippet list.
</Callout>
