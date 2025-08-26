---
title: Pieces Copilot
path: /extensions-plugins/visual-studio-code/copilot
visibility: PUBLIC
status: PUBLISHED
description: Unlock AI-generated debugging, code comments, context-adjusted prompting,  and more with Pieces Copilot.
metaTitle: How to Use Pieces Copilot in VS Code | Pieces Docs
metaDescription: Enhance VS Code with Pieces Copilot – generate code, add comments, debug, and use AI Quick Actions with swappable LLMs seamlessly
---

## Overview

Pieces Copilot within the <a target="_blank" href="https://marketplace.visualstudio.com/items?itemName=MeshIntelligentTechnologiesInc.pieces-vscode">Pieces for VS Code Extension</a> integrates advanced AI capabilities into your coding workflow, like swappable LLMs for adding code comments, generating additional code, debugging, and more.

The Pieces Copilot allows you to generate intelligent code comments, access AI Quick Actions, and ask variable-context coding questions without leaving Visual Studio Code.

## Generative AI Conversations

Facing an issue or not sure how to tackle a coding challenge? You can [ask the Pieces Copilot specific coding questions](/products/extensions-plugins/visual-studio-code/copilot/chat) directly in VS Code using the Copilot Chat side window.

You can ask any question that doesn’t require context, such as *“What is the basic format for a JSON object?”,* or more in-depth questions where the Pieces Copilot needs context from your active code.

<Image src="https://cdn.hashnode.com/res/hashnode/image/upload/v1732736633318/f96645a1-a52f-455e-b128-84cf9d2f2c80.png" alt="" align="center" fullwidth="true" />

## Adding Conversation Context

Contextual awareness allows the Pieces Copilot to help you overcome obstacles faster by providing answers that are *actually* relevant to the current issue you’re facing and to your code.

