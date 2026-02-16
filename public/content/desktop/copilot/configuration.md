---
title: Configure Pieces Copilot
path: /desktop/copilot/configuration
visibility: PUBLIC
status: PUBLISHED
description: Customization is key to getting the most out of any AI assistant. Read about switching between local and cloud-hosted models, adjusting the appearance of Pieces Copilot Chats, and more.
metaTitle: Adjusting Pieces Copilot | Pieces Docs
metaDescription: Learn how to enrich your Pieces Copilot chats by integrating context – like folders, file, and other saved materials – from your previous tasks and current projects.
---

# Adjusting Models & Appearance

Learn how to switch between local and cloud-hosted models, change the aesthetics and layout of your Pieces Copilot chat view, and more.

## Managing the LLM Runtime

There are dozens of local and cloud-hosted LLMs to choose from within the Pieces Desktop App—here’s how to do it.

### LLM Runtime Modal

At the bottom left of the Pieces Copilot view is the active model. By default, this is a cloud LLM. 

Clicking this button opens the **Manage Copilot LLM Runtime** modal, where you can enter your own API key or [select local and cloud-hosted LLMs served through Pieces.](/products/core-dependencies/pieces-os#local-vs-cloud-models)

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/ltm_27_rework_gifs/new_list_of_models_cloud.webp" alt="" align="center" fullwidth="true" />

<Callout type="info">
  Some cloud models are available to Pieces Pro users only (for example: OpenAI GPT-5.2 Pro/GPT-5.2, Anthropic Claude 4.5 Opus, Google Gemini 3 Pro Preview). To unlock these premium models, see [Pieces Pro](/paid-plans).
</Callout>

### Model Selection

Pieces Copilot allows you to choose between cloud-hosted models and on-device models.

Each option has its benefits:

* **Cloud LLMs:** Typically offer state-of-the-art performance and are ideal for complex queries requiring deep context. Supported providers and example models include OpenAI (GPT-5.2 Pro, GPT-5.2, GPT-5.1, GPT-5 Thinking, GPT-5, GPT-5 Fast, o4 Mini, o3 Pro, o3 Mini, o3, o1, GPT-4.1, GPT-4o, GPT-4o Mini), Anthropic (Claude 4.5 Opus, Claude 4.5 Sonnet, Claude 4.5 Haiku, Claude 4 Sonnet, Claude 3.7 Sonnet, Claude 3.5 Sonnet, Claude 3.5 Haiku), and Google (Gemini 3 Pro Preview, Gemini 3 Flash Preview, Gemini 2.5 Pro, Gemini 2.5 Flash, Gemini 2.5 Flash Lite, Gemini 2 Flash Lite). See the complete list on the [Cloud Models](/products/large-language-models/cloud-models) page.

* **On-Device LLMs:** Ensure data privacy and are optimal for offline or air-gapped environments.

You can read this documentation containing [all local and cloud-hosted LLMs available through the Pieces Desktop App.](/products/core-dependencies/local-models/supported-models)

### Resetting Conversations

In case you need a fresh start or want to clear the current context, the interface includes options (accessible via the **Chat Options** menu) to reset the conversation.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/ltm_27_rework_gifs/pieces_copilot/gif_of_resetting_conversation.gif" alt="" align="center" fullwidth="true" />

This is particularly useful when you want to switch focus or change the conversation pipeline.

### Search Functionality

To browse and download local models, click the **Active Model** button and hover over **All Models**, then scroll down to find available local models.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Desktop%20App/scrolling_through_llms.gif" alt="" align="center" fullwidth="true" />

Local models are downloaded on-demand through PiecesOS. Simply select a local model to download and use it.

***

<Callout type="tip">
  Local models run entirely on your device through PiecesOS, providing complete privacy and offline functionality without any external dependencies.
</Callout>

***

### Adjusting Chat Appearance

Within the same modal area, a `Settings Gear` icon gives you access to personalization options.

From here, you can choose a chat accent color to customize the look and feel of your Copilot interface, and enable or disable the option to enable LTM by default when starting a new chat.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Settings/Aesthetics/changing_colors.png" alt="" align="center" fullwidth="true" />

When enabling Long-Term Memory Context by default, every new chat automatically incorporates your saved long-term memory context, ensuring that your conversations are always informed by your previous work.

You can also use the keyboard shortcut `cmd+shift+t` (macOS) or `ctrl+shift+t` (Windows/Linux) to toggle the *Dark/Bright* theme for the Pieces Desktop App.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Desktop%20App/screenshot_of_copilot.png" alt="" align="center" fullwidth="true" />