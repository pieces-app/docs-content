---
title: JetBrains Plugin
path: /extensions-plugins/jetbrains
visibility: PUBLIC
status: PUBLISHED
description: The Pieces for JetBrains Plugin integrates Pieces suite features into JetBrains IDEs, making tools easily accessible.
metaTitle: Using Pieces for JetBrains Plugin | Pieces Docs
metaDescription: The Pieces for JetBrains Plugin enhances your development experience by seamlessly integrating the best features from the Pieces suite directly into JetBrains IDEs.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/plugins_extensions/jetbrains.png" alt="" align="center" fullwidth="true" />

***

## Pieces for JetBrains Plugin

The <a target="_blank" href="https://plugins.jetbrains.com/plugin/17328-pieces">Pieces for JetBrains Plugin</a> enhances your development experience by seamlessly integrating the best features from the Pieces suite directly into JetBrains IDEs, making your favorite tools readily accessible within your workspace.

It provides developers with powerful tools for **managing code snippets, debugging, and refactoring** within their familiar development environment.

* [Pieces Copilot:](/products/extensions-plugins/jetbrains/copilot) Users can start generative AI conversations and add files and folders as context to get the solutions they need, including out-of-IDE context with the optional Long-Term Memory Engine (LTM-2.7).

* [Pieces Drive:](/products/extensions-plugins/jetbrains/drive) Effortlessly save, locate, and share frequently used code snippets, making it easier to organize your work, quickly access essential pieces of code, and collaborate effectively with others.

