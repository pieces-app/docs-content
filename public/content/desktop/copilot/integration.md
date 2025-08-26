---
title: Integrating Context & Projects
path: /desktop/copilot/integration
visibility: PUBLIC
status: PUBLISHED
description: Learn how to enrich your Pieces Copilot chats by integrating context—like folders, file, and other saved materials—from your previous tasks and current projects.
metaTitle: Integrate context and projects with Pieces Copilot | Pieces Docs
metaDescription: Learn how to use Pieces Copilot within the Pieces Desktop App, navigate the view, find and start new conversations, add context, and utilize prebuilt chat.
---

## Using Context with Pieces Copilot

Adding context to Pieces Copilot chats makes responses significantly more relevant and useful—especially when that context is pulled directly from your workflow.

<Card title="Want to learn more about using LTM Context?" image="https://cdn.hashnode.com/res/hashnode/image/upload/v1743103872340/1b9ffce3-f465-4c7e-afd8-5e98d2a8fba5.png">
  Read this [LLM Prompting Guide](/products/quick-guides/ltm-prompting/tips) or learn how to use [Pieces Copilot with LTM Context](/products/quick-guides/copilot-with-context) via these helpful Quick Guides.
</Card>

## Enriching Chats with LTM-2.5 Context

Integrating context ensures Pieces Copilot isn’t answering in a vacuum.

By including Long-Term Memory data and project-specific resources, you can improve the accuracy of generative AI responses, reduce context-switching, work more effectively.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Context%20%26%20Projects/switching_context_in_activity.gif" alt="" align="center" fullwidth="true" />

### Related Workstream Activities

Pieces Copilot will draw on memories and workflow context captured by the LTM engine to prepare a relevant, context-rich answer for you.

The Workstream Activity cards will display under the response with several cards linking to past *Workstream Activity Rollups* that contain the context used to create that response.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/pieces_copilot/pieces_copilot_MAIN/copilot_worksteam_activity.gif" alt="" align="center" fullwidth="true" />

<Callout type="tip">
  Clicking one of the surfaced context cards will take you to that specific Rollup in the **Workstream Activities** view.
</Callout>

### LTM Context Toggle

Below the *Set Context* section of the main Pieces Copilot view, you have the option to enable LTM Context.

When turned on, your long-term memory data—captured by PiecesOS from your previous workflow—is automatically injected into every new chat.

This means that even if you start a fresh conversation, Pieces Copilot has access to important context from earlier sessions.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Settings/Additional%20Settings/toggling_ltm.gif" alt="" align="center" fullwidth="true" />

### Adding Folders

Click the `Folders` button in the *Set Context* area.

This opens the **Manage Copilot Context** modal, where you can add local code directories.

To do so, click `Add Folders` to open your Finder (macOS) or File Explorer (Windows/Linux).

Select the directories that you want the Pieces Copilot to use as context. This is especially useful when working on large projects where entire folders contain valuable code references.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Interacting/adding_folder_to_copilot_chat.png" alt="" align="center" fullwidth="true" />

### Adding Files

Similarly, clicking the `Files` button opens the same modal so you can select individual files from anywhere on your device.

Click `Add Files` to select specific code files.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Interacting/add_file_copilot.png" alt="" align="center" fullwidth="true" />

These files are then parsed by Pieces Copilot to provide precise answers related to your code.

### Adding Websites

If you need to reference external code on a website—like on Stack Overflow—click the `Add Websites` option, which is accessible via the [Quick Action menu.](/products/desktop/drive/enrichment-and-metadata#using-the-quick-menu)

This opens a modal where you can enter a website URL.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Context%20%26%20Projects/add_Website.png" alt="" align="center" fullwidth="true" />

Websites with code snippets or technical documentation can then be used as contextual material for your Pieces Copilot queries.

## Enriching Chats with Saved Materials

You can also add saved materials from the [Pieces Drive](/products/desktop/drive) into your Pieces Copilot Chat as context for the conversation.

### Selecting Saved Materials

Clicking the `Saved Materials` button opens up an interface that displays a clickable list of code snippets and documents previously saved in Pieces Drive.

Choose the relevant saved material that you’d like to include in your current conversation.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Interacting/add_snippet_to_copilot.gif" alt="" align="center" fullwidth="true" />

This ensures that the Pieces Copilot is aware of your pre-curated, AI-enriched materials and can reference them in its responses.