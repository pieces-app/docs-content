---
title: Pieces Copilot
path: /extensions-plugins/visual-studio/copilot
visibility: PUBLIC
status: PUBLISHED
description: The Pieces Copilot in the Pieces for Visual Studio Extension boosts coding with AI features like interchangeable LLMs, code generation, and debugging, AI Quick Actions in Visual Studio, and more.
metaTitle: How to use Pieces Copilot for Visual Studio | Pieces Docs
metaDescription: Use Pieces Copilot inside Visual Studio to generate code, debug, and improve productivity with AI-powered coding assistance.
---

## Generative AI Conversations

Facing an issue or not sure how to tackle a coding challenge? You can [ask the Pieces Copilot specific coding questions](/products/extensions-plugins/visual-studio/copilot/chat) directly in Visual Studio using Pieces Copilot in the `Solution Explorer`.

You can ask any question that doesn’t require context, such as *“What is the basic format for a JSON object?”,* or more in-depth questions where the Pieces Copilot needs context from your active code.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/pieces_copilot_main/copilot_chat_in_active_code_file.png" alt="" align="center" fullwidth="true" />

## Adding Conversation Context

Contextual awareness enables the Pieces Copilot to help you solve problems more quickly by providing answers that are relevant to the issue you're dealing with and your code.

You can add context by selecting specific lines of code or entire files directly from your active file.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/pieces_copilot_main/hovering_on_ask_copilot_about_selection_command_right_click_menu.png" alt="" align="center" fullwidth="true" />

Start by right-clicking some selected code and selecting one of the following options from the tool menu:

* `Ask Copilot About Selection`: Includes the active selected code in the conversation.

* `Ask Copilot About Active File`: Includes the entire active file with the conversation for a broader range of context.

To use this feature, include details like error messages or [file context](/products/extensions-plugins/visual-studio/copilot/chat#adding-context-to-copilot-chats) for more accurate responses from the LLM conversation.

You can also add multiple files and other items as context to your prompt, giving the Pieces Copilot comprehensive information to assist you in troubleshooting.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/pieces_copilot_main/adding_context_to_chat.png" alt="" align="center" fullwidth="true" />

## Pieces Copilot Tools

Explore the powerful AI tools and features in the Pieces for Visual Studio Extension.

### Documenting Code

Easily generate insightful code comments with the Pieces for Visual Studio Extension. Pieces Copilot understands your code’s structure and function, [creating clear and useful comments to improve readability and simplify maintenance](/products/extensions-plugins/visual-studio/copilot/documenting-code#commenting-code-selections-with-pieces-copilot).

To add documentation and comments to your code, select the code snippet, right-click, hover over `Pieces`, and click `Comment Selection with Copilot`.

This opens Pieces Copilot in the Visual Studio sidebar, adding documentation to the highlighted snippet. You can then select one of the `Insert at Cursor` or `Accept Changes` options to add the comments to your code.

You can also click `Pieces > Comment`, an AI Quick Action that lives above accessible functions within your code.

<Callout type="info">
  Use this feature to maintain consistency in documentation and simplify handoffs for collaborative projects.
</Callout>

### Generate & Update Code

With the Pieces for Visual Studio extension, you can easily change code to adapt to new requirements or insert quick fixes with two powerful Pieces Copilot commands:

* `Modify Selection with Copilot`: [Edit or transform the selected code snippet](/products/extensions-plugins/visual-studio/copilot/refactoring#modifying-your-code-with-pieces-copilot) to improve readability, optimize performance, or adapt it for specific needs.

* `Explain Selection with Copilot`: [Get a clear explanation of what the selected code does](/products/extensions-plugins/visual-studio/copilot/chat#accessing-pieces-copilot-in-vs-code), making it easier to understand and document.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/pieces_copilot_main/saving_snippet_keybind.gif" alt="" align="center" fullwidth="true" />

## Selecting Your Pieces Copilot Runtime

Choose between [different LLMs directly within Visual Studio](/products/extensions-plugins/visual-studio/copilot/llm-settings) by accessing the sidebar and selecting your preferred model by clicking the currently utilized LLM under `Active Model`.

Options include lightweight models for simple queries, advanced models for in-depth analysis, and **local** and **cloud-based LLMs.**

This flexibility lets you customize Pieces Copilot to fit your development needs, focusing on either speed or accuracy.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/pieces_copilot_main/selecting_LLM_runtime.png" alt="" align="center" fullwidth="true" />

Read more about [what LLMs are available ](/products/extensions-plugins/visual-studio/configuration#supported-llms)within the Pieces for Visual Studio Extension.

## Pieces Copilot As a Daily Driver

The Pieces Copilot is a powerful, adaptable tool that grows with you as you use it—*so use it!*

***

<AccordionGroup>
  <Accordion title="Collaborative Coding Made Easy">
    Generate detailed comments and documentation to improve team collaboration and reduce onboarding times, ensuring a consistent team coding style.
  </Accordion>

  <Accordion title="Troubleshoot and Resolve Bugs Swiftly">
    Use the Pieces Copilot in Visual Studio to speed up bug fixing. Its contextual understanding and suggested solutions make troubleshooting quicker, keeping your project on track.
  </Accordion>

  <Accordion title="Quick Prototyping">
    Generate initial implementations and boilerplate code for prototypes and fast-paced projects. Perfect for hackathons, PoCs, and other time-sensitive tasks.
  </Accordion>

  <Accordion title="Skill Enhancement">
    Pieces Copilot is also a learning tool. It helps you discover best practices, new paradigms, and advanced techniques in real-time.
  </Accordion>

  <Accordion title="Efficient Code Refactoring">
    Optimize your codebase with innovative refactoring suggestions. Pieces Copilot analyzes your code patterns, recommends structural improvements, and provides optimizations for better performance and readability.
  </Accordion>
</AccordionGroup>

***

<a target="_blank" href="https://marketplace.visualstudio.com/items?itemName=MeshIntelligentTechnologiesInc.PiecesVisualStudio">Download the Pieces for Visual Studio Extension today!</a>