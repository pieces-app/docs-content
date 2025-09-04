---
title: Visual Studio Extension
path: /extensions-plugins/visual-studio
visibility: PUBLIC
status: PUBLISHED
description: The Pieces for Visual Studio Extension is a powerful tool that integrates smoothly with the Visual Studio IDE. It boosts productivity and supports efficient code management.
metaTitle: Using Pieces for Visual Studio | Pieces Docs
metaDescription: Chat with Pieces Copilot inside Visual Studio for AI-driven code insights, debugging help, and automated coding assistance.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/visual_studio_extension_MAIN/icons_banners/visual-studio.png" alt="" align="center" fullwidth="true" />

***

## Pieces for Visual Studio Extension

The <a target="_blank" href="https://marketplace.visualstudio.com/items?itemName=MeshIntelligentTechnologiesInc.pieces-vscode">Pieces for Visual Studio Extension</a> is a powerful and versatile tool that integrates seamlessly with the Visual Studio IDE, enhancing productivity and enabling efficient code management.

It provides users with a streamlined solution for managing and interacting with saved code snippets through the Pieces Drive, while leveraging the AI-powered capabilities of the Pieces Copilot—all directly within their development environment.

* [Pieces Copilot](/products/extensions-plugins/visual-studio/copilot): Engage in AI-driven conversations to enhance productivity by generating code, adding comments, troubleshooting, and more—all contextualized to your project by adding files and folders as context, with or without the powerful Long-Term Memory Engine (LTM).

* [Pieces Drive](/products/extensions-plugins/visual-studio/drive): Effortlessly save, locate, and share frequently used code snippets to your Pieces Drive—Making it easier to organize your work, quickly access essential pieces of code, and collaborate effectively with others.

<CardGroup cols={2}>
  <Card title="Getting Started" image="/assets/icons/visual_studio.png">
    Follow [these instructions](/products/extensions-plugins/visual-studio/get-started) to download and install the Pieces for Visual Studio IDE Extension.
  </Card>

  <Card title="Support & Troubleshooting" image="/assets/icons/platform_logos/pieces_logo.png">
    Explore [troubleshooting options](/products/extensions-plugins/visual-studio/troubleshooting), navigate to our [support page](/products/support), or <a target="_blank" href="https://calendar.google.com/calendar/u/0/appointments/schedules/AcZssZ22WJ2Htd2wRMJhueCNYc0xbFBFCAN-khijcuoXACd_Uux3wIhgZeGkzDRcqD3teamAI-CwCHpr">directly book a call</a> with our engineers.
  </Card>
</CardGroup>

<guides-overview-card />

This extension is designed to offer **two main pillars of functionality** for users working in the Visual Studio IDE—Pieces Copilot and Pieces Drive.

### AI Assistance with Pieces Copilot

Through Pieces Copilot, developers can generate code solutions with [context-based AI conversations](/products/extensions-plugins/visual-studio/copilot/chat), [add code comments](/products/extensions-plugins/visual-studio/copilot/documenting-code), <a target="_blank" href="/products/extensions-plugins/visual-studio/troubleshooting">troubleshoot</a>, and fix bugs inside Visual Studio.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/visual_studio_extension_MAIN/pieces_highlighted_showing_pieces_options.png" alt="" align="center" fullwidth="true" />

### Material Management with Pieces Drive

With Pieces Drive and PiecesOS built into Visual Studio, developers can [save](/products/extensions-plugins/visual-studio/drive/save-snippets), [edit](/products/extensions-plugins/visual-studio/drive/edit-update), [search](/products/extensions-plugins/visual-studio/drive/search-reuse), and [share](/products/extensions-plugins/visual-studio/drive/sharing) their code easily.

This feature allows developers to keep their favorite code in a personal, easy-to-access library. They can quickly review past work, find related authors and links with the extra details saved with each piece, and much more.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/visual_studio_extension_MAIN/snippet_saved_materials_open_in_sidebar.png" alt="" align="center" fullwidth="true" />

## Using Pieces Copilot

Inside Visual Studio, the Pieces Copilot offers **several powerful actions** to enhance your coding workflow using generative AI.

To begin, you can [initiate a conversation with the LLM of your choice](/products/extensions-plugins/visual-studio/copilot/chat) by right-clicking and selecting the `Ask Copilot About Selection` or any of the available Copilot Chat options.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/visual_studio_extension_MAIN/right_click_asking_about_something.gif" alt="" align="center" fullwidth="true" />

For added context, you can also add specific files, folders or even entire repositories to the conversation so that the LLM utilized by Pieces Copilot has a comprehensive understanding of your project and the task at hand.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/visual_studio_extension_MAIN/add_folders_to_context.png" alt="" align="center" fullwidth="true" />

