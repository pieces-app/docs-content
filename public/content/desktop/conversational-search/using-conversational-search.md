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

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/landing_overview_conversational_chat_and_examples.png" alt="" align="center" fullwidth="true" />

> Full Conversational Search interface on homepage showing suggested prompts, chat input, model selector, and bottom toolbar

## Talking with Your Memories

Have conversations with your captured workflow context. Ask specific questions about your past work, decisions, or activities.

### Suggested Prompts

Suggested prompts appear as clickable buttons based on your recent workflow. Click any prompt to instantly start that conversation. Responses include Related Timeline Events cards showing which memories were used as sources.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/clicking_on_sample_prompt.gif" alt="" align="center" fullwidth="true" />

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

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/using-conversational-search/conversational_chat_with_sample_question.png" alt="" align="center" fullwidth="true" />

> Start New Chat button and input field with example question typed

### Starting Fresh Chats

Use `Start New Chat` when you want to discuss a completely different topic. Starting a new chat ensures better results when switching topics since Conversational Search uses relevant memory context across the entire conversation.

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

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/conversational_search_filter_sources.png" alt="" align="center" fullwidth="true" />

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

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/conversational_search_filter_time.png" alt="" align="center" fullwidth="true" />

> Time Ranges modal showing preset options and calendar view

### Combining Filters

Use Sources and Time Ranges together for precise queries—for example, "Chrome browsing from yesterday afternoon."

## Working with Responses

All response actions are available in the *toolbar* below each response:

* **Copy:** Click the `clipboard icon` to copy the entire response to your clipboard
* **Export:** Click the `export icon` to download responses as PDF (for sharing/printing), Markdown (for editing), or Plain Text
* **Regenerate:** Click the `regenerate icon` (circular arrow) to re-run the response with the same model or switch to a different one for comparison
* **Convert to Timeline Event:** Click the `paper/document icon` to save important responses—they'll appear in the *memories sidebar* for later reference
* **Use as Context:** Click the `three-dot menu` (`⋮`) and select "Use as Context" to add the response as context for follow-up questions

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/conversational_search_response_options.png" alt="" align="center" fullwidth="true" />

> Response toolbar showing Copy, Export, Regenerate, Convert to Timeline Event, and More menu buttons labeled

### Related Timeline Events

Cards appear below responses showing which source Timeline Events were used to generate the answer. Click any card to view the full Timeline Event details and verify where information came from.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/relevant_summaires_conversational_chat.png" alt="" align="center" fullwidth="true" />

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

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/using-conversational-search/model_selection_in_desktop_app.png" alt="" align="center" fullwidth="true" />

> Model selector dropdown 

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

## Managing Your Chat History

All conversations automatically save to the *memories sidebar*, listed chronologically with other workflow activities. Click any saved chat to reopen it with full history and preserved filter settings.

<Callout type="tip">
  Your chat history is part of your LTM memories. Conversational Search can reference previous conversations when answering new questions.
</Callout>

***

## Next Steps

Now that you know how to use Conversational Search, learn how to start context-specific conversations directly from your workflow memories.

[Starting a conversation with a Timeline Event →](/products/desktop/conversational-search/chat-with-timeline-events)
