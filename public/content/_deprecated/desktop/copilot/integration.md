---
title: Integrating Context & Projects
path: /desktop/copilot/integration
visibility: PUBLIC
status: PUBLISHED
description: Learn how to enrich your Conversational Search chats by integrating context—like folders, file, and other saved materials—from your previous tasks and current projects.
metaTitle: Integrate context and projects with Conversational Search | Pieces Docs
metaDescription: Learn how to use Conversational Search within the Pieces Desktop App, navigate the view, find and start new conversations, add context, and utilize prebuilt chat.
---

## Using Context with Conversational Search

Adding context to Conversational Search chats makes responses significantly more relevant and useful—especially when that context is pulled directly from your workflow.

<Card title="Want to learn more about using LTM Context?" image="/assets/icons/platform_logos/pieces_logo.png">
  Check out the [LTM Prompting Guide](/products/quick-guides/ltm-prompting) or learn how to use [Conversational Search with LTM Context](/products/quick-guides/copilot-with-context) via these helpful Quick Guides.
</Card>

## Enriching Chats with LTM-2.7 Context

Integrating context ensures Conversational Search isn’t answering in a vacuum.

By including Long-Term Memory data and project-specific resources, you can improve the accuracy of generative AI responses, reduce context-switching, work more effectively.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/ltm_27_rework_gifs/pieces_copilot/showing_pfd_ltm_source_gif.gif" alt="Conversational Search response with LTM Workstream Activity context cards" align="center" fullwidth="true" />

### Related Workstream Activities

Conversational Search will draw on memories and workflow context captured by the LTM engine to prepare a relevant, context-rich answer for you.

The Timeline cards will display under the response with several cards linking to past timeline events that contain the context used to create that response.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/ltm_27_rework_gifs/pieces_copilot/querying_pieces_copilot.gif" alt="Timeline context cards under a Copilot response linking to past events" align="center" fullwidth="true" />

<Callout type="tip">
  Clicking one of the surfaced context cards will take you to that specific Roll-Up in **Timeline**.
</Callout>

### LTM Context Toggle

Below the *Set Context* section of the main Conversational Search view, you have the option to enable LTM Context. 

When turned on, your long-term memory data—captured by PiecesOS from your previous workflow—is automatically injected into every new chat.

This means that even if you start a fresh conversation, Conversational Search has access to important context from earlier sessions.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Settings/Additional%20Settings/toggling_ltm.gif" alt="Toggling LTM context on in Conversational Search view" align="center" fullwidth="true" />

### Adding Folders

Click the `Folders` button in the *Set Context* area.

This opens the **Manage Copilot Context** modal, where you can add local code directories.

To do so, click `Add Folders` to open your Finder (macOS) or File Explorer (Windows/Linux).

Select the directories that you want Conversational Search to use as context. This is especially useful when working on large projects where entire folders contain valuable code references.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Interacting/adding_folder_to_copilot_chat.png" alt="Adding folders as context in Manage Copilot Context" align="center" fullwidth="true" />

### Adding Files

Similarly, clicking the `Files` button opens the same modal so you can select individual files from anywhere on your device.

Click `Add Files` to select specific code files.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Interacting/add_file_copilot.png" alt="Adding individual files as Copilot context" align="center" fullwidth="true" />

These files are then parsed by Conversational Search to provide precise answers related to your code.

### Adding Websites

If you need to reference external code on a website—like on Stack Overflow—click the `Add Websites` option, which is accessible via the [Quick Action menu.](/products/desktop/drive/enrichment-and-metadata#using-the-quick-menu)

This opens a modal where you can enter a website URL.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Context%20%26%20Projects/add_Website.png" alt="Adding a website URL as Copilot context" align="center" fullwidth="true" />

Websites with code snippets or technical documentation can then be used as contextual material for your Conversational Search queries.

## Enriching Chats with Saved Materials

You can also add saved materials from the [Pieces Drive](/products/desktop/drive) into your Conversational Search Chat as context for the conversation.

### Selecting Saved Materials

Clicking the `Saved Materials` button opens up an interface that displays a clickable list of code snippets and documents previously saved in Pieces Drive.

Choose the relevant saved material that you’d like to include in your current conversation.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Interacting/add_snippet_to_copilot.gif" alt="Selecting saved materials from Pieces Drive as Copilot context" align="center" fullwidth="true" />

This ensures that Conversational Search is aware of your pre-curated, AI-enriched materials and can reference them in its responses.
