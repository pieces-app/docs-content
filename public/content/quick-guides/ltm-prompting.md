---
title: Long-Term Memory Prompting Guide
path: /quick-guides/ltm-prompting
visibility: PUBLIC
status: PUBLISHED
description: Learn how to query Pieces Long-Term Memory effectively using time, source, gesture, topic, and people—plus best practices and example prompts for the Workstream Activity view.
metaTitle: Long-Term Memory prompting guide | Pieces Docs
metaDescription: Learn how to query Pieces Long-Term Memory effectively. Combine time, source, topic, and more for better results. Includes example prompts and best practices.
---

## Why This Matters

With Pieces Long-Term Memory, you can query across captured memories using natural language—like asking a colleague who was there with you. The key to great results is combining a few dimensions in your questions: when, where, what, and who.

These guides show how to query LTM context using the Pieces Copilot in the Pieces Desktop App or any app with a Pieces plugin or extension.

<Callout type="alert">
  For any chat, you must activate the **LTM Context** (or Long-Term Memory Context) button in the chat interface. Without it, Pieces Copilot cannot search your Long-Term Memory—even with a well-structured query.
</Callout>

You also need [LTM-2.7 enabled](/products/core-dependencies/pieces-os/quick-menu#ltm-2-engine) in PiecesOS.

## The Five Keys to Great LTM Queries

Combine these elements in your questions for better results. You don't need all five—even one or two helps significantly.

| **Dimension** | **What to include** | **Example** |
|---------------|---------------------|-------------|
| **Time** | When did it happen? | "yesterday," "last week," "this morning" |
| **Source** | Where did it happen? (which app) | "in VS Code," "from Chrome," "in Teams" |
| **Gesture** | What were you doing? | "copying," "searching," "editing" |
| **Topic** | What project or subject? | "authentication module," "API integration" |
| **People** | Who were you working with? | "Sarah," "the security team" |

**Pro tip:** Be specific when you can. "What did I work on for the customer portal yesterday?" works better than "What was I doing?"

### Modality Filtering

You can narrow results by the type of activity:

| **Scope** | **Use when you want** | **Example phrases** |
|-----------|------------------------|----------------------|
| All sources | General summaries, themes | "everything I did," "my work today" |
| Communications | Emails, chats, meetings | "in my conversations," "in meetings" |
| Code/Technical | Terminal, IDE, code | "commands I ran," "in VS Code" |
| Capture | Clipboard, screenshots | "things I copied," "snippets I saved" |

### Query Best Practices

**Do:**
* Write naturally—ask like you'd ask a colleague
* Be specific about time when it matters ("last Tuesday" > "recently")
* Combine dimensions (time + topic + people works well)
* Mention the project or theme when you remember it

**Don't:**
* Overthink it—start simple and add details if needed
* Be too vague ("show me stuff" won't help)
* Give up after one try—small tweaks often improve results

## Guide Links

Click one of the cards below to jump to that guide.

<CardGroup cols={2}>
  <Card title="Use Cases and Example Prompts" href="/products/quick-guides/ltm-prompting/examples">
    Examples of the typical use cases we see for Pieces LTM with the kinds of prompts users ask.
  </Card>

  <Card title="Use Cases for the Pieces Workstream Activity View" href="/products/quick-guides/ltm-prompting/workstream-activity">
    A selection of popular use cases for the new Pieces Workstream Activity view.
  </Card>
</CardGroup>