You can also access `Pieces: Explain / Modify / Comment Selection with Copilot` commands from the right-click menu to easily get a breakdown of the code’s logic, make changes such as adding error handling, or add comments to your code.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/visual_studio_extension_MAIN/hovering_explain.png" alt="" align="center" fullwidth="true" />

### Using AI Quick Actions

The Pieces Copilot comes packaged with **AI Quick Actions**, which are similar to CodeLens actions that sit above functions nearest to your cursor.

These Quick Actions are nested under `Pieces`, which automatically sits above applicable functions.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/visual_studio_extension_MAIN/nested_pieces_in_function.png" alt="" align="center" fullwidth="true" />

<Callout type="alert">
  Unfortunately, Visual Studio does not support CodeLens features for Python, so **AI Quick Actions will not work in Python files.**\
  \
  Supported languages for CodeLens features (AI Quick Actions) include **C/C++, C#, Basic, VBScript, TypeScript, and JavaScript.**
</Callout>

With the new `Pieces > Comment` tool, the Pieces Copilot can generate meaningful, insertable documentation that explains your code's purpose and function.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/visual_studio_extension_MAIN/using_ai_quick_actions.png" alt="" align="center" fullwidth="true" />

Additionally, the `Pieces > Explain` feature can quickly generate a code logic breakdown while initiating a Copilot Chat conversation in the side window, providing deeper insights and context.

***

| Pieces > Comment | Pieces > Explain |
| ---------------- | ---------------- |

***

## Managing Your Code Snippets

Saving and managing code snippets with Pieces for Visual Studio extension is quick and effortless.

To save a snippet, simply right-click the selected code, hover over `Pieces`, and select `Save Current Selection to Pieces` or `Save Active File to Pieces`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/visual_studio_extension_MAIN/material_management_redo.png" alt="" align="center" fullwidth="true" />

Snippets are automatically stored in your Pieces Drive, keeping them organized and accessible—you can search for them using the `Search Pieces Drive` function, which can be found in the right-click menu.

Additionally, you can use the `Share Current Selection` option to share snippets with others directly from the extension easily.

<Callout type="tip">
  Common snippet types include utility functions, API requests, and reusable code blocks.
</Callout>

When you save snippets to your repository, Pieces enriches them with AI-generated metadata, including [tags, titles, authorship details, and descriptions](/products/extensions-plugins/visual-studio/drive/save-snippets#whats-stored-when-you-save-a-snippet), ensuring everything stays organized and accessible.

Below is a brief overview of the various material management options available within the Pieces for Visual Studio Extension:

* `Save Current Selection / Active File to Pieces`: Right-click a selected block of code or your entire active file and [save it to your Pieces Drive with AI-enriched metadata](/products/extensions-plugins/visual-studio/drive/save-snippets#whats-stored-when-you-save-a-snippet), ensuring easy access to frequently used snippets.

* `Ask Copilot About Selection`: [Start a conversation with Pieces Copilot](/products/extensions-plugins/visual-studio/copilot/chat#accessing-copilot-chat-in-vs-code) to gain insights, explanations, or suggestions for improvement for the selected code.

* `Share Current Selection`: [Share snippets with your team](/products/extensions-plugins/visual-studio/drive/sharing) by creating distributable copies of reusable code.

* `Search Pieces Drive`: [Find specific snippets in your repository](/products/extensions-plugins/visual-studio/drive/search-reuse#via-search-feature) using keywords, tags, or titles.

### **Referencing & Reusing**

The <a target="_blank" href="https://marketplace.visualstudio.com/items?itemName=MeshIntelligentTechnologiesInc.pieces-vscode">Pieces for Visual Studio Extension</a> provides robust search tools to help you quickly find and access your saved snippets.

You can [perform broad searches or narrow your results by using specific terms](/products/extensions-plugins/visual-studio/drive/search-reuse#via-search-feature) such as function names, keywords, or tags, making locating the exact code you need effortless.

Right-clicking anywhere in your active file, hovering over `Pieces`, and selecting `Search Pieces Drive` will open up the search bar in the Pieces Drive view—from there, enter your query or use filters to find the saved material you’re looking for.

As you search, snippets matching your query will be displayed in a filtered list of your previously saved snippets.

From there, you can open the snippet and see its metadata in markdown or use the Pieces Drive window to edit the enriched metadata saved alongside it.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/visual_studio_extension_MAIN/snippet_saved_materials_open_in_sidebar.png" alt="" align="center" fullwidth="true" />

***

## Download the Extension

Ready to streamline your development? Download the Pieces for Visual Studio Extension and follow our [installation guide to start.](/products/extensions-plugins/visual-studio/get-started)