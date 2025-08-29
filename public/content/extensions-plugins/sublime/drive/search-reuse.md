---
title: Searching
path: /extensions-plugins/sublime/drive/search-reuse
visibility: PUBLIC
status: PUBLISHED
description: You can find your saved code easily with the Pieces for Sublime Text Plugin by utilizing a few different search methods.
metaTitle: How to Search & Retrieve Code Snippets in Sublime with Pieces Drive
metaDescription: Quickly find and reuse saved snippets in Sublime Text with Pieces Drive’s powerful search tools.
---

## Locate Materials in Pieces Drive

One of the most powerful tools baked into the Pieces for Sublime Text Plugin is the search functionality which allows you to utilize **three different searching methods.**

To get started open the command palette using `⌘+shift+p` (macOS) or `ctrl+shift+p` (Windows/Linux) and type `Pieces: Search`. You’ll be presented with the options to use Neural, Fuzzy, and Full Text code searching.

### via Fuzzy Search

Fuzzy Search helps find relevant matches even with typos, misspellings, or variations.

It’s great for locating partially-remembered function names, error messages, log entries, or comments, saving time with flexible, quick searches.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair_2/sublime/fuzzy_search.png" alt="" align="center" fullwidth="true" />

### via Full Text Search

Full Text Search finds documents or records with an exact word match.

It indexes all words for fast searching, ideal for specific queries like function declarations, pulling up matching snippets and related classes efficiently.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair_2/sublime/full_text_search.png" alt="" align="center" fullwidth="true" />

### via Neural Code Search

Neural Code Search uses machine learning to find code snippets based on natural language descriptions.

It captures context and semantics, delivering accurate results, especially helpful for new developers or complex queries.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/using_snippets/search_and_reuse/search_natural_NPL.gif" alt="" align="middle" fullwidth="true" />

## Viewing and Reusing Saved Snippets

[Saved snippets](/products/extensions-plugins/sublime/drive/save-snippets) can be viewed alongside their saved metadata by opening up them up directly from the command palette.

### via Command Palette

<Steps>
  <Step title="Open the Command Palette">
    Open the Command Palette using `⌘+shift+p` (macOS) or `ctrl+shift+p` (Windows/Linux)
  </Step>

  <Step title="Open Saved Materials">
    Type in `Pieces: Open Saved Material` to access your saved materials
  </Step>

  <Step title="Select a Snippet">
    Scroll through the list to find the snippet you’d like to view
  </Step>

  <Step title="Open the Snippet">
    Highlight the desired snippet and press `return` (macOS) or `enter` (Windows/Linux)
  </Step>
</Steps>

This opens up the snippet in markdown preview mode in a separate window. In the new window, you have the ability to [share, view metadata, edit, copy, or delete the snippet](/products/extensions-plugins/sublime/drive).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/using_snippets/search_and_reuse/open_saved_media.gif" alt="" align="center" fullwidth="true" />

## Real Time Snippet Streaming[​](/extensions-plugins/jetbrains#real-time-snippet-streaming)

Each product in the Pieces Suite uses [PiecesOS](/products/core-dependencies/pieces-os) to get information about your snippets' context.

When you update a snippet in the [Pieces for Developers Desktop App](/products/desktop)—such as a name or description, tags or any of the other metadata—those changes are also reflected in your Pieces for Sublime Text Plugin without refreshing.

<Callout type="tip">
  If your snippets are not updating right away, see the [troubleshooting guide](/products/extensions-plugins/sublime/troubleshooting) for details on how to refresh your snippet list.
</Callout>