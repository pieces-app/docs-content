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

3. `Add Messages`**:**

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

## Interacting with Generated Responses

When Pieces Copilot generates a reply, a toolbar appears with helpful buttons, icons, and cards to manage or reuse that output.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/ltm_27_rework_gifs/pieces_copilot/showing_available_toolbar_options_copilot.webp" alt="" align="center" fullwidth="true" />

### Response Toolbar Actions

There are several actions you can take under each generated Pieces Copilot response. 

1. `Model & Time`: A chip shows the model used (for example, Claude, GPT, Gemini, or a local model) and how long ago the response was generated.

2. `Copy`: Click the copy icon to copy the entire response to your clipboard.

3. `Export`: Export the response to your `Downloads` folder by default. You can select from PDF, markdown, or plaintext formats.

4. `Regenerate`: Use the refresh icon to re-run the response with the same model or a different one. Clicking opens a modal where you can select the model you want to use for the regeneration.

5. `Convert to Workstream Summary`: The paper icon converts this Copilot output into a Workstream Summary so you can capture and reference it later in your workflow.

6. `More Options (⋮)`: The three-dot menu reveals additional actions. You can select `Use as Context` to add that specific response as context for follow-up prompts, or `Delete Message` to remove the message from the current conversation.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/ltm_27_rework_gifs/pieces_copilot/copilot_message_available_options_toolbar.gif" alt="" align="center" fullwidth="true" />

<Callout type="tip">
  If LTM Context is enabled, you may also see related context cards surface beneath the response. These link to Workstream Activity Rollups that informed the generation.
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

## Searching Previous Chats

When you are in the Pieces Copilot view, click the search bar at the very top labeled `Find chats…`. 

This opens a centered modal showing your recent chats. 

You can scroll this list, and each item displays a percentage on the right that represents how relevant that chat likely is to your current workflow or how frequently you return to it.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/ltm_27_rework_gifs/pieces_copilot/showing_find_chats_search_field.png" alt="" align="center" fullwidth="true" />

### Running a Search

Type your query into the search field and press `enter` (Windows/Linux) or `return` (macOS) to execute the search. Results will appear with matching terms highlighted in yellow. 

If a chat is an exact match for your query, you’ll see an `EXACT MATCH` label on the right instead of a percentage.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/ltm_27_rework_gifs/pieces_copilot/searching_chats_yellow_syntax.png" alt="" align="center" fullwidth="true" />

<Callout type="tip">
  Pressing enter/return is **required** to run the search from the modal.
</Callout>

## Deep Study

Did you know that Pieces can provide highly accurate, sourced, timestamped deep research reports of your work history, personal projects, and progress on a given topic? 

DeepStudy leverages your Long-Term Memory so Copilot can analyze work across people, applications, topics, and time windows.

- **Deep contextual recall**: Connects information across timeframes, collaborators, and apps
- **Comprehensive recaps**: Summarizes work done over days, weeks, or months
- **Targeted queries**: Answers questions that specify people, topics, projects, and date ranges
- **Actionable insights**: Surfaces linked artifacts (issues, errors, files) and proposes next steps

Using this feature, simply ask Pieces Copilot *"Can you perform a deep study on what I've done for the last few days?"* using your selected local or cloud LLM, and you'll receive an in-depth report that you can save, share, or export on your given topic.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair/deep_study_demo.webp" alt="" align="center" fullwidth="true" />

<Callout type="tip">
  Deep Study requires that you enable the Long-Term Memory Engine.
</Callout>

### Example prompts

Use natural language and include time ranges, people, and topics when possible. 

Here's some prompts you can try: 

```text
Perform a deep study of what I worked on last week related to WebSocket errors.
```

```text
Tell me everything I did with [PERSON NAME] over the last 3 months.
```

```text
What did I accomplish related to [TOPIC] in [MONTH]?
```

```text
When was the last time I worked on [PROJECT/FILE]?
```