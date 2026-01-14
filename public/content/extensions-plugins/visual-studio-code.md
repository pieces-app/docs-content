---
title: Visual Studio Code Extension
path: /extensions-plugins/visual-studio-code
visibility: PUBLIC
status: PUBLISHED
description: Learn more about the Pieces for Visual Studio Code (VSC) Extension.
metaTitle: Using the Pieces for Visual Studio Code Extension | Pieces Docs
metaDescription: Enhance VS Code with the Pieces Extension – manage code snippets and use AI-powered Copilot for seamless coding and workflow optimization.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/plugins_extensions/vsc.png"
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/plugins_extensions/vsc.png" alt="" align="center" fullwidth="true" />

***

## Pieces for Visual Studio Code

The <a target="_blank" href="https://marketplace.visualstudio.com/items?itemName=MeshIntelligentTechnologiesInc.PiecesVisualStudio">Pieces for VS Code Extension</a> is a versatile tool that integrates seamlessly with the VS Code editor and IDEs based on VS Code, such as Cursor.

It provides users with a streamlined way to manage and interact with saved code snippets and harness the capabilities of the AI-powered [Pieces Copilot](/products/extensions-plugins/visual-studio-code/copilot) directly within their coding environment.

* [Pieces Copilot](/products/extensions-plugins/visual-studio-code/copilot): Engage in AI-driven conversations to enhance productivity by generating code, adding comments, troubleshooting, and more—all contextualized to your project by adding files and folders as context, with or without the powerful Long-Term Memory Engine (LTM).

* [Pieces Drive](/products/extensions-plugins/visual-studio-code/drive): Effortlessly save, locate, and share frequently used code snippets to your Pieces Drive—Making it easier to organize your work, quickly access essential pieces of code, and collaborate effectively with others.

<CardGroup cols={2}>
  <Card title="Getting Started" image="/assets/icons/vs_code.png">
    Follow [these instructions](/products/extensions-plugins/visual-studio-code/get-started) to download and install the Pieces for VS Code Extension.
  </Card>

  <Card title="Support & Troubleshooting" image="/assets/icons/platform_logos/pieces_logo.png">
    Explore [troubleshooting options](/products/extensions-plugins/visual-studio-code/troubleshooting), navigate to our [support page](/products/support), or <a target="_blank" href="https://calendar.app.google/WVUDtUfNy5Vst3sH7">directly book a call</a> with our engineers.
  </Card>
</CardGroup>

<guides-overview-card />

This extension is designed to offer **two main pillars of functionality** for users working in the Visual Studio Code environment—Pieces Copilot and Pieces Drive.

## Enhanced AI Assistance

Through Pieces Copilot, developers can generate code solutions with [context-based AI conversations](/products/extensions-plugins/visual-studio-code/copilot/chat), [add code comments](/products/extensions-plugins/visual-studio-code/copilot/documenting-code), troubleshoot, and fix bugs inside VS Code.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/MAIN_vs_code_extension/new_right_click_menu.png" alt="" align="center" fullwidth="true" />

### Integrated Snippet Management

With Pieces Drive embedded in VS Code, developers can also [save, edit, search, and share their code snippets,](/products/extensions-plugins/visual-studio-code/drive) boosting productivity by keeping reusable code accessible.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/updated_vs_screenshots/main/updated_no_saved_mats_view.png" alt="" align="center" fullwidth="true" />

## Using Pieces Copilot

Inside VS Code, the Pieces Copilot offers **several powerful actions** to enhance your coding workflow using generative AI.

To start, you can [initiate a conversation with the LLM of your choice](/products/extensions-plugins/visual-studio-code/copilot/chat), providing as much context as needed by adding files, folders, or even entire repositories to the chat.

To explore options, select a portion of code, right-click, and hover over the `Pieces` item in the context menu.

From here, you’ll find several quick actions, including:

* `Modify Selection with Copilot`: Edit or transform the selected code to improve readability, optimize performance, or adapt it for other needs.

* `Explain Selection with Copilot`: Get detailed explanations of the code’s functionality.

* `Comment Selection with Copilot`: Generate inline comments to improve code clarity.

You can also use the `Ask Copilot About Active File` action to provide more context about your project. This helps Pieces Copilot **better understand your entire file** and **deliver more relevant suggestions.**

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/MAIN_vs_code_extension/hover_over_ask_active_file.png" alt="" align="center" fullwidth="true" />

