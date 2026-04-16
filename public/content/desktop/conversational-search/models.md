---
title: Models
path: /desktop/conversational-search/models
visibility: PUBLIC
status: PUBLISHED
description: Switch between cloud and local AI models, browse the model catalog, download on-device models, and configure chat appearance.
metaTitle: Models | Conversational Search
metaDescription: Switch between cloud and local AI models in Pieces Conversational Search, browse the catalog, and download on-device models.
---

## Model Selection

Switch between cloud and local models based on your needs. Use cloud models (Claude, GPT, Gemini) for faster responses and advanced reasoning. Use local models for complete privacy and offline capability.

<Steps>
  <Step title="Open Model Selector">
    Click the `model button` in the *bottom toolbar* to open the model selector.
  </Step>

  <Step title="Choose a Model">
    You'll see Recent models you've used, Suggested models for your current task, or click `All Models` to see everything available.
  </Step>

  <Step title="Switch Models">
    When you switch models, your chat history stays intact, and new messages will use the selected model.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/using-conversational-search/model_selection_in_desktop_app.png" alt="Model selector dropdown with recent, suggested, and all models options" align="center" fullwidth="true" />

> Model selector dropdown

## LLM Runtime Modal

Click the active model control (for example the model name in the bottom toolbar) to open the **LLM runtime** modal. There you can enter API keys if needed, switch models, and open the full catalog of [local and cloud-hosted models served through Pieces](/products/core-dependencies/pieces-os#local-vs-cloud-models).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/ltm_27_rework_gifs/new_list_of_models_cloud.webp" alt="LLM runtime modal listing cloud and local models in Conversational Search" align="center" fullwidth="true" />

<Callout type="info">
  Some cloud models are available to Pieces Pro users only (for example: OpenAI GPT-5.2 Pro/GPT-5.2, Anthropic Claude 4.5 Opus, Google Gemini 3 Pro Preview). To unlock premium models, see [Pieces Pro](/paid-plans).
</Callout>

Cloud models from OpenAI, Anthropic, and Google (and others) are listed on the [Cloud Models](/products/large-language-models/cloud-models) page. For on-device options and privacy, use local models; the full catalog for the Desktop App is in [supported local and cloud models](/products/core-dependencies/local-models/supported-models).

## Browse and Download Local Models

Open the LLM runtime modal, open **All Models**, then scroll to find local models. Select a model to download it on demand through PiecesOS; once downloaded, you can run it entirely on your device.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Desktop%20App/scrolling_through_llms.gif" alt="Scrolling the All Models list to browse and download local models" align="center" fullwidth="true" />

<Callout type="tip">
  Local models run through PiecesOS on your device for privacy and offline use.
</Callout>

## Chat Appearance and Defaults

In the LLM runtime area, open the `Settings` gear to set a chat accent color and choose whether **LTM context** is on by default for **new** chats.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Settings/Aesthetics/changing_colors.png" alt="Conversational Search appearance settings with accent color and LTM default toggle" align="center" fullwidth="true" />

You can also use `cmd+shift+t` (macOS) or `ctrl+shift+t` (Windows/Linux) to toggle the Desktop App *Dark/Bright* theme.

***

For detailed model configuration and management, see [Configuration > Models](/products/desktop/configuration/models).
