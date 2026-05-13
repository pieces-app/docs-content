---
title: Talk with Your Memories
path: /desktop/conversational-search/using-conversational-search
visibility: PUBLIC
status: PUBLISHED
description: Learn how to talk with your memories, filter searches, switch models, and work with responses in Conversational Search.
metaTitle: Talk with Your Memories | Pieces Docs
metaDescription: Learn how to talk with your memories, filter searches, switch models, and work with responses in Conversational Search.
---

***Conversational Search*** is the ability to talk with your memories through **Agentic Chats**. Powered by [Agentic Long-Term Memory](/products/core-dependencies/pieces-os#ltm-27), the agent reasons across your artificial memory in multiple turns, following threads, cross-referencing context, and building toward complete answers instead of guessing in one shot.

Ask specific questions, search through your memories, and filter by apps or time ranges to customize which memories you're talking with. The agent can search your memories, the web, your calendar, local files, and browser history to build complete answers.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/conversational-search/homepage_conversational_search.png" alt="Conversational Search interface with suggested chats, recent chats, chat input, and model selector" align="center" fullwidth="true" />

> Full Conversational Search interface on homepage showing suggested chats, recent chats, chat input, model selector, and bottom toolbar

## Talking with Your Memories

Have conversations with your captured workflow context. Ask specific questions about your past work, decisions, or activities.

### Suggested Chats

Personalized chat suggestions appear on the homepage under *Suggested Chats for You*, generated from your recent workflow activity. Click any suggestion to instantly start that conversation. Responses include Related Timeline Events cards showing which memories were used as sources.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/clicking_on_sample_prompt.gif" alt="Clicking a suggested chat showing response with Related Timeline Events cards" align="center" fullwidth="true" />

> Clicking a suggested chat, showing the complete flow from click to response with Related Timeline Events cards

### Resume Recent Chats

Continue where you left off with your most recent conversations.

<Steps>
  <Step title="Find Resume Recent Chats">
    Look below the *Suggested Chats* section on the homepage.
  </Step>
  <Step title="Click a Chat Card">
    Click any card showing a conversation title and timestamp.
  </Step>
  <Step title="Continue Your Conversation">
    The chat opens with full history and context intact—type a follow-up question to continue.
  </Step>
</Steps>

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

### Adding Files and Folders as Context

Attach local files or folders to give Conversational Search additional context beyond your LTM memories.

<Steps>
  <Step title="Click the + Button">
    Click the `+` button to the left of the chat input field.
  </Step>
  <Step title="Select Files or Folders">
    Browse and select files or folders from your device. Alternatively, drag and drop files directly into the chat input area.
  </Step>
  <Step title="Verify Context Chips">
    Attached items appear as context chips above the input field.
  </Step>
  <Step title="Ask Your Question">
    Type your question—the agent uses the file contents alongside your LTM memories when generating responses.
  </Step>
</Steps>

### Scoping a chat to one summary or event

To focus the assistant on **one** specific memory (for example a generated summary), open that item in [Pieces Timeline](/products/desktop/timeline), open the **three-dots menu** (⋮) on the event, and choose **`Chat`**. See [Chat from a summary](/products/desktop/timeline/event-actions#chat-from-a-summary). For a broader slice of memories, use the **Filter By...** menu below to scope by Apps, Time, or Modality.

## Filtering Your Searches

Filter which memories are used when answering your questions.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/conversational-search/filter_results_by_menu.png" alt="Filter Results By menu showing Apps, Time, and Modality filter options" align="center" fullwidth="true" />

> Filter Results By menu showing Apps, Time, and Modality filter options

<Steps>
  <Step title="Open the Filter Menu">
    Click the `Filter By...` button (filter icon) in the *bottom toolbar*.
  </Step>
  <Step title="Choose a Filter Category">
    Hover over **Apps**, **Time**, or **Modality** to see available options.
  </Step>
  <Step title="Select Your Filters">
    Check the options you want to include. You can combine multiple filters.
  </Step>
  <Step title="Ask Your Question">
    Type your question—results will only include memories matching your filters.
  </Step>
</Steps>

### Filter by Apps

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/conversational-search/filter_by_apps.png" alt="Filter by Apps submenu showing available applications" align="center" fullwidth="true" />

> Filter by Apps submenu showing available applications to include in your search

<Steps>
  <Step title="Hover Over Apps">
    In the filter menu, hover over **Apps**.
  </Step>
  <Step title="Check Applications">
    Select the applications you want to include (e.g., Chrome, VS Code, Slack, Teams).
  </Step>
</Steps>

### Filter by Time

<Steps>
  <Step title="Hover Over Time">
    In the filter menu, hover over **Time**.
  </Step>
  <Step title="Choose a Preset or Custom Range">
    Select a preset (Yesterday, This week, Last month) or click **Custom** to set a specific date range.
  </Step>
</Steps>

### Modality

Restrict searches to specific types of captured context—the method by which a memory was formed. Hover over **Modality** to see the available types:

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/conversational-search/filter_by_modality.png" alt="Filter by Modality submenu showing Vision, Clipboard, Audio, and Google Calendar options" align="center" fullwidth="true" />

> Filter by Modality submenu showing Vision, Clipboard, Audio, and Google Calendar options

* **Vision** — What you’ve seen (screen context captured by LTM).
* **Clipboard** — What you’ve copied and pasted.
* **Audio** — What you’ve said and heard.
* **Google Calendar** — Events and meeting context from connected calendars.

Click **Manage Connections** at the bottom of the Modality panel to enable, disable, or authorize integrations.

### Combining Filters

Combine Apps, Time, and Modality filters for precise queries—for example, "Chrome browsing from yesterday afternoon," or "anything I copied from Slack last week," or "meetings on my Google Calendar this month."

## Working with Responses

### Ask Follow-Up About Selected Text

Highlight text from a response to ask follow-up questions about it.

<Steps>
  <Step title="Highlight Text">
    Click and drag to select any text in an AI response.
  </Step>
  <Step title="Click Ask Follow-Up">
    Click the `Ask follow-up` button that appears.
  </Step>
  <Step title="Review the Context Box">
    The selected text appears in a context box above the chat input.
  </Step>
  <Step title="Type Your Follow-Up">
    Type your follow-up question and press Enter to send. Click the `X` icon to dismiss if you change your mind.
  </Step>
</Steps>

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

Browse and switch models directly from chat, without navigating to Settings. The model picker shows inline descriptions and capabilities so you can choose the right model for your task.

| Mode | Speed | Quality | Best For |
| --- | --- | --- | --- |
| **Fast** | Fastest | Good | Quick questions, simple lookups, code completion |
| **Balanced** | Moderate | Better | General tasks, summaries, explanations |
| **Extra Thinking** | Slower | Best | Complex reasoning, debugging, multi-step analysis |

<Steps>
  <Step title="Open Model Selector">
    Click the `model button` in the *bottom toolbar* to open the model inventory.
  </Step>

  <Step title="Browse Built-In Models">
    Under *Built-In Models*, you'll see **Claude**, **Gemini**, and **GPT**. Hover over any provider to see available modes.
  </Step>

  <Step title="Choose a Provider and Mode">
    Under *Built-In Models*, hover over **Claude**, **Gemini**, or **GPT** to see Fast, Balanced, and Extra Thinking modes.
  </Step>

  <Step title="Select a Model">
    Click your choice. The model switches immediately for your next message.
  </Step>
</Steps>

Your chat history stays intact when you switch models. New messages use the selected model while previous responses remain unchanged.

### All Models

Click `All Models` to browse the full catalog, including cloud models, local models (via Ollama), BYOK configurations, and enterprise deployments. Local models run entirely on your device through PiecesOS for privacy and offline use.

The unified model inventory works across all providers: OpenAI, Anthropic, Google, AWS Bedrock, Azure, OpenRouter, on-device models, and more.

<Callout type="info">
  Some cloud models are available to Pieces Pro users only. To unlock premium models, see [Pieces Pro](/paid-plans).
</Callout>

For detailed model configuration, see [Choose a Model](/products/desktop/conversational-search/models).

### Reset a conversation

When you need a clean slate, use **Chat Options** on an active thread to reset the conversation so context and messages start fresh for that chat.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/ltm_27_rework_gifs/pieces_copilot/gif_of_resetting_conversation.gif" alt="Resetting a Conversational Search conversation from Chat Options" align="center" fullwidth="true" />

### Chat appearance and defaults

In the LLM runtime area, open the `Settings` gear to set a chat accent color and choose whether **LTM context** is on by default for **new** chats.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Settings/Appearance/appearance_settings.png" alt="Conversational Search appearance settings with accent color and LTM default toggle" align="center" fullwidth="true" />

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

If you know the exact source app, time range, or type of memory you're looking for, use the `Filter By...` menu to scope by Apps, Time, or Modality instead of describing them in your prompt. Filters are more accurate than natural language time expressions.

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

## Chat Input & Bottom Toolbar

The chat input area includes a text field where you type your questions, along with a toolbar below it with the following controls (left to right):

* **`+` (Add Context)** — Attach local files or folders to the conversation. You can also drag and drop files directly into the input area.
* **`Filter By...`** — Open the [filter menu](#filtering-your-searches) to scope by Apps, Time, or Modality.
* **Model selector** — Shows the active model (e.g., `Claude · Fast`). Click to switch between cloud and local models.
* **Reflection Mode (lotus icon)** — Toggle the agent’s ability to reflect on its own reasoning and self-correct in real time. See [Reflection Mode](#reflection-mode).
* **`Send`** — Send your message. You can also press `Enter`.

To scope the whole chat to **one** captured summary or event, use **`Chat`** on that item’s three-dots menu in Timeline. See [Chat from a summary](/products/desktop/timeline/event-actions#chat-from-a-summary) and [Scoping a chat from Timeline](/products/desktop/conversational-search/context-integration#scoping-a-chat-from-timeline).

### Queue Up Your Next Message

Type your next message while the agent is still responding. Queued messages send automatically when the current response finishes.

<Steps>
  <Step title="Type While Waiting">
    While the agent is generating a response, type your follow-up question in the input field.
  </Step>
  <Step title="Queue or Interrupt">
    Press `Enter` to queue the message for automatic sending, or click `Send` to **stop the current response** and immediately send your new message instead.
  </Step>
</Steps>

<Callout type="tip">
  Interrupting is useful when you realize mid-response that you want to steer the agent in a different direction, especially during longer agentic chats where the agent is doing multi-step work.
</Callout>

### Chat options menu

On an **active** thread (after you have sent messages), open the `⋮` menu at the top of the chat to **Pin Chat**, **Refresh** if generation stalls, or **Delete** the conversation. These options do not appear on a blank new chat.

<Callout type="alert">
  Pin, Refresh, and Delete appear only inside a chat that already has user input and assistant replies.
</Callout>

### Token Usage per Conversation

Track how many tokens each conversation consumes. Every chat shows cumulative token usage broken down by **input**, **output**, **reasoning**, and **cache**. Both LLM calls and tool calls are counted, giving you full visibility into the true cost of agentic work.

<Steps>
  <Step title="Open Token Stats">
    In an active chat, look for the token usage indicator in the chat header or response toolbar.
  </Step>
  <Step title="View Breakdown">
    Click to expand the breakdown showing input tokens (your prompts), output tokens (responses), reasoning tokens (agent thinking), and cached tokens (reused context).
  </Step>
</Steps>

Token tracking helps you:

* **Manage API usage** if you're on a metered plan or using BYOK
* **Compare model efficiency** by seeing which models use more tokens for similar tasks
* **Understand agentic costs** since multi-turn reasoning and tool calls add up

## Reflection Mode

Reflection Mode enables the agent to reflect on its own reasoning and self-correct in real time. When enabled, the agent produces higher-quality responses by evaluating its logic as it generates answers, catching errors and refining its output before delivering it to you.

### Enabling Reflection Mode

Toggle Reflection Mode using the `lotus icon` in the *bottom toolbar*, next to the model selector. Hover over the icon to see the tooltip: *"Enable Reflection Mode — Agent will reflect on its own reasoning and self-correct in real time."*

When Reflection Mode is active, the agent automatically engages deeper research and analysis based on the complexity of your prompt—no manual activation required. Complex questions about your workflow history, multi-step investigations, and cross-app analysis all benefit from Reflection Mode.

<Card title="Hey!" image="/assets/icons/platform_logos/pieces_logo.png">
  For LTM-specific prompting patterns, see the [LTM Prompting Guide](/products/quick-guides/ltm-prompting) and [examples](/products/quick-guides/ltm-prompting/examples).
</Card>

***

## Next Steps

Now that you know how to use Conversational Search, learn how to start context-specific conversations directly from your workflow memories.

[Starting a conversation with a Timeline Event →](/products/desktop/conversational-search/chat-with-timeline-events)
