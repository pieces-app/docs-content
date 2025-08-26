---
title: Pieces Copilot
path: /extensions-plugins/jetbrains/copilot
visibility: PUBLIC
status: PUBLISHED
description: With Pieces Copilot in the Pieces for JetBrains Plugin, you can add AI features to any JetBrains IDE, like generating code comments and accessing AI Quick Actions.
metaTitle: How to use Pieces Copilot with Jetbrains Plugins
metaDescription: With Pieces Copilot inside the Pieces for JetBrains Plugin, you can bring the power of AI into any of your JetBrains IDEs – like PyCharm, IntelliJ IDEA, RubyMine, and more.
---

## Generative AI Conversations

If you’re unsure how to implement a specific piece of functionality, stuck on a bug, or simply want a useful answer to something within your codebase, you can use the Pieces Copilot to receive context-aware responses to help you move forward.

The Pieces for JetBrains plugin provides several levels of conversation functionality, each of which is fully integrated with Pieces—you can enable the **Long Term Memory Engine (LTM-2.5)** for full, streamlined context across your entire workflow, or open a limited context conversation in the IDEs side view.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/MAIN_pieces_copilot/chat_window_open.png" alt="" align="center" fullwidth="true" />

## Adding Conversation Context

The Pieces Copilot lets you add specific folders or files to the conversation’s context window—like files from the codebase you’re working in—so that you always have explicit and accurate answers to pressing questions at your fingertips.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/MAIN_pieces_copilot/add_to_copilot_context_file.png" alt="" align="center" fullwidth="true" />

Start by right-clicking some code and select one of the following options from the tool menu:

* `Ask Copilot About Selection`: Includes the active selected code with the Copilot chat.

* `Ask Copilot About Active File`: Includes the entire active file with the Copilot chat for a broader range of context.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/MAIN_pieces_copilot/hovering_ask_about_selection.png" alt="" align="center" fullwidth="true" />

## Pieces Copilot Tools

Discover powerful AI-powered tools and features within the Pieces for JetBrains Plugin.

### Documenting Code

Effortlessly create meaningful code comments using the Pieces for JetBrains Plugin.

By analyzing your code's structure and purpose, [Pieces Copilot generates clear and helpful comments](/products/extensions-plugins/jetbrains/copilot/documenting-code#commenting-code-selections-with-pieces-copilot) to improve readability and facilitate maintenance.

To add documentation and comments to code, select the code snippet—no matter how long—then right-click, hover on `Pieces`, and click `Comment Selection with Copilot`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/MAIN_pieces_copilot/hovering_comment_selection.png" alt="" align="center" fullwidth="true" />

This opens the Pieces Copilot in the JetBrains sidebar, which begins adding documentation to the highlighted snippet, from which you can select the `Insert at Cursor` option to add the comments to your code.

You can also click `Pieces: Comment`, an [AI Quick Action](/products/extensions-plugins/jetbrains/copilot/chat#ai-quick-actions) that lives above accessible functions within your code.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/MAIN_pieces_copilot/adding-code-comments-quick-action.gif" alt="" align="center" fullwidth="true" />

<Callout type="info">
  Use this feature to maintain consistency in documentation and simplify handoffs for collaborative projects.
</Callout>

### Enhanced Debugging Tools

Detect and address code issues quickly with the Pieces for JetBrains Plugin [Code Debugging feature](/products/extensions-plugins/jetbrains/copilot/debugging-errors). It pinpoints problems, suggests solutions, and provides detailed context, making bug fixes faster and more intuitive.

The code debugging feature is particularly useful for tackling complex tasks and ensuring code quality across projects.

Using this feature is simple—locate the error in the code, marked by a red underline. Hover over the section to view the quick debug information provided by JetBrains. Then, click on `More Actions` and select `Pieces: Copilot Fix`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/MAIN_pieces_copilot/pieces_fix_quick_action.gif" alt="" align="center" fullwidth="true" />

### Generate & Update Code

With the Pieces for JetBrains Plugin, enhance your workflow using powerful AI Quick Actions:

* `Pieces: Explain`: [Use this AI Quick Action to get an explanation and summary of the function](/products/extensions-plugins/jetbrains/copilot/chat#via-ai-quick-actions), making it easier to understand and document.

* `Pieces: Comment`: [This AI Quick Action adds intelligent code comments](/products/extensions-plugins/jetbrains/copilot/documenting-code#via-pieces-comment) to the selected function based on the context of the code itself to ensure accuracy.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/MAIN_pieces_copilot/comment%20inline.png" alt="" align="center" fullwidth="true" />

## Selecting Your Pieces Copilot Runtime

Choose between [different LLMs directly within JetBrains](/products/extensions-plugins/jetbrains/copilot/llm-settings) by accessing the sidebar and selecting your preferred model by clicking the currently utilized LLM under `Active Model` (Claude 3.5 Sonnet).

Options range from lightweight models for simple queries to advanced models for in-depth analysis, as well as **local** and **cloud-based LLMs.**

This flexibility allows you to tailor Pieces Copilot to your specific development needs, whether speed or accuracy.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/MAIN_pieces_copilot/changing_runtime.png" alt="" align="center" fullwidth="true" />

Read more about [what LLMs are available ](/products/extensions-plugins/jetbrains/configuration#supported-llms)with the Pieces for JetBrains Plugin.

## Pieces Copilot As a Daily Driver

The Pieces Copilot is a powerful, adaptable tool that grows with you as you use it—*so use it!*

***

<AccordionGroup>
  <Accordion title="Collaborative Coding Made Easy">
    Generate detailed comments and documentation for better team collaboration and also reduce onboarding times, creating a unified coding style across teams.
  </Accordion>

  <Accordion title="Troubleshoot and Resolve Bugs Swiftly">
    Use the Pieces Copilot in JetBrains to streamline the bug-fixing process. Its contextual understanding and suggested solutions make troubleshooting faster, keeping your project on course.
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

<a target="_blank" href="http://plugins.jetbrains.com/plugin/17328-pieces">Download the Pieces for JetBrains Plugin today!</a>