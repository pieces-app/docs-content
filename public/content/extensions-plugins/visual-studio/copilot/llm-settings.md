---
title: Switching LLMs
path: /extensions-plugins/visual-studio/copilot/llm-settings
visibility: PUBLIC
status: PUBLISHED
description: The Pieces for Visual Studio Extension supports various LLMs, both cloud-based and local, providing flexibility for different workflows.
metaTitle: How to Switch LLMs in Pieces Copilot for Visual Studio
metaDescription: Learn how to switch between multiple LLMs in the Pieces for Visual Studio Plugin to enhance AI-driven development.
---

## Switching LLMs

Currently, the Pieces for Visual Studio Extension supports over 54 cloud and local models, [which you can find here.](/products/large-language-models)

## How To Configure Your LLM Runtime

Switching your LLM model in the Pieces for Visual Studio Extension is simple. You can select the model that best suits your needs.

How to change your LLM:

<Steps>
  <Step title="Open the Copilot Chat View">
    Open the Copilot Chat view by clicking the `Pieces Copilot Icon` in the sidebar.
  </Step>

  <Step title="Locate the Active Model">
    Locate the **Active Model** in the bottom-left corner of the view where the current model (e.g., *GPT-4o Mini*) is displayed.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/llm_settings/changing_active_model.gif" alt="" align="center" fullwidth="true" />
  </Step>

  <Step title="View the Models">
    Click on `Change Model` to open the **Manage Copilot Runtime** modal.
  </Step>

  <Step title="Choose your Desired Model">
    Browse the list of local and cloud models, and select your preferred model.
  </Step>
</Steps>

You can use local models for on-device AI inference, which you can [read more about here](/products/core-dependencies/local-models).

From here, you can browse and select from various available models, such as the local and cloud-based models listed [in the table at the top of this page.](/products/extensions-plugins/visual-studio/configuration#supported-llms)

<Callout type="tip">
  Local models run entirely on your device through PiecesOS, ensuring complete privacy and offline functionality without any external dependencies.
</Callout>

Once you’ve chosen a new model, the switch is instant, allowing you to continue your work seamlessly with the selected model's capabilities—*no need to restart or refresh anything.*

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/llm_settings/showing_llms.gif" alt="" align="center" fullwidth="true" />

***

Cloud-hosted models offer access to the latest AI capabilities, while on-device models ensure offline functionality, making Pieces Copilot adaptable to your specific workflow and environment.

***