---
title: Configure Pieces Copilot
path: /desktop/copilot/configuration
visibility: PUBLIC
status: PUBLISHED
description: Customization is key to getting the most out of any AI assistant. Read about switching between local and cloud-hosted models, adjusting the appearance of Pieces Copilot Chats, and more.
metaTitle: Adjusting Pieces Copilot | Pieces Docs
metaDescription: Learn how to enrich your Pieces Copilot chats by integrating context – like folders, file, and other saved materials – from your previous tasks and current projects.
---

## Adjusting Models & Appearance

Learn how to switch between local and cloud-hosted models, change the aesthetics and layout of your Pieces Copilot chat view, and more.

## Managing the LLM Runtime

There are dozens of local and cloud-hosted LLMs to choose from within the Pieces Desktop App—here’s how to do it.

### LLM Runtime Modal

At the bottom left of the Pieces Copilot view is the active model—by default you’ll see *GPTo3-Mini.*

Clicking this button opens the **Manage Copilot LLM Runtime** modal, where you can enter your own API key or [select local and cloud-hosted LLMs served through Pieces.](/products/core-dependencies/ollama#using-local-vs-cloud-models)

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Settings/Pieces%20Copilot/screenshot_of_llms.png" alt="" align="center" fullwidth="true" />

### Model Selection

Pieces Copilot allows you to choose between cloud-hosted models and on-device models.

Each option has its benefits:

* **Cloud LLMs:** Typically offer state-of-the-art performance and are ideal for complex queries requiring deep context.

* **On-Device LLMs:** Ensure data privacy and are optimal for offline or air-gapped environments.

You can read this documentation containing [all local and cloud-hosted LLMs served through the Pieces Desktop App.](/products/core-dependencies/ollama/supported-models)

### Resetting Conversations

In case you need a fresh start or want to clear the current context, the interface includes options (accessible via the **Chat Options** menu) to reset the conversation.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Desktop%20App/quick%20options%20(3%20dots).png" alt="" align="center" fullwidth="true" />

This is particularly useful when you want to switch focus or change the conversation pipeline.

### Search Functionality

A search bar labeled *Find Cloud LLMs* lets you browse available cloud-based models—then, switching to *On-Device,* you can search through the list of local models available with the [optional Ollama client.](/products/core-dependencies/ollama)

***

<Callout type="alert">
  Ollama is required to use local LLMs with Pieces software.

  If you don’t have it installed, that’s okay—you can download and install it through the Pieces Desktop App by clicking on the `Active Model` button.
</Callout>

***

To switch between the *Cloud* and *On-Device* model list, click the slider next to the search bar.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Desktop%20App/scrolling_through_llms.gif" alt="" align="center" fullwidth="true" />

Once toggled, the search bar updates to *Find On-Device LLMs* and shows a message either prompting you to install Ollama or indicating that Ollama is installed and ready, along with its version number.

***

<Callout type="tip">
  While Ollama is required for on-device generative AI, you do not need it to use the Long-Term Memory Engine.

  This distinction ensures that you can benefit from local Long-Term Memory features even if you choose not to use on-device LLMs.
</Callout>

***

### Adjusting Chat Appearance

Within the same modal area, a `Settings Gear` icon gives you access to personalization options.

From here, you can choose a chat accent color to customize the look and feel of your Copilot interface, and enable or disable the option to enable LTM by default when starting a new chat.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Settings/Aesthetics/changing_colors.png" alt="" align="center" fullwidth="true" />

When enabling Long-Term Memory Context by default, every new chat automatically incorporates your saved long-term memory context, ensuring that your conversations are always informed by your previous work.

You can also use the keyboard shortcut `cmd+shift+t` (macOS) or `ctrl+shift+t` (Windows/Linux) to toggle the *Dark/Bright* theme for the Pieces Desktop App.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Desktop%20App/screenshot_of_copilot.png" alt="" align="center" fullwidth="true" />