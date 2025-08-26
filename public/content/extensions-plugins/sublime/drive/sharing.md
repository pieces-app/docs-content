---
title: Sharing Snippets
path: /extensions-plugins/sublime/drive/sharing
visibility: PUBLIC
status: PUBLISHED
description: The Share Snippets feature in the Pieces for Sublime Text Plugin lets users create shareable links for code snippets directly from the interface, simplifying sharing with others.
metaTitle: How to Share Code Snippets in Sublime with Pieces Drive
metaDescription: Easily share code snippets from Sublime Text using Pieces Drive’s shareable links.
---

## How to Share a Saved Snippet

To create a link that you can share anywhere, right-click on a section of selected code, hover over the `Pieces` option, and then choose `Generate Shareable Link`.

A prompt will appear, allowing you to either `Copy` or `Dismiss` the shareable link.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/using_snippets/sharing/gen_shareable_link.png" alt="" align="center" fullwidth="true" />

When you click `Generate Shareable Link`, the Pieces Copilot will generate the link, then open a small menu with two options—`Copy` or `Dismiss`, allowing you to either copy the link or disregard the link.

Selecting `Copy` will copy the shareable URL to your clipboard:

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/using_snippets/sharing/using_snippets_menu_generate_shareable_link_1092024.png" alt="" align="center" fullwidth="true" />

This feature allows the recipient to easily access and view the snippet, even if they don't have Pieces installed or have a Pieces account.

<Callout type="tip">
  This link can easily be shared via email, Discord, Slack, or other platforms. The recipient can view the snippet **without needing to have a Pieces account.**
</Callout>

## Generating Links for Existing Snippets

In addition to sharing code snippets on the fly, you can also open up previously saved materials and generate a shareable link from the embedded `Share` button.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/using_snippets/using_snippets_PARENT_PAGE/sharing_saved_media.gif" alt="" align="center" fullwidth="true" />

## Enriched Sharing Experience

When you `Share` a snippet, it’s not just the code that’s included. The snippet comes with additional metadata to provide context—[you can read more about that here.](/products/extensions-plugins/sublime/drive/save-snippets#whats-stored-when-you-save-a-snippet)

* `Snippet Type`: Identify the language or framework, such as Python or React.

* `Tags`: Useful keywords for quick categorization.

* `Description`: A short summary of what the snippet does.

* `Related Links`: Helpful resources or documentation tied to the snippet.

* `Author Information`: A record of who created the snippet.

<Image src="https://cdn.hashnode.com/res/hashnode/image/upload/v1733970528143/f4acf9e2-0d73-4634-8695-a6cdcfbd3814.png" alt="" align="center" fullwidth="true" />

## What Information Gets Shared

When a snippet is saved to the Pieces Cloud, the code is [enriched with valuable information](/products/extensions-plugins/sublime/drive/save-snippets#whats-stored-when-you-save-a-snippet) such as related people, links, annotations, tags, and an automatically-generated description.

This information is visible to the right of the code block when the shared snippet is open in your browser:

<Image src="https://cdn.hashnode.com/res/hashnode/image/upload/v1733970040011/f627038f-b8f3-46f8-8235-600d1a8a8efd.png" alt="" align="center" fullwidth="true" />

### Sensitive Information Watchdog

The `Generate Shareable Link` feature does more than just allow you to effectively share snippets across your entire team and other communities, though.

You'll see a section titled **Sensitive Information:**

<Image src="https://cdn.hashnode.com/res/hashnode/image/upload/v1733970500459/864946d3-8d27-435c-beb4-01f5d37e5fdc.png" alt="" align="center" fullwidth="true" />

Our in-house ML model scans snippets for potentially sensitive information, like API keys or passwords, and alerts you so that you can make an informed decision before sharing the snippet.  

The scan happens locally using on-device machine learning models **before the snippet is uploaded to the cloud** for sharing—that way, you can make an informed decision about sharing your code.