- [AI Quick Actions:](/products/extensions-plugins/jetbrains/copilot/chat#ai-quick-actions) Fully integrated and Pieces-powered AI Quick Actions tools are built right into your code, making it even easier to access Pieces Copilot explanation and documentation features.

<CardGroup cols={2}>
  <Card title="Getting Started" image="/assets/icons/jetbrains.png">
    Follow [these instructions](/products/extensions-plugins/jetbrains/get-started) to download and install the <a target="_blank" href="https://plugins.jetbrains.com/plugin/17328-pieces">Pieces for JetBrains plugin.</a>
  </Card>

  <Card title="Support" image="/assets/icons/platform_logos/pieces_logo.png">
    Explore [troubleshooting options](/products/extensions-plugins/jetbrains/troubleshooting), navigate to our [support page](/products/support), or <a target="_blank" href="https://calendar.google.com/calendar/u/0/appointments/schedules/AcZssZ22WJ2Htd2wRMJhueCNYc0xbFBFCAN-khijcuoXACd_Uux3wIhgZeGkzDRcqD3teamAI-CwCHpr">directly book a call</a> with our engineers.
  </Card>
</CardGroup>

<guides-overview-card />

<Callout type="tip">
  All media (e.g., GIFs, screenshots) in this documentation were captured in **PyCharm CE.**
</Callout>

The Pieces for JetBrains Plugin verifies against the JetBrains IntelliJ Ultimate IDE, but works across the entire JetBrains suite of IDEs.

The minimum version required for the Pieces for JetBrains Plugin to work in your JetBrains IDE is **2023.1.**

If you’re not quite sure what version your JetBrains IDE is, [you can click here to find out how to check it.](/products/extensions-plugins/jetbrains/configuration#checking-your-jetbrains-ide-version)

This plugin is currently available for use in any JetBrains IDE, such as:

* <a target="_blank" href="https://www.jetbrains.com/idea/">IntelliJ IDEA</a>

* <a target="_blank" href="https://www.jetbrains.com/webstorm/">WebStorm</a>

* <a target="_blank" href="https://www.jetbrains.com/phpstorm/">PhpStorm</a>

* <a target="_blank" href="https://www.jetbrains.com/pycharm/">PyCharm</a>

* <a target="_blank" href="https://www.jetbrains.com/clion/">CLion</a>

* <a target="_blank" href="https://www.jetbrains.com/go/">GoLand</a>

* <a target="_blank" href="https://www.jetbrains.com/rider/">Rider</a>

* <a target="_blank" href="https://www.jetbrains.com/ruby/">RubyMine</a>

* <a target="_blank" href="https://www.jetbrains.com/datagrip/">DataGrip</a>

* <a target="_blank" href="https://www.jetbrains.com/objc/">AppCode</a>

* <a target="_blank" href="https://developer.android.com/studio">Android Studio</a>

The Pieces for JetBrains plugin provides developers with **two pillars of functionality**:

### AI Assistance with Pieces Copilot

Pieces Copilot offers [AI-assisted features](/products/extensions-plugins/jetbrains/copilot) like starting contextualized [generative AI conversations](/products/extensions-plugins/jetbrains/copilot/chat), <a target="_blank" href="/products/extensions-plugins/jetbrains/copilot/documenting-code">adding code comments</a>, and <a target="_blank" href="/products/extensions-plugins/jetbrains/troubleshooting">troubleshooting code</a>.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/jetbrains_plugin/right_click_hover_over_save_to_pieces.png" alt="" align="center" fullwidth="true" />

### Material Management with Pieces Drive

Pieces Drive enables you to [save, edit, search, and share useful code snippets](/products/extensions-plugins/jetbrains/drive) to boost your workflow productivity and streamline collaboration with others.

These features let developers store their favorite code in a personal, easy-to-access library. They can quickly review past work, find related authors and links with the extra details saved with each piece, and more.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/jetbrains_plugin/pieces_drive_right_click.png" alt="" align="center" fullwidth="true" />

## Using Pieces Copilot

You can perform **several decisive** **actions** with the Pieces Copilot inside of your JetBrains IDE, like starting a conversation directly inside the editor with your LLM of choice about a specific code snippet, fragment, folder, or terminal output.

The **Ask Copilot** feature is the backbone of the Pieces Copilot experience.

Pieces recently rolled out its new **AI Quick Actions** feature—similar to VS Code’s Codelens—which allows for select quick actions powered by Pieces Copilot, namely `Pieces: Explain` and `Pieces: Comment`.

<Callout type="tip">
  The Quick Action tools—`Pieces: Explain` and `Pieces: Comment`—are above the function nearest to your cursor.
</Callout>

Using either AI Quick Actions triggers the Pieces Copilot conversation window, where you can find the output from the LLM of your choice.

These AI Quick Action tools live above certain pieces of code, like functions, so you always have easy access to them.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/jetbrains_plugin/lightbulb_fix.png" alt="" align="center" fullwidth="true" />

## Managing Code Snippets

When you save code to your personal repository, Pieces **automatically enriches the snippet** with AI-generated tags, titles, related authors and links, and a description.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/jetbrains_plugin/right_click_menu.png" alt="" align="center" fullwidth="true" />

You can save code snippets by right-clicking a selection of code and choosing the `Save Current Selection to Pieces` option from the pop-up window.

Alternatively, right-click and hover over the `Pieces` item to access several other snippet-related functions.

Other material management actions available in this menu include:

***

| **Action**                                | **Purpose**                                                                                                                                                                                                                                                                                             |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Save Current Selection / File to Pieces` | Right-click a selected block of code or your entire active file and [save it to your Pieces Drive with AI-enriched metadata](/products/extensions-plugins/jetbrains/drive/save-snippets#whats-stored-when-you-save-a-snippet), ensuring easy access to frequently used snippets. |
| `Save File to Pieces`                     | Save an entire file to Pieces Drive for future reference.                                                                                                                                                                                                                                               |
| `Ask Copilot About Selection`             | Ask Pieces Copilot to generate suggestions or explain the selection with a query.                                                                                                                                                                                                                       |
| `Modify Selection with Copilot`           | Adjust and refine selected code using AI suggestions.                                                                                                                                                                                                                                                   |
| `Comment Selection with Copilot`          | Auto-generate comments for the selected code snippet using AI.                                                                                                                                                                                                                                          |
| `Explain Selection with Copilot`          | Receive an explanation for the code using your chosen LLM through Pieces Copilot.                                                                                                                                                                                                                       |
| `Share via Pieces Link`                   | Generate a shareable link for your snippet, allowing collaboration even with those who don’t have a Pieces account.                                                                                                                                                                                     |
| `Search Pieces Drive`                     | Search for previously saved snippets in Pieces.                                                                                                                                                                                                                                                         |
| `Pieces Quick Search`                     | Quickly find and retrieve relevant snippets saved in Pieces.                                                                                                                                                                                                                                            |

***

### **Referencing & Reusing**

The <a target="_blank" href="https://plugins.jetbrains.com/plugin/17328-pieces">Pieces for JetBrains Plugin</a> provides robust search tools to help you quickly find and access your saved snippets.

You can easily find saved snippets in your JetBrains IDE by double-tapping the shift key and selecting the `Pieces` window.

Enter a query, and any snippet you’ve saved that matches the query will be returned to the drop-down list.

Once you’ve located the snippet you want, pressing `return` (macOS), `enter` (Windows/Linux), or clicking the snippet title will open it inside your JetBrains IDE.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/jetbrains_plugin/searching_for_snippet.gif" alt="" align="center" fullwidth="true" />

***

## Download the Plugin

Follow the [installation instructions](/products/extensions-plugins/jetbrains/get-started) to get started with the Pieces for JetBrains Plugin.