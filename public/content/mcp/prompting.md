---
title: MCP Prompting
path: /mcp/prompting
visibility: PUBLIC
status: PUBLISHED
description: A straightforward guide on using different prompting techniques to retrieve and manage useful, relevant workflow context using Pieces MCP integrations.
metaTitle: Pieces MCP Prompting
metaDescription: Master effective prompting for Pieces MCP. Learn to craft precise queries that leverage context-driven AI responses, optimizing your coding workflow instantly.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/MCP/mcp.png"
---

## Prompting Guide

The `ask_pieces_ltm` tool allows you to query Pieces LTM with natural language questions to retrieve context.

Right now, we recommend setting up the Pieces MCP within [Cursor](/products/mcp/cursor) or [Visual Studio](/products/mcp/github-copilot).

### Basic Queries

You can start prompting with simple user queries, such as:

1. "What was I working on yesterday?"

2. "Ask Pieces what files I modified last week."

3. “What Google docs were I referring to this morning before my stand-up meeting?”

### Advanced Parameters

To refine your queries further, consider using parameters such as time ranges, application sources, or specific topics.

* **Time Ranges**—Try prompting using time ranges, such as “yesterday” or “April 2nd through April 6th” for more accurate, time-based questions.

* **Application Sources**—Ask Pieces to provide contextual data from specific sources, like “Stack Overflow pages I visited on Chrome” or “meeting notes from Notion” to refine source data.

* **Topics**—If your work is spread across different projects, get more accurate responses by including topic-specific keywords, like “Show recent work I’ve done on the authentication migration project”.

### Combining Parameters

Combine parameters for precise queries—like mixing topic keywords with a specific application name within the scope of a timeframe.

Here are some examples of multi-paramater prompting:

1. "What JavaScript code related to API authentication did I write in VS Code yesterday?"

2. "Find notes on database changes between Monday and Wednesday."

## Controlling Agent Responses with Pieces MCP

You can also control the agent's actions directly through your prompts, allowing Pieces MCP to first retrieve relevant data from your context, then instruct the agent to perform specific tasks or updates.

Here’s an example:

* **Prompt:***"What is the package version update that Mark asked me to make? Make the relevant update in my package manifest."*

* **Outcome:** Pieces MCP retrieves Mark's requested package version update from your context, then automatically directs the agent to apply this update to your `package.json` manifest.

## Effective Prompting Tips

Sometimes, it can be challenging to create a prompt that gets you exactly what you need.

<Callout type="tip">
  When using Pieces, especially with its large, on-device repository of personalized workflow data, it's best to use more specific prompts.
</Callout>

Use these techniques and tips to refine your prompting:

* Clearly specify *timeframes*.

* Mention relevant *applications*.

* Include *technical keywords* relevant to your query.

* Refer explicitly to *open files* when relevant.

* Ask *follow-up questions* for refined results.

<Callout type="info">
  If you want to read more information on LTM prompting, [check out this guide.](/products/quick-guides/ltm-prompting)
</Callout>

### Examples of Effective Prompts

Check out these example prompts to see how to effectively combine parameters for specific AI outputs using the Pieces MCP for your Agent.

<CardGroup cols={2}>
  <Card title="Development Context">
    * “Show examples of React Context usage."

    * "What was my last implementation of API error handling?"

    * “Have I previously optimized rendering performance in React components?”
  </Card>

  <Card title="Project History">
    * "Track the evolution of the dashboard feature."

    * "Review documented challenges with the payment system."

    * “Show the decisions made around UI updates for the onboarding flow.”
  </Card>

  <Card title="Learning Retrieval">
    * "Find recent bookmarks about Kubernetes."

    * What resources did I save recently related to Python decorators?”

    * “Show notes taken about GraphQL in March.”
  </Card>

  <Card title="Code & Collaboration">
    * “Show code review comments related to database indexing.”

    * “Did we finalize naming conventions for the latest API endpoints?”

    * “What feedback did I leave on recent pull requests?”
  </Card>
</CardGroup>