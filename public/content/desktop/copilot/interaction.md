---
title: Using Pieces Copilot
path: /desktop/copilot/interaction
visibility: PUBLIC
status: PUBLISHED
description: Learn the basics of using the Pieces Copilot within the Pieces Desktop App, and discover how to navigate the view, find and start new conversations, add context, and utilize prebuilt chat pipelines.
metaTitle: Using Pieces Copilot | Pieces Docs
metaDescription: Introduction to Pieces Copilot – your AI assistant for technical queries, code generation, debugging, and workflow insights in a chat interface.
---

## Chat Interface & Navigation

When opening the Pieces Desktop App after installation, you are first presented with a default view—the Pieces Copilot.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/screenshot_of_copilot.png" alt="" align="center" fullwidth="true" />

This view is the central hub from which you can start new chats, access previous chats, and configure Long-Term Memory, models, and context to suit the task at hand.

## Main Chat Window

The central area of the Pieces Copilot view is a blank chat where you can start a new conversation.

To get the most out of generative AI using local or cloud models through Pieces Copilot, make sure you [check out our LLM Prompting Guide.](/products/quick-guides/ltm-prompting/tips)

At the top of the window, you will see a set of three *Suggested Prompts*—these dynamic prompts adapt based on your topics common to your workflow (if captured by LTM) and serve as a quick way to begin engaging with the AI.

Directly above the chat input field, a *Set Context* area provides four buttons:

* `LTM Context: Off / On`**:** Toggle whether to automatically include long-term memory context from your workflow.

* `Folders`**:** Opens a modal to add local code directories.

* `Files`**:** Opens a modal to add individual files.

* `Saved Materials`**:** Lets you pick items previously saved in Pieces Drive.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Interacting/add_snippet_to_copilot.gif" alt="" align="center" fullwidth="true" />

These buttons help you easily inject context into your chat so Pieces Copilot can deliver more accurate and relevant responses.

<Card title="Hey!" image="/assets/icons/platform_logos/pieces_logo.png">
  Do you know how to find specific LTM-sourced information, get deeplinks, and generate summaries of projects you’ve been working on with Pieces Copilot? If you don’t, [check out this Quick Guide.](/products/quick-guides/ltm-prompting/examples)
</Card>

## Input Field and Quick Actions

Inside the Pieces Copilot Chat view, there are several quick actions you can utilize that let you proactively adjust chat context—like toggling the LTM state, adding folders or websites containing code, and more.

### Text Input Field

At the bottom of the chat window is a text input field with the placeholder:

```markdown
“Paste code, drag and drop an image, or ask a technical question…” 
```

This is your primary area for entering queries or pasting code, and is flanked by buttons on either side for adding context or using other in-chat tools:

* To the *left* of the input field is the Quick Action button, which contains a modal menu with quick access to several context-adding actions.

* To the *right,* you’ll find actions to insert code blocks into the chat or extract code from screenshots.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Interacting/gif_of_running_through_all_options.gif" alt="" align="center" fullwidth="true" />

### Left-Side Quick-Action Button

Just to the left of the input field is a **Chat Bubble** icon.

Clicking it opens a [context menu](/products/desktop/copilot/integration) with a list of quick actions:

1. `LTM Context`**:** Toggle the current state—*on* or *off.*

2. `Add Files`**,** `Add Folders`**,** `Add Snippets`**,** `Add Websites`**:** Each option opens the corresponding modal for adding context from local resources or the web.

3. `Add Messages`**:** (Currently grayed out—coming soon.)

[Read more about adding context to your Pieces Copilot Chats.](/products/desktop/copilot/integration#adding-folders)

### Right-Side Tools

Next to the text input field, you’ll find:

1. A `{ }` button that, when clicked, automatically inserts a code block template (using triple backticks) for pasting code.

2. A square button featuring an `“A”` icon that enables you to extract code from screenshots. When you click this button, your file explorer opens, allowing you to select an image that contains code.

## Chat Options

There are 2 kinds of chat options available within the Pieces Copilot Chat view—actions which let you pin, refresh or delete chats, and the `New Chat` button with optional **Chat Pipelines.**

### Chat Options Menu

At the top right corner of the active chat window, a vertical ellipsis (three stacked dots) reveals additional options:

1. `Pin Chat`**:** Keeps the current chat pinned at the top of your sidebar.

2. `Refresh`**:** Reloads the chat if the AI stops generating a response.

3. `Delete`**:** Removes the chat from your history.

<Callout type="alert">
  These options are available inside of an existing chat with user input and AI generations—i.e., an *active* chat. You will not see these options when inside a blank chat template.
</Callout>

### New Chat & Pipelines

In the left sidebar, the `New Chat` button features a dropdown arrow.

When clicked, it presents you with 3 options:

***

| **Chat Pipeline**                       | **Type**                                         | **Use Case**                                                                                                          |
| --------------------------------------- | ------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
| *Generally discuss technical topics*    | Multipurpose                                     | For discussing more multi-modal, general but technical topics.                                                        |
| *Ask questions about a local code base* | Project-oriented comprehension and documentation | An optimized LLM pathway for keeping generations relevant to your code context. Useful for learning new codebases.    |
| *Generate code for a local project*     | Project-oriented code generation                 | Oriented for contextualized code generation—works best when local code repositories are added to the chat as context. |

***

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Interacting/chat_pipelines.png" alt="" align="center" fullwidth="true" />

<Callout type="tip">
  You can select one of these chat pipelines as the default pipeline when creating new chats.
</Callout>

## Sidebar & Chat History

When the Pieces Copilot view is opened, you are presented with a *left-hand sidebar* that displays your past chat conversations arranged chronologically.

This allows you to quickly revisit previous interactions by clicking on a chat entry with its date stamp.

An icon at the top of the sidebar lets you collapse or expand this panel as needed—called **Focus Mode**—so you can focus solely on your current conversation if desired.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Interacting/going_through_chat_history_and_exploring.gif" alt="" align="center" fullwidth="true" />