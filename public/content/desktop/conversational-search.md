---
title: Conversational Search
path: /desktop/conversational-search
visibility: PUBLIC
status: PUBLISHED
description: Chat with workflow context captured by Long-Term Memory in the Pieces Desktop App.
metaTitle: Conversational Search | Pieces Docs
metaDescription: Use Conversational Search in Pieces Desktop to ask questions about captured workflow context, with optional filters and file attachments.
---

<Embed 
  src="https://youtu.be/Anlbmu9hCOg" 
  title="Conversational Search overview video demonstrating the interface, suggested chats, and example conversations"
/>

***

## Overview

**Conversational Search** is the chat interface in the Pieces Desktop App. You ask questions about past work, and responses draw on context captured by the [Long-Term Memory (LTM-2.7)](/products/core-dependencies/pieces-os/long-term-memory) Engine.

You can include all captured memories or limit scope by app, time range, and modality. You can also attach local files and folders. Chats are saved to [Pieces Timeline](/products/desktop/timeline) so you can open them again later.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/conversational_chat_view.png" alt="Home view with Conversational Search, suggested chats, recent chats, and Start New Chat" align="center" fullwidth="true" />

> Conversational Search homepage with suggested chats, recent chats, and Start New Chat

## Getting Started on the Homepage

When you open Conversational Search from the Desktop App home view, you have three entry points:

* **Suggested Chats for You** — Conversation starters based on recent activity. Click one to open a thread; responses include Related Timeline Events showing which memories were used.
* **Resume Recent Chats** — Cards for your latest threads. Click any card to continue with full history intact.
* **Start New Chat** — Type in the input at the bottom and press `Enter` to ask your own question.

<Callout type="tip">
  Click `Refresh suggestions` (circular icon beside the suggestions grid) to regenerate prompts from your latest activity. Click `Reveal previous chats in timeline` (panel icon on the *Resume Recent Chats* row) to open older threads in [Pieces Timeline](/products/desktop/timeline).
</Callout>

**Example questions:**

* "Why did we choose PostgreSQL over MySQL for the auth project?"
* "What was the blocker I hit last Tuesday afternoon?"
* "What did Sarah and I discuss about the API redesign in Teams?"

## While You Chat

The bottom toolbar controls how each conversation runs:

| Control | What it does |
| --- | --- |
| `+` | Attach files or folders (or drag and drop into the input) |
| `Filter By...` | Limit memories by app, time, or modality |
| Model selector | Pick a cloud model mode (Fast, Balanced, or Extra Thinking) |
| `lotus icon` | Toggle *Reflection Mode* for deeper reasoning on hard questions |
| `Send` | Send a message (`Enter` queues a follow-up while the agent is still responding) |

On active threads, the `⋮` menu at the top lets you **Pin**, **Refresh**, or **Delete** the chat. Token usage appears in the chat header so you can see input, output, reasoning, and cache totals for metered or BYOK plans.

To scope a chat to **one** Timeline Event or summary, open that item in Timeline and choose `Chat` from the three-dots menu (⋮). See [Add Context to Your Chats](/products/desktop/conversational-search/setting-context).

***

## Explore Conversational Search

<FancyCard title="Filter by Apps, Time & Modality" href="/products/desktop/conversational-search/scoping-your-prompt" colored={false}>
  Use the Filter By menu to narrow which memories the agent can use in a thread.
</FancyCard>

<FancyCard title="Add Context to Your Chats" href="/products/desktop/conversational-search/setting-context" colored={false}>
  Attach files, start chats from Timeline Events, and review source memories in the Relevant Summaries sidebar.
</FancyCard>

<FancyCard title="Choose a Model" href="/products/desktop/conversational-search/models" colored={false}>
  Switch between Fast, Balanced, and Extra Thinking modes for Claude, Gemini, and GPT.
</FancyCard>

<FancyCard title="Write Better Prompts" href="/products/desktop/conversational-search/prompting-guide" colored={false}>
  Use keywords, time ranges, app names, and follow-ups to get sharper answers.
</FancyCard>

***

If Conversational Search is not what you need, explore [Pieces Timeline](/products/desktop/timeline) to browse captured events and summaries, or [Single-Click Summaries](/products/desktop/single-click-summaries) for one-click workflow reports.