### Using AI Quick Actions

The Pieces Copilot now comes packaged with **AI Quick Actions**, which are similar to CodeLens actions that sit above functions nearest your cursor.

With the new `Pieces: Comment` tool, the Pieces Copilot can [generate meaningful, insertable documentation](/products/extensions-plugins/visual-studio-code/copilot/documenting-code) explaining your code’s purpose and function, and `Pieces: Explain` can quickly [generate a breakdown of some code logic](/products/extensions-plugins/visual-studio-code/copilot/chat#via-pieces-explain) while simultaneously initiating a Copilot chat in the side window.

***

| `Pieces: Comment` | `Pieces: Explain` |
| ----------------- | ----------------- |

***

To get started, look for the **AI Quick Actions** buttons in your code. These buttons relocate depending on the location of the nearest visible functions. Then, click the documentation or explanation tool, depending on your use case.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/updated_vs_screenshots/main/pieces_quick_actions_add_comments.png" alt="" align="center" fullwidth="true" />

## Using Pieces Drive

Saving and managing code snippets within Pieces Drive in the VS Code extension is **simple** and **efficient**.

To save a snippet, right-click the selected code, hover over `Pieces`, and choose `Save Current Selection to Pieces`. You can also use the `Share` option to share snippets with others.

<Callout type="tip">
  Common snippet types include utility functions, API requests, and reusable code blocks.
</Callout>

When you save snippets to your Drive, Pieces enriches them with AI-generated metadata, such as [tags, titles, authorship details, and descriptions,](/products/extensions-plugins/visual-studio-code/drive/save-snippets#whats-stored-when-you-save-a-snippet) keeping everything organized and accessible.

You can find brief descriptions below of the different material management options available within the Pieces for VS Code Extension:

* `Save Current Selection to Pieces`: Right-click a code block and [save it to Pieces Drive with AI-enriched metadata](/products/extensions-plugins/visual-studio-code/drive/save-snippets#whats-stored-when-you-save-a-snippet), ensuring easy access to frequently used snippets.

* `Save Active File to Pieces`: [Save the entire active file to your repository](/products/extensions-plugins/visual-studio-code/drive/save-snippets#saving-active-files-to-pieces) in one action—ideal for preserving larger scripts or complete files.

* `Ask Copilot About Selection`: [Start a conversation with Pieces Copilot](/products/extensions-plugins/visual-studio-code/copilot/chat#pieces-ask-copilot-about-selection) to gain insights, explanations, or suggestions for improvement for the selected code.

* `Ask Copilot About Active File`: [Analyze the active file with Pieces Copilot](/products/extensions-plugins/visual-studio-code/copilot/chat#pieces-ask-about-active-file) to get insights and recommendations for your codebase.

* `Share`: [Share snippets with your team](/products/extensions-plugins/visual-studio-code/drive/sharing) by creating distributable copies of reusable code.

* `Search Pieces`: Quickly [find specific snippets in your repository](/products/extensions-plugins/visual-studio-code/drive/search-reuse#via-search-feature) using keywords, tags, or titles.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/MAIN_vs_code_extension/save_active_file_to_pieces.png" alt="" align="center" fullwidth="true" />

### Referencing & Reusing

The <a target="_blank" href="https://marketplace.visualstudio.com/items?itemName=MeshIntelligentTechnologiesInc.PiecesVisualStudio">Pieces for VS Code Extension</a> offers powerful search tools to quickly find and access your saved snippets.

You can [perform broad searches or refine results using specific terms](/products/extensions-plugins/visual-studio-code/drive/search-reuse#via-search-feature) like function names, keywords, or tags, making it easy to locate the exact code you need.

To search, right-click, hover over `Pieces`, and select `Search Pieces`.

This opens a search bar where you can input queries to find your snippets. Once found, [snippets can be shared or copied](/products/extensions-plugins/visual-studio-code/drive/search-reuse#viewing-and-reusing-saved-snippets) directly into your project.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/MAIN_vs_code_extension/share_right_click.png" alt="" align="center" fullwidth="true" />

***

## Download the Extension

Ready to streamline your development? Download the <a target="_blank" href="https://marketplace.visualstudio.com/items?itemName=MeshIntelligentTechnologiesInc.PiecesVisualStudio">Pieces for VS Code Extension</a> and follow our [installation guide to start.](/products/extensions-plugins/visual-studio-code/get-started)