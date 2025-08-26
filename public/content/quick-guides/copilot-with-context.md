---
title: Using Pieces Copilot with Context
path: /quick-guides/copilot-with-context
visibility: PUBLIC
status: PUBLISHED
description: Use a combination of Pieces Long-Term Memory, and code context, to get help implementing a feature.
metaTitle: How to use Pieces Copilot with Context | Pieces Docs
metaDescription: Learn how to use Pieces Copilot with Long-Term Memory and code context to get AI-powered assistance in implementing features efficiently.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/quick_guides/quick_guides.png"
---

## Prerequisites

To complete this Quick Guide, you’ll need:

1. **The Pieces Desktop App** installed and actively running on your device.

2. **Long-Term Memory** enabled in the Pieces Desktop App.

3. **Optional**—Pieces installed in a Python IDE, such as the [VS Code Extension](/products/extensions-plugins/visual-studio-code), or the [JetBrains PyCharm Plugin](/products/extensions-plugins/jetbrains).

## In This Quick Guide

This Quick Guide will show you how to combine the Pieces Long-Term Memory with code context in a Pieces Copilot chat, demonstrating how you can use AI to help implement a feature in a Python app.

As a developer, a common daily task is reviewing a ticket in a tool like GitHub Issues or Jira and then implementing it in a codebase.

This often involves switching back and forth between the code and the ticket, which can affect your productivity due to constant context switching.

With Pieces, you can use the Long-Term Memory feature to remind you of the ticket details. You can then combine this with your code, allowing Pieces to guide you on implementing the issue, all from within your IDE!

### Review a GitHub Issue

The first step is to review the issue by letting Pieces capture it, and then ask the Pieces Copilot about it.

<Steps>
  <Step title="Review the GitHub Issue">
    Open the following GitHub issue in your browser. Slowly scroll through the comments on the issue, taking maybe 30 seconds or so to scroll through it.\
    \
    You can <a target="_blank" href="https://github.com/pieces-app/pieces-certification-course-content/issues/1">use this issue</a> as an example.
  </Step>

  <Step title="Ask Pieces About the Issue">
    In the Pieces Copilot, start a new chat, ensuring the Long-Term Memory (LTM) context is enabled, and use the following prompt:

    ```plaintext
    Summarize the create a sign up page issue I was just reading
    ```
  </Step>
</Steps>

Pieces will respond with a summary of the issue:

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/quick_guides/using_pieces_copilot_with_memory_context/new_media/github_issue.png" alt="" align="center" fullwidth="true" />

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

### Use the Project as Context

The next step is to add the project as context to the Pieces Copilot chat. This lets you link the project to the Long-Term Memory and ask questions about the code.

Adding the project as context to your Pieces Copilot Chat will look a little different depending on whether you’re using the Pieces Desktop App or an IDE with the respective Pieces plugin or extension installed,such as VS Code.

<Steps>
  <Step title="via Pieces Desktop App">
    From the Pieces Desktop App, select the `Manage Conversation Context `button, then select `Add Folders`.

    From the `Manage Copilot Context | Folders` dialog, select `Add Folders`.

    Select the `scifi_store` folder in the repository you cloned in the previous step.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/quick_guides/using_pieces_copilot_with_memory_context/new_media/scifi_store_selected_folder.png" alt="" align="center" fullwidth="true" />
  </Step>

  <Step title="via VS Code with Pieces Installed">
    From the **Explorer**, right-click on the pane itself (not on a file or folder), and select `Pieces`, then click `Pieces: Add to Copilot Context`.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/quick_guides/using_pieces_copilot_with_memory_context/new_media/in_ide_folder_Add_scifi.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

### Prompt Pieces Copilot

Now that Pieces has the issue from the Long-Term Memory and the project folder as context, you can ask Pieces to implement this issue.

<Steps>
  <Step title="Ask Pieces how to Implement the Issue">
    In the same Pieces Copilot chat, use this prompt (or one like it):

    ```plaintext
    How can I implement this issue in this project?
    ```
  </Step>

  <Step title="Check the Response">
    The Pieces Copilot will now reason over your project, as well as the GitHub issue you were looking at.

    The response will contain relevant instructions on how to implement this issue, such as code for the endpoint, the new page leveraging the existing app templates, and so on.

    Review these code changes along with the original codebase.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/quick_guides/using_pieces_copilot_with_memory_context/new_media/asking_to_fix.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

<Callout type="tip">
  🎉 Congratulations, you’ve completed the *Using Pieces Copilot with Context* Quick Guide! 🎉
</Callout>

## Bonus—Try One Prompt

This Quick Guide showed two prompts: one to get the details about the issue and another to learn how to implement it.

This was done in 2 stages to illustrate the information from the Pieces Long-Term Memory, but is *unnecessary*. You can do this in a single prompt!

<Steps>
  <Step title="Create a New Copilot Chat">
    Create a new Pieces Copilot Chat in the Pieces Desktop App, or in your IDE.
  </Step>

  <Step title="Add the Project Folder as Context">
    Add the `scifi_store` project as context to this new Pieces Copilot Chat.
  </Step>

  <Step title="Prompt Pieces Copilot">
    Use this single prompt when interacting with Pieces Copilot;

    ```plaintext
    How can I implement the create a sign up page issue I was just reading in this Python project?
    ```
  </Step>

  <Step title="Check the Response">
    The Pieces Copilot will now reason over your project, as well as the GitHub issue, and give you suggestions on how to implement it.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/quick_guides/using_pieces_copilot_with_memory_context/new_media/extra_example.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>