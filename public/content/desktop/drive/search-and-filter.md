---
title: Searching & Filtering Materials
path: /desktop/drive/search-and-filter
visibility: PUBLIC
status: PUBLISHED
description: Learn how to find materials from your Pieces Drive using basic and advanced filtering techniques.
metaTitle: Search & filter code snippets in Pieces Drive | Pieces Docs
metaDescription: Easily search and filter saved code snippets in Pieces Drive using powerful search, filters, and language-based sorting for quick access.
---

## Finding Materials in Pieces Drive

As your collection of saved snippets and code files grows, finding the right material at the right time becomes critical.

Pieces Drive addresses this need with a powerful search engine, user-friendly filters, and intuitive ways to narrow down results by content, language, and more. 

## Using the Search Bar

At the very top of the Pieces Drive view is the **Search Bar**, labeled *Find Materials.*

This is your starting point for quick lookups.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Drive/Searching%20%26%20Filtering%20Materials/searching_pieces_drive.png" alt="" align="center" fullwidth="true" />

### Natural Language Queries

Pieces supports more than simple keyword matching.

Type a phrase like *“How to parse JSON in Python,”* and it looks through titles, annotations, and snippet content for matches.

If you recall partial details about a snippet—*“route handler,”* for example—Pieces tries to interpret your intent and provide the best possible matches.

### Instant Results

After you type your query, results populate in the Saved Materials List on the left.

Each matching snippet’s auto-generated title and a quick preview appear—just click any snippet to open it in the main detail pane.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Navigation/Global%20Search/quick_search_filters.png" alt="" align="center" fullwidth="true" />

<Callout type="tip">
  Searching “local storage React” can bring up multiple snippets involving React’s local storage usage, even if the phrase “local storage” doesn’t appear verbatim in the snippet title.
</Callout>

## Quick Filters

Right next to the search bar, you’ll see **Quick Filter** toggles in the dropdown that can help you narrow down your search quickly.

These are:

* `Titles`: Matches against snippet titles (auto-generated or custom).

* `Annotations`: Matches text that appears in the snippet’s annotations or descriptions.

* `Content`: Matches the literal code or text content of your snippet.

You can enable one, two, or all three filters at once.

***

| **Filter**    | **Search Type**                                                                        | **Result** |
| ------------- | -------------------------------------------------------------------------------------- | ---------- |
| *Title*       | Matches against snippet titles (auto-generated or custom).                             | ✅          |
| *Annotation*  | Matches text that appears in the snippet’s annotations or descriptions.                | ✅          |
| *Content*     | Matches the literal code or text content of your snippet.                              | ✅          |
| *All Filters* | Pieces searches titles, annotations, and snippet code simultaneously—broadest results. | ✅          |

***

This level of granularity helps you quickly dial into the snippet you need without scrolling through dozens of partial matches.

## Advanced Filtering

For deeper searching, Pieces Drive offers an **Add Search Filters** feature which has an icon, located to the left or right of the Quick Filters (depending on your interface layout).

These advanced filters let you refine your search using specific criteria and store them for later reuse.

### via Language, Tags, and Phrases

Pieces lets you filter using *language*, *tags* and specific *natural language phrases* so that you see only what you need to see—this is particularly useful if you have similar-sounding snippets across multiple languages.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Drive/Searching%20%26%20Filtering%20Materials/search_filters.png" alt="" align="center" fullwidth="true" />

There are a few different use cases for searching with these methods:

* `Language`**:** Search your Pieces Drive for saved materials written in Python, C#, JavaScript, TypeScript, or other languages.

* `Tags`**:** If you only want backend-related Node.js snippets, you can add a *tag* filter for *“Node.js”* AND *“backend.”*

* `Phrase`**:** If you remember an exact line of code or an exact phrase, place it within quotes to perform a more strict search (e.g., "server.listen(port)").