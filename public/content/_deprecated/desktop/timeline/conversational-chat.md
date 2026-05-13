---
title: Conversational Chat
path: /desktop/timeline/conversational-chat
visibility: PUBLIC
status: PUBLISHED
description: Ask questions about your workflow with context-aware assistance powered by LTM-2.7 in Conversational Chat.
metaTitle: Conversational Chat | Timeline
metaDescription: Ask questions about your workflow with context-aware assistance powered by LTM-2.7 in Conversational Chat.
---

## Conversational Chat

**Conversational Chat** is your conversational interface for asking questions about your workflow. Powered by the [Long-Term Memory (LTM-2.7)](/products/core-dependencies/pieces-os#ltm-27) Engine with access to up to 9 months of captured context, it searches your actual memories—conversations, documents, commits, and decisions.

Unlike generic AI, responses reference your specific work. Related Roll-Ups cards below responses reveal which memories were used.

<Image src="https://www.jacksonsquareshopping.co.uk/wp-content/uploads/2016/12/placeholder-1920x1080-copy.png" alt="Conversational Chat with suggested chats, recent chats, and Start New Chat" align="center" fullwidth="true" />

> Conversational Chat section showing suggested chats, recent chats, and Start New Chat

## Getting Started

### Suggested Chats

Personalized chat suggestions appear under *Suggested Chats for You*, generated from your recent workflow activity. Click any suggestion to instantly start that conversation.

Suggestions update dynamically based on your captured context. Click the refresh icon next to the header for new suggestions.

### Resume Recent Chats

Below the suggested chats, *Resume Recent Chats* shows your most recent conversations with their titles and timestamps. Click any card to reopen that conversation with its full history and context intact.

### Starting a Chat

Click `Start New Chat` or type directly in the input field. Type naturally: "What did I work on yesterday?" or "Find that Slack conversation about API changes." Press Enter to send.

<Image src="https://www.jacksonsquareshopping.co.uk/wp-content/uploads/2016/12/placeholder-1920x1080-copy.png" alt="Chat interface opening after a suggested chat or Start New Chat" align="center" fullwidth="true" />

> Clicking a suggested chat or Start New Chat, showing the chat interface opening

## How It Works

### Context-Aware Responses

When you ask a question, Conversational Chat searches your captured memories for relevant context. It references your specific activities, not generic AI knowledge, providing personalized answers based on your actual work.

It can recall specific conversations, documents, decisions, and problems you've encountered.

### Related Roll-Ups

Below each response, "Related Workstream Activities" cards appear showing which specific memories were used in the answer.

Each card is clickable and takes you to full LTM Roll-Up details, providing transparency into where information came from.

<Image src="https://www.jacksonsquareshopping.co.uk/wp-content/uploads/2016/12/placeholder-1920x1080-copy.png" alt="Response with Related Workstream Activities cards linking to roll-ups" align="center" fullwidth="true" />

> Chat response with 2-3 Related Roll-Up cards below, showing user clicking a card to view full roll-up

## Choosing Your AI Model

### Model Selector (Bottom-Left Corner)

The model selector shows **Recent models** and **Suggested models** sections.

* **Cloud models** (Claude 4.1 Opus, Claude 4 Sonnet, etc.)—Faster responses and advanced reasoning.
* **Local models** (o3, o1, GPT-4, etc.)—Complete privacy and work offline.

Click any model name to switch. Use the "All Models" button to see the complete list.

### Additional Controls (Bottom Toolbar)

* **Sources**—Control which data sources are used.
* **Time Ranges**—Filter memories by time period.
* **Reflection Mode**—Toggle the lotus icon to enable the agent to reflect on its reasoning and self-correct in real time.

<Image src="https://www.jacksonsquareshopping.co.uk/wp-content/uploads/2016/12/placeholder-1920x1080-copy.png" alt="Model selector with Recent and Suggested models and Sources, Time Ranges, Reflection Mode" align="center" fullwidth="true" />

> Model selector dropdown showing Recent and Suggested sections with available models, plus bottom toolbar with Sources, Time Ranges, and Reflection Mode toggle

## Asking Effective Questions

**Questions that work well:**

* **Time-based**: "What did I work on yesterday afternoon?", "Summarize my week"
* **Topic-specific**: "Find conversations about the API redesign"
* **Decision recall**: "Why did we decide to use PostgreSQL?"
* **Reference finding**: "Find that link about React performance"
* **Summary requests**: "Give me a recap of client feedback"

**Making questions more specific:** Include timeframes ("yesterday", "last week", "between Monday and Wednesday") and mention projects, people, or topics ("work on the dashboard", "conversations with Tom"). Use follow-up questions—the chat maintains conversation context.

## Managing Chats

Chats auto-save and appear in the [Timeline Activities](/products/desktop/timeline/timeline-activities) sidebar, listed chronologically with other workflow activities.

Click previous chats in the sidebar to continue conversations. Use `Start New Chat` for fresh conversations on new topics.

## Tips & Best Practices

* Start with suggested chats to discover what works, then adapt them to your needs.
* Be specific with timeframes: "last Tuesday" works better than "recently".
* Check Related Roll-Ups to verify information sources and access full context.
* Use follow-up questions to dig deeper—context is maintained within conversations.
* Try different models for different tasks (local for privacy, cloud for speed).
* Remember: Conversational Chat only knows about your captured workflow—not work done before you started using Pieces or in applications where LTM is disabled.