To use this feature, include details like error messages or [file context](/products/extensions-plugins/visual-studio-code/copilot/chat#adjusting-conversation-context) for more accurate responses from the LLM conversation.

You can also [add multiple files and other items as context](/products/extensions-plugins/visual-studio-code/copilot/chat#adding-items-to-copilot-chats) to your question, giving the Pieces Copilot comprehensive information to help you troubleshoot.

<Image src="https://cdn.hashnode.com/res/hashnode/image/upload/v1732736690908/a20309cb-50cc-44ab-9866-e5ab301bb4c8.png" alt="" align="center" fullwidth="true" />

Start by right-clicking some code and selecting one of the following options from the tool menu:

* `Ask Copilot About Selection`: Includes the active selected code in the chat.

* `Ask Copilot About Active File`: Includes the entire active file with the Copilot chat for a broader range of context.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/pieces_copilot/MAIN_pieces_copilot/hover_over_ask_active_file.png" alt="" align="center" fullwidth="true" />

## Pieces Copilot Tools

Discover powerful AI-powered tools and features within the Pieces for VS Code Extension.

### Documenting Code

Easily generate insightful code comments with the Pieces for VS Code Extension. By understanding your code’s structure and function, [Pieces Copilot creates clear and useful comments](/products/extensions-plugins/visual-studio-code/copilot/documenting-code#commenting-code-selections-with-pieces-copilot) to enhance readability and simplify maintenance.\
\
To add documentation and comments to code, select the code snippet—no matter how long—then right-click, hover on `Pieces`, and click `Comment Selection with Copilot`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/pieces_copilot/MAIN_pieces_copilot/hover_over_comment.png" alt="" align="center" fullwidth="true" />

This opens the Pieces Copilot in the VS Code sidebar, where documentation is automatically generated for the highlighted snippet. You can then select `Insert at Cursor` to add the comments directly to your code.

You can also click `Pieces: Add Comments`, which is an [AI Quick Action](/products/extensions-plugins/visual-studio-code#using-ai-quick-actions) that lives above accessible functions within your code.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/pieces_copilot/MAIN_pieces_copilot/add_comments_quick_action.gif" alt="" align="center" fullwidth="true" />

<Callout type="tip">
  Use this feature to maintain consistency in documentation and simplify handoffs for collaborative projects.
</Callout>

### AI-Powered Debugging Tools

Detect and address code issues quickly with Pieces for VS Code Extension [Code Debugging feature.](/products/extensions-plugins/visual-studio-code/copilot/debugging-errors) It pinpoints problems, suggests solutions, and provides detailed context, making bug fixes faster and more intuitive.

The code debugging feature is particularly useful for tackling complex debugging tasks and ensuring code quality across projects.

Using this feature is simple—click the **lightbulb** icon near an error—marked with a red underline—to see the `Pieces: Fix` option, then click it.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/pieces_copilot/MAIN_pieces_copilot/pieces_fix_quick_action.gif" alt="" align="center" fullwidth="true" />

### Generate & Update Code

With the Pieces for VS Code extension, you can enhance your workflow with two powerful Pieces Copilot commands:

* `Modify Selection with Copilot`: [Edit or transform the selected code snippet](/products/extensions-plugins/visual-studio-code/copilot/refactoring#modifying-your-code-with-pieces-copilot) to improve readability, optimize performance, or adapt it for specific needs.

* `Explain Selection with Copilot`: [Get a clear explanation of what the selected code does](/products/extensions-plugins/visual-studio-code/copilot/chat#accessing-pieces-copilot-in-vs-code), making it easier to understand and document.

<Image src="https://cdn.hashnode.com/res/hashnode/image/upload/v1731382876801/88c397c2-519e-45a6-b15d-53afc59fba02.png?auto=compress,format&format=webp" alt="" align="left" fullwidth="true" />

## Selecting Your Pieces Copilot Runtime

Choose between [different LLMs directly within VS Code](/products/extensions-plugins/visual-studio-code/copilot/llm-settings) by accessing the sidebar and selecting your preferred model by clicking the currently-utilized LLM under `Active Model`—e.g., Claude 3.5 Sonnet, GPT-4o, etc.

Options range from lightweight models for simple queries to advanced models for in-depth analysis, as well as **local** and **cloud-based LLMs.**

This flexibility allows you to tailor Pieces Copilot to your specific development needs, whether it’s speed or accuracy.

<Image src="https://cdn.hashnode.com/res/hashnode/image/upload/v1732737435734/dce7140b-934e-42ef-bb82-9cff7bd5b620.png" alt="" align="center" fullwidth="true" />

Read more about [what LLMs are available for use](/products/extensions-plugins/visual-studio-code/configuration#supported-llms) with the Pieces for VS Code Extension.

## Pieces MCP

The new Pieces MCP enables you to utilize the LTM (Long-Term Memory) within any of your preferred IDEs, including VS Code.

The [Pieces MCP](http://google.com/link-to-the-mcp-docs-in-chat) works inline with GitHub Copilot within VS Code, allowing you to use your favorite Pieces actions directly within your VS Code or VS Code forks.

## Pieces Copilot As a Daily Driver

The Pieces Copilot is a powerful, adaptable tool that grows with you as you use it—*so use it!*

***

<AccordionGroup>
  <Accordion title="Collaborative Coding Made Easy">
    Generate detailed comments and documentation for better team collaboration and also reduce onboarding times, creating a unified coding style across teams.
  </Accordion>

  <Accordion title="Troubleshoot and Resolve Bugs Swiftly">
    Use the Pieces Copilot in VS Code to streamline the bug-fixing process. Its contextual understanding and suggested solutions make troubleshooting faster, keeping your project on course.
  </Accordion>

  <Accordion title="Quick Prototyping">
    Generate initial implementations and boilerplate code for prototypes and fast-paced projects. Ideal for hackathons, PoCs, and other time-sensitive tasks.
  </Accordion>

  <Accordion title="Skill Enhancement">
    Pieces Copilot doubles as a learning tool, helping you explore best practices, new paradigms, and advanced techniques in real-time.
  </Accordion>

  <Accordion title="Efficient Code Refactoring">
    Optimize your codebase through intelligent refactoring recommendations. The Pieces Copilot analyzes your code patterns suggests structural improvements and delivers optimizations for both performance and readability.
  </Accordion>
</AccordionGroup>

***

<a target="_blank" href="https://pieces.app/plugins/vs-code">Download the Pieces for VS Code Extension today!</a>