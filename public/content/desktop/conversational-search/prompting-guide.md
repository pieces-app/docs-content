---
title: Prompting Guide
path: /desktop/conversational-search/prompting-guide
visibility: PUBLIC
status: PUBLISHED
description: Write better prompts for Conversational Search—use specific keywords, time ranges, source apps, and follow-up techniques.
metaTitle: Prompting Guide | Conversational Search
metaDescription: Learn effective prompting techniques for Pieces Conversational Search, including keywords, time ranges, app sources, and follow-up strategies.
---

## Asking Effective Questions

The more specific your questions, the better Conversational Search can find relevant memories and provide accurate answers.

## Use Specific Keywords

Include unique keywords related to what you're looking for—project names, ticket numbers, package names, or specific topics.

**Good:** "What is the status of project Aurora?"

**Bad:** "What is the status of my project?"

<Callout type="tip">
  If you can't remember specific keywords, try asking: "Give me the titles of all the project documents I've been working on last month" to find keywords for more specific prompts.
</Callout>

## Include Time Ranges

Specify when something happened to narrow down results. Conversational Search stores up to 9 months of memories.

**Examples:**
* "What decision did we make about the database schema last week?"
* "What were the plans I received in December?"
* "What was I debugging yesterday afternoon?"

## Mention Source Applications

Reference specific apps to separate similar content across different sources.

**Example:** "What did Sarah and I discuss in Teams about the deployment?"

This separates Teams conversations from emails or document comments.

## Combine Techniques

Mix keywords, time ranges, and applications for the most accurate results.

**Example:** "What is the URL for the Project Aurora document I discussed in Teams with Sarah last Thursday?"

This combines the keyword "Project Aurora," the application "Teams," the person "Sarah," and the time "last Thursday" to narrow down results precisely.

## Use Filters Instead of Prompts

If you know the exact source app or time range, use the `Sources` and `Time Ranges` filters instead of describing them in your prompt. Filters are more accurate than natural language time expressions. See [Scoping Your Prompt](/products/desktop/conversational-search/scoping-your-prompt) for details.

## Example Prompts

<CardGroup cols={2}>
  <Card title="Development Context">
    * "Show examples of React Context usage."
    * "What was my last implementation of API error handling?"
    * "Have I previously optimized rendering performance in React components?"
  </Card>

  <Card title="Project History">
    * "Track the evolution of the dashboard feature."
    * "Review documented challenges with the payment system."
    * "Show the decisions made around UI updates for the onboarding flow."
  </Card>

  <Card title="Learning Retrieval">
    * "Find recent bookmarks about Kubernetes."
    * "What resources did I save recently related to Python decorators?"
    * "Show notes taken about GraphQL in March."
  </Card>

  <Card title="Code & Collaboration">
    * "Show code review comments related to database indexing."
    * "Did we finalize naming conventions for the latest API endpoints?"
    * "What feedback did I leave on recent pull requests?"
  </Card>
</CardGroup>

<Callout type="info">
  For MCP-specific prompting patterns, see the [MCP Prompting Guide](/products/mcp/prompting) and the [LTM Prompting Guide](/products/quick-guides/ltm-prompting).
</Callout>

***

Learn how to scope your searches with filters in [Scoping Your Prompt](/products/desktop/conversational-search/scoping-your-prompt).
