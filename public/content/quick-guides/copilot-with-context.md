---
title: Using Conversational Search with Context
path: /quick-guides/copilot-with-context
visibility: PUBLIC
status: PUBLISHED
description: Use a combination of Pieces Long-Term Memory, and code context, to get help implementing a feature.
metaTitle: How to use Conversational Search with Context | Pieces Docs
metaDescription: Learn how to use Conversational Search with Long-Term Memory and code context to get AI-powered assistance in implementing features efficiently.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/quick_guides/quick_guides.png"
---

## Prerequisites

To complete this Quick Guide, you’ll need:

1. **The Pieces Desktop App** installed and actively running on your device.

2. **Long-Term Memory** enabled in the Pieces Desktop App.

3. **Optional**—Pieces connected in a Python IDE via MCP, such as [Visual Studio Code](/products/mcp/vs-code) or [JetBrains IDEs](/products/mcp/jetbrains-ides) (including PyCharm).

## In This Quick Guide

This Quick Guide shows how to combine **Long-Term Memory** with **Conversational Search**—including scoping a chat to a specific captured memory using **`Chat`** on a Timeline summary—so you can get AI help implementing a feature in a Python app.

As a developer, a common daily task is reviewing a ticket in a tool like GitHub Issues or Jira and then implementing it in a codebase.

This often involves switching back and forth between the code and the ticket, which can affect your productivity due to constant context switching.

With Pieces, Long-Term Memory captures the ticket as you read it. After you work in your project, Pieces can use those **captured memories**—and you can open **Conversational Search** scoped to the right **summary** from Timeline using the **`Chat`** action on the three-dots menu.

### Review a GitHub Issue

The first step is to review the issue by letting Pieces capture it, and then ask Conversational Search about it.

<Steps>
  <Step title="Review the GitHub Issue">
    Open the following GitHub issue in your browser. Slowly scroll through the comments on the issue, taking maybe 30 seconds or so to scroll through it.\
    \
    You can <a target="_blank" href="https://github.com/pieces-app/pieces-certification-course-content/issues/1">use this issue</a> as an example.
  </Step>

  <Step title="Ask Pieces About the Issue">
    In Conversational Search, start a new chat, ensuring the Long-Term Memory (LTM) context is enabled, and use the following prompt:

    ```plaintext
    Summarize the create a sign up page issue I was just reading
    ```
  </Step>
</Steps>

Pieces will respond with a summary of the issue:

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/quick_guides/using_pieces_copilot_with_memory_context/new_media/github_issue.png" alt="Conversational Search summarizing a GitHub issue using LTM context" align="center" fullwidth="true" />

### Clone the Project

This issue refers to a sci-fi store—a small web application written in Python and Flask for an upcoming retail store that sells themed sci-fi toys.

<Steps>
  <Step title="Clone the Project Repo">
    <a target="_blank" href="https://github.com/pieces-app/pieces-certification-course-content">Clone this GitHub repository.</a>
  </Step>

  <Step title="Navigate to the Sci-Fi Store folder">
    Inside the repo is a folder called `scifi_store`.

    If you use an IDE like VS Code or JetBrains PyCharm, open this folder in that IDE.
  </Step>
</Steps>

### Tie the project to Conversational Search (Timeline Chat)

You **cannot** attach a project folder or individual files directly to Conversational Search. Instead, **LTM** must **capture** your work in `scifi_store`, then you **scope** a chat to the summary or event that holds that context.

<Steps>
  <Step title="Work in the project so LTM captures it">
    With **Long-Term Memory** enabled, spend a few minutes in your IDE inside `scifi_store`—open files, scroll relevant modules, or run the app—so Pieces records useful workflow context.
  </Step>

  <Step title="Open Timeline and find a relevant summary">
    In the Pieces Desktop App, open [Pieces Timeline](/products/desktop/timeline). Look for a recent **roll-up** or **summary** that reflects that coding session (for example activity involving your editor and that repo).
  </Step>

  <Step title="Choose Chat on the three-dots menu">
    Open that item in the main panel. Click the **three-dots menu** (⋮) on the event header and select **`Chat`**. Conversational Search opens with that memory in scope.

    For more detail, see [Chat from a summary](/products/desktop/timeline/event-actions#chat-from-a-summary).
  </Step>
</Steps>

### Prompt Conversational Search

With the GitHub issue in LTM and a **scoped** chat tied to a summary that includes your project activity, you can ask Pieces how to implement the issue.

<Steps>
  <Step title="Ask Pieces how to Implement the Issue">
    In the same Conversational Search chat, use this prompt (or one like it):

    ```plaintext
    How can I implement this issue in this project?
    ```
  </Step>

  <Step title="Check the Response">
    The Conversational Search will use **Long-Term Memory**—including the issue you read and the workflow captured from `scifi_store` inside the scoped summary—to propose implementation steps.

    The response may include concrete suggestions such as code for an endpoint, a new page using existing templates, and so on.

    Review these code changes along with the original codebase.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/quick_guides/using_pieces_copilot_with_memory_context/new_media/asking_to_fix.png" alt="Conversational Search reasoning over the project and GitHub issue" align="center" fullwidth="true" />
  </Step>
</Steps>

<Callout type="tip">
  🎉 Congratulations, you’ve completed the *Using Conversational Search with Context* Quick Guide! 🎉
</Callout>

## Bonus—Try One Prompt

This Quick Guide showed two prompts: one to get the details about the issue and another to learn how to implement it.

This was done in 2 stages to illustrate the information from the Pieces Long-Term Memory, but is *unnecessary*. You can do this in a single prompt!

<Steps>
  <Step title="Create a New Conversational Search chat">
    Start from home or your IDE, or open **`Chat`** from a Timeline summary that already contains both the issue and recent work in `scifi_store`.
  </Step>

  <Step title="Scope with Timeline Chat if needed">
    If you need one focused memory in scope, use **`Chat`** on the relevant summary’s three-dots menu—see [Chat from a summary](/products/desktop/timeline/event-actions#chat-from-a-summary).
  </Step>

  <Step title="Prompt Conversational Search">
    Use this single prompt when interacting with Conversational Search;

    ```plaintext
    How can I implement the create a sign up page issue I was just reading in this Python project?
    ```
  </Step>

  <Step title="Check the Response">
    The assistant uses your **Long-Term Memory** (issue + captured IDE activity) to suggest how to implement the ticket—especially if you used **Chat** on a summary that already bundles that context.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/quick_guides/using_pieces_copilot_with_memory_context/new_media/extra_example.png" alt="Conversational Search implementing an issue with a single prompt" align="center" fullwidth="true" />
  </Step>
</Steps>