---
title: Pieces CLI
path: /cli
visibility: PUBLIC
status: PUBLISHED
description: The Pieces CLI is a flexible command-line interface for Pieces that integrates smoothly with your development environment.
metaTitle: Using the Pieces CLI | Pieces Docs
metaDescription: Learn how to use Pieces CLI for seamless command-line integration, allowing you to save, retrieve, and manage code snippets efficiently.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/CLI_MAIN/pieces_cli_banner.png" alt="" align="center" fullwidth="true" />

***

## Pieces CLI

The Pieces CLI offers users a straightforward way to manage and utilize saved code snippets through the Pieces Drive. It uses the AI-powered features of the [Pieces Copilot](/products/cli/copilot), all directly within your terminal.

* [Pieces Copilot](/products/cli/copilot): Utilize AI-driven conversations to enhance productivity by offering contextual assistance for your projects. It helps you understand code, write code comments, perform troubleshooting, and more by incorporating files and folders as context, with or without the powerful Long-Term Memory Engine (LTM-2.5).

* [Pieces Drive](/products/cli/drive): Easily save, find, and share your frequently used code snippets in your Pieces Drive. This makes organizing your work easy, allows for quick access to the code you need, and facilitates effective collaboration with others.

<CardGroup cols={2}>
  <Card title="Getting Started" image="https://cdn.hashnode.com/res/hashnode/image/upload/v1745331342247/687c66b0-ac65-412f-a9e0-39e6ac00c93b.png">
    Follow [these instructions](/products/cli/get-started) on how to download and install the Pieces CLI.
  </Card>

  <Card title="Support & Troubleshooting" image="https://cdn.hashnode.com/res/hashnode/image/upload/v1745331350108/c3c9ac64-c629-447a-a8fc-307d1f8f297b.webp">
    Explore [troubleshooting options](/products/cli/troubleshooting), navigate to our support page, or <a target="_blank" href="https://calendar.google.com/calendar/u/0/appointments/schedules/AcZssZ22WJ2Htd2wRMJhueCNYc0xbFBFCAN-khijcuoXACd_Uux3wIhgZeGkzDRcqD3teamAI-CwCHpr">directly book a call</a> with our engineers.
  </Card>
</CardGroup>

<Card title="Learn More with Quick Guides" image="https://cdn.hashnode.com/res/hashnode/image/upload/v1747065928779/0f8466fc-9daf-4c91-87ba-f596cd1cd6d3.png">
  Pieces Quick Guides help you quickly understand and utilize powerful features like the Long-Term (LTM-2.5) Memory Engine and Pieces Copilot. [Click here to get started.](/products/quick-guides/overview)
</Card>

This software is designed to offer **two main features**: AI Assistance with the Pieces Copilot and developer material management within the Pieces Drive.

### Enhanced AI Assistance

Through the Pieces CLI, developers can boost productivity by having AI-driven conversations that use [relevant notes and folders as context](/products/cli/copilot/chat), all within their terminal.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_copilot/chat/pieces_context_chat.gif" alt="" align="center" fullwidth="true" />

### Integrated Snippet Management

With Pieces Drive and PiecesOS in their terminal, developers can [save, search, and share their code snippets](/products/cli/drive). This enhances productivity by making reusable code accessible and organized within their notes and project files.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/CLI_MAIN/pieces_drive_list.png" alt="" align="center" fullwidth="true" />

## Using Pieces Copilot

The Pieces CLI enhances your workflow by letting you save, manage, and share snippets in the terminal. It offers features like snippet enrichment, sharing via custom links, and seamless integration with your development environment.

To explore available options, run `pieces help` within your terminal.

From here, you’ll find several actions, including:

* `Edit`: [Change the name and classification of the material](/products/cli/drive/edit-and-update) within Pieces Drive from directly within the terminal.

* `Create and Delete`: Pieces CLI allows you to [manage your snippets easily from within your terminal](/products/cli/drive/saving-materials), allowing you to create and delete snippets.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/CLI_MAIN/edit_command.png" alt="" align="center" fullwidth="true" />

## Managing Your Code Snippets

Saving and managing materials with the Pieces CLI is done with lightweight and familiar terminal-style commands.

To save a snippet, copy a section of text or code to your clipboard, head over to Pieces CLI, and type `pieces create`. If you’re in `pieces run` mode, you can just type `create`.

<Callout type="tip">
  Common snippet types include utility functions, API requests, and reusable code blocks.
</Callout>

When you save snippets to your Pieces Drive with Pieces CLI, they get AI-generated metadata like [tags, titles, authorship details, and descriptions](/products/cli/drive/save-snippets#whats-stored-when-you-save-a-snippet). This keeps everything organized and easy to access and use at any point.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/CLI_MAIN/snippet_content.png" alt="" align="center" fullwidth="true" />

### Referencing & Reusing

Pieces CLI provides you with powerful search tools to quickly find and access your snippets that you previously saved to Pieces Drive.

There are three different search methods: *Fuzzy Search*, *Neural Code Search*, and *Full Text Search.*

To search for snippets, while Pieces CLI is open, type `search “query”`.

You can also opt-in to using Neural Code Search with `—mode ncs` or Full Text Search with `—mode fts`.

<Callout type="info">
  Your query must be encapsulated in quotations for Pieces CLI to capture your full prompt
</Callout>

A new terminal window will open and you’ll be presented with a list of materials that closely match your query.

Scroll down or up with the `arrow keys` and select the material by pressing `enter`. The material will display with its attributes and the code that was stored in the material.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/CLI_MAIN/ncs_search_results.png" alt="" align="center" fullwidth="true" />

***

Download the Pieces CLI and follow our [installation guide](/products/cli/get-started) to start streamlining your workflow!