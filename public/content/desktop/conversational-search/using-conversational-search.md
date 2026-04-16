---
title: Using Conversational Search
path: /desktop/conversational-search/using-conversational-search
visibility: PUBLIC
status: PUBLISHED
description: Learn how to talk with your memories, filter searches, switch models, and work with responses in Conversational Search.
metaTitle: Using Conversational Search | Pieces Docs
metaDescription: Learn how to talk with your memories, filter searches, switch models, and work with responses in Conversational Search.
---

***Conversational Search*** is the ability to talk with your memories. You can have conversations with your captured workflow context—ask specific questions, search through your memories, and filter by apps or time ranges to customize which memories you're talking with. All responses are powered by [Long-Term Memory (LTM-2.7)](/products/core-dependencies/pieces-os#ltm-27).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/landing_overview_conversational_chat_and_examples.png" alt="Conversational Search interface with suggested prompts, chat input, model selector" align="center" fullwidth="true" />

> Full Conversational Search interface on homepage showing suggested prompts, chat input, model selector, and bottom toolbar

## Talking with Your Memories

Have conversations with your captured workflow context. Ask specific questions about your past work, decisions, or activities.

### Suggested Prompts

Suggested prompts appear as clickable buttons based on your recent workflow. Click any prompt to instantly start that conversation. Responses include Related Timeline Events cards showing which memories were used as sources.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/clicking_on_sample_prompt.gif" alt="Clicking suggested prompt showing response with Related Timeline Events cards" align="center" fullwidth="true" />

> Clicking a suggested prompt, showing the complete flow from click to response with Related Timeline Events cards

### Asking Your Own Questions

Type your own questions to have conversations with your memories about specific topics or moments.

<Steps>
  <Step title="Start a New Chat">
    Click `Start New Chat` to begin a fresh conversation.
  </Step>

  <Step title="Type Your Question">
    Type your question in the input field and press Enter to send.
  </Step>

  <Step title="Get Your Answer">
    You'll get a response powered by LTM-2.7 with context from your captured memories.
  </Step>
</Steps>

**Example questions:**
* "Why did we choose PostgreSQL over MySQL for the authentication project?"
* "What was the blocker I encountered last Tuesday afternoon?"
* "Find that React performance article I read last month"
* "What did Sarah and I discuss about the API redesign in Teams?"
* "Show me the code changes I made related to WebSocket connections"

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/using-conversational-search/conversational_chat_with_sample_question.png" alt="Start New Chat button and input field with example question typed" align="center" fullwidth="true" />

> Start New Chat button and input field with example question typed

### Starting Fresh Chats

Use `Start New Chat` when you want to discuss a completely different topic. Starting a new chat ensures better results when switching topics since Conversational Search uses relevant memory context across the entire conversation.

### Scoping a chat to one summary or event

You cannot attach local files or folders to Conversational Search. To focus the assistant on **one** specific memory (for example a generated summary), open that item in [Pieces Timeline](/products/desktop/timeline), open the **three-dots menu** (⋮) on the event, and choose **`Chat`**. See [Chat from a summary](/products/desktop/timeline/event-actions#chat-from-a-summary). For a broader slice of memories, use **Sources** and **Time Ranges** below.

## Filtering Your Searches

Filter by specific apps or time ranges to narrow your search scope and get more focused answers.

### Sources Filter

Limit searches to memories from specific applications. Use this when you want answers based only on specific apps.

<Steps>
  <Step title="Click Sources Button">
    Click the `Sources` button in the *bottom toolbar* to open the filter modal.
  </Step>

  <Step title="Select Apps">
    Check the apps you want to include. You can select multiple apps at once.
  </Step>

  <Step title="Apply Filter">
    Selected sources apply to your current chat and all future messages until you change them.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/conversational_search_filter_sources.png" alt="Sources filter modal with app checkboxes, Chrome and VS Code selected" align="center" fullwidth="true" />

> Sources filter modal showing list of apps with checkboxes, with Chrome and VS Code selected

### Time Ranges Filter

Focus searches on specific time periods. Use this when you need information from a specific period.

<Steps>
  <Step title="Click Time Ranges Button">
    Click the `Time Ranges` button in the *bottom toolbar* to open the filter modal.
  </Step>

  <Step title="Select Time Range">
    Choose from 31+ preset options (e.g., "Yesterday", "This week", "Last month") or use the calendar view for custom date ranges. You can select multiple ranges at once.
  </Step>

  <Step title="Apply Filter">
    Selected time ranges apply to your current chat and all future messages until you change them.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/conversational_search_filter_time.png" alt="Time Ranges modal showing preset options and calendar view" align="center" fullwidth="true" />

> Time Ranges modal showing preset options and calendar view

### Combining Filters

Use Sources and Time Ranges together for precise queries—for example, "Chrome browsing from yesterday afternoon."

## Working with Responses

### Ask Follow-Up About Selected Text

Highlight any text in an AI response and click `Ask follow-up` to add it as context for your next message. The selected text appears in a context box above the chat input—type your follow-up question and send. The box can be dismissed with the `X` icon if you change your mind.

### Response Toolbar Actions

All response actions are available in the *toolbar* below each response:

* **Model & time:** A chip shows which model produced the answer and how long ago the response was generated.

* **Copy:** Click the `clipboard icon` to copy the entire response to your clipboard
* **Export:** Click the `export icon` to download responses as PDF (for sharing/printing), Markdown (for editing), or Plain Text
* **Regenerate:** Click the `regenerate icon` (circular arrow) to re-run the response with the same model or switch to a different one for comparison
* **Convert to Timeline Event:** Click the `paper/document icon` to save important responses—they'll appear in the *memories sidebar* for later reference
* **Use as Context:** Click the `three-dot menu` (`⋮`) and select "Use as Context" to add the response as context for follow-up questions

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/conversational_search_response_options.png" alt="Response toolbar with Copy, Export, Regenerate, and Convert buttons" align="center" fullwidth="true" />

> Response toolbar showing Copy, Export, Regenerate, Convert to Timeline Event, and More menu buttons labeled

### Related Timeline Events

Cards appear below responses showing which source Timeline Events were used to generate the answer. Click any card to view the full Timeline Event details and verify where information came from.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/relevant_summaires_conversational_chat.png" alt="Response with Related Timeline Events cards showing memory titles and timestamps" align="center" fullwidth="true" />

> Response with Related Timeline Events cards below showing memory titles and timestamps

## Model Selection

Switch between cloud and local models based on your needs. Use cloud models (Claude, GPT, Gemini) for faster responses and advanced reasoning. Use local models (o3, o1) for complete privacy and offline capability.

<Steps>
  <Step title="Open Model Selector">
    Click the `model button` in the *bottom toolbar* to open the model selector.
  </Step>

  <Step title="Choose a Model">
    You'll see Recent models you've used, Suggested models for your current task, or click `All Models` to see everything available.
  </Step>

  <Step title="Switch Models">
    When you switch models, your chat history stays intact, and new messages will use the selected model.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/using-conversational-search/model_selection_in_desktop_app.png" alt="Model selector dropdown with recent, suggested, and all models options" align="center" fullwidth="true" />

> Model selector dropdown 

### LLM runtime modal

Click the active model control (for example the model name in the bottom toolbar) to open the **LLM runtime** modal. There you can enter API keys if needed, switch models, and open the full catalog of [local and cloud-hosted models served through Pieces](/products/core-dependencies/pieces-os#local-vs-cloud-models).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/ltm_27_rework_gifs/new_list_of_models_cloud.webp" alt="LLM runtime modal listing cloud and local models in Conversational Search" align="center" fullwidth="true" />

<Callout type="info">
  Some cloud models are available to Pieces Pro users only (for example: OpenAI GPT-5.2 Pro/GPT-5.2, Anthropic Claude 4.5 Opus, Google Gemini 3 Pro Preview). To unlock premium models, see [Pieces Pro](/paid-plans).
</Callout>

Cloud models from OpenAI, Anthropic, and Google (and others) are listed on the [Cloud Models](/products/large-language-models/cloud-models) page. For on-device options and privacy, use local models; the full catalog for the Desktop App is in [supported local and cloud models](/products/core-dependencies/local-models/supported-models).

### Browse and download local models

Open the LLM runtime modal, open **All Models**, then scroll to find local models. Select a model to download it on demand through PiecesOS; once downloaded, you can run it entirely on your device.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Desktop%20App/scrolling_through_llms.gif" alt="Scrolling the All Models list to browse and download local models" align="center" fullwidth="true" />

<Callout type="tip">
  Local models run through PiecesOS on your device for privacy and offline use.
</Callout>

### Reset a conversation

When you need a clean slate, use **Chat Options** on an active thread to reset the conversation so context and messages start fresh for that chat.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/ltm_27_rework_gifs/pieces_copilot/gif_of_resetting_conversation.gif" alt="Resetting a Conversational Search conversation from Chat Options" align="center" fullwidth="true" />

### Chat appearance and defaults

In the LLM runtime area, open the `Settings` gear to set a chat accent color and choose whether **LTM context** is on by default for **new** chats.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Settings/Aesthetics/changing_colors.png" alt="Conversational Search appearance settings with accent color and LTM default toggle" align="center" fullwidth="true" />

You can also use `cmd+shift+t` (macOS) or `ctrl+shift+t` (Windows/Linux) to toggle the Desktop App *Dark/Bright* theme.

## Asking Effective Questions

The more specific your questions, the better Conversational Search can find relevant memories and provide accurate answers.

### Use Specific Keywords

Include unique keywords related to what you're looking for—project names, ticket numbers, package names, or specific topics.

**Good:** "What is the status of project Aurora?"

**Bad:** "What is the status of my project?"

<Callout type="tip">
  If you can't remember specific keywords, try asking: "Give me the titles of all the project documents I've been working on last month" to find keywords for more specific prompts.
</Callout>

### Include Time Ranges

Specify when something happened to narrow down results. Conversational Search stores up to 9 months of memories.

**Examples:**
* "What decision did we make about the database schema last week?"
* "What were the plans I received in December?"
* "What was I debugging yesterday afternoon?"

### Mention Source Applications

Reference specific apps to separate similar content across different sources.

**Example:** "What did Sarah and I discuss in Teams about the deployment?"

This separates Teams conversations from emails or document comments.

### Combine Techniques

Mix keywords, time ranges, and applications for the most accurate results.

**Example:** "What is the URL for the Project Aurora document I discussed in Teams with Sarah last Thursday?"

This combines the keyword "Project Aurora," the application "Teams," the person "Sarah," and the time "last Thursday" to narrow down results precisely.

### Use Filters Instead of Prompts

If you know the exact source app or time range, use the `Sources` and `Time Ranges` filters instead of describing them in your prompt. Filters are more accurate than natural language time expressions.

## LTM Context Toggle

Control whether Conversational Search includes Long-Term Memory context in your conversations. When enabled, your chats automatically draw from up to 9 months of captured workflow context.

<Callout type="info">
  LTM must be enabled to access the chat feature in Pieces Desktop. If LTM is off, chat does not work. LTM is enabled by default in conversations.
</Callout>

### Enabling or Disabling LTM Context

<Steps>
  <Step title="Click User Profile">
    Click your `User Profile` in the top left of the Pieces Desktop App.
  </Step>
  <Step title="Hover Over LTM-2.7">
    Hover over `LTM-2.7` in the dropdown menu that appears.
  </Step>
  <Step title="Toggle LTM">
    To keep LTM active, ensure it is not paused or turned off. To disable, select a pause duration (15 minutes, 1 hour, 6 hours, 12 hours, or 24 hours) or choose `Turn Off`. When paused or off, Conversational Search will not include workflow history context.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/context-integration/hovering_over_ltm_turnoff.png" alt="Toggling LTM context for Conversational Search" align="center" fullwidth="true" />

> User profile menu showing LTM-2.7 hover menu with pause and turn off options

### Viewing the Relevant Summaries Sidebar

After receiving a response, see exactly which Timeline Events were used to generate it.

<Steps>
  <Step title="Find Relevant Summaries Button">
    Look for the `Relevant Summaries` button at the bottom of a chat response.
  </Step>
  <Step title="Open Sidebar">
    Click the button to open the sidebar on the right side. Each entry shows the Timeline Event title, description, timestamp, and related applications.
  </Step>
  <Step title="Sort Summaries (Optional)">
    Click the sort dropdown in the top right of the sidebar—options include `Suggested`, `Recent`, and `Most Viewed`.
  </Step>
  <Step title="Click a Timeline Event">
    Click any Timeline Event to view full details about when it was captured and what context it contains.
  </Step>
</Steps>

## Managing Your Chat History

All conversations automatically save to the *memories sidebar*, listed chronologically with other workflow activities. Click any saved chat to reopen it with full history and preserved filter settings. Use **Focus Mode** (the control at the top of the sidebar) to collapse the sidebar when you want to concentrate on the active thread.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Interacting/going_through_chat_history_and_exploring.gif" alt="Sidebar chat history and Focus Mode toggle in Conversational Search" align="center" fullwidth="true" />

<Callout type="tip">
  Your chat history is part of your LTM memories. Conversational Search can reference previous conversations when answering new questions.
</Callout>

### Find chats

Click the search field labeled `Find chats…` at the top of the Conversational Search view to open a modal of recent threads. Each row can show a **relevance** percentage (or an `EXACT MATCH` label). Type a query and press `Enter` / `Return` to run the search; matching text is highlighted in the results.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/ltm_27_rework_gifs/pieces_copilot/showing_find_chats_search_field.png" alt="Find chats search field showing recent chats with relevance percentages" align="center" fullwidth="true" />

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/ltm_27_rework_gifs/pieces_copilot/searching_chats_yellow_syntax.png" alt="Chat search results with highlighted terms and exact match labels" align="center" fullwidth="true" />

## Input field, quick actions, and chat options

The input area supports rich prompts: paste code, drop an image, or ask a technical question. Use the quick-action (chat bubble) menu beside the field for shortcuts (for example toggling LTM-related options). On the right, tools can insert a fenced code block or extract code from a screenshot via the file picker.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Interacting/gif_of_running_through_all_options.gif" alt="Quick actions and tools beside the Conversational Search input field" align="center" fullwidth="true" />

To scope the whole chat to **one** captured summary or event, use **`Chat`** on that item’s three-dots menu in Timeline—not the input shortcuts. See [Chat from a summary](/products/desktop/timeline/event-actions#chat-from-a-summary) and [Scoping a chat from Timeline](/products/desktop/conversational-search/context-integration#scoping-a-chat-from-timeline).

### Chat options menu

On an **active** thread (after you have sent messages), open the `⋮` menu at the top of the chat to **Pin Chat**, **Refresh** if generation stalls, or **Delete** the conversation. These options do not appear on a blank new chat.

<Callout type="alert">
  Pin, Refresh, and Delete appear only inside a chat that already has user input and assistant replies.
</Callout>

### Chat pipelines

When you start a **New Chat**, you can pick a **chat pipeline** that shapes how the model uses context:

| **Pipeline** | **Type** | **Use case** |
| --------------------------------------- | ------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------- |
| *Generally discuss technical topics* | Multipurpose | General technical discussion and mixed modalities. |
| *Ask questions about a local code base* | Project-oriented comprehension | Optimized when LTM has captured relevant IDE or repo activity; pair with [Chat from a summary](/products/desktop/timeline/event-actions#chat-from-a-summary) if you need one memory in scope. |
| *Generate code for a local project* | Project-oriented generation | Optimized when recent workflow memories include the project; use **Chat** on a relevant Timeline summary when you need a focused session. |

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Interacting/chat_pipelines.png" alt="Chat pipeline dropdown with multipurpose, comprehension, and generation options" align="center" fullwidth="true" />

<Callout type="tip">
  You can set one of these pipelines as the default when creating new chats.
</Callout>

## Deep Study (Pieces Pro)

Deep Study uses your Long-Term Memory to produce **sourced, timestamped research-style reports** across apps, people, topics, and time ranges.

* **Deep contextual recall** across collaborators, apps, and sessions
* **Recaps** over days, weeks, or months
* **Targeted queries** with people, topics, projects, and dates
* **Actionable insights** with links to artifacts and suggested next steps

Ask naturally—for example: *"Can you perform a deep study on what I've done for the last few days?"*

### How to activate Deep Study (Pro)

At the bottom of the chat, click `Activate DeepStudy` (marked **PRO**). Your **next** prompt runs the Deep Study workflow. Deep Study requires **Long-Term Memory** to be enabled.

### What to expect

* **Duration:** Often on the order of 10–20 minutes depending on how much recent context is included.
* **Progress:** After you submit a deep-study prompt, you’ll see progress and a `Thinking` state; expand sections to inspect intermediate agent steps.

### Model used for Deep Study

Deep Study runs on a **dedicated cloud model** managed by Pieces (currently a Google model; subject to change). Your per-chat model choice applies to normal replies; Deep Study always uses its own runtime.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/ltm_27_rework_gifs/deep_study_demo_with_agentic_progress_meter.webp" alt="Deep Study progress UI with thinking state and agent steps" align="center" fullwidth="true" />

### Example prompts

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

<Card title="Hey!" image="/assets/icons/platform_logos/pieces_logo.png">
  For LTM-specific prompting patterns, see the [LTM Prompting Guide](/products/quick-guides/ltm-prompting) and [examples](/products/quick-guides/ltm-prompting/examples).
</Card>

***

## Next Steps

Now that you know how to use Conversational Search, learn how to start context-specific conversations directly from your workflow memories.

[Starting a conversation with a Timeline Event →](/products/desktop/conversational-search/chat-with-timeline-events)
