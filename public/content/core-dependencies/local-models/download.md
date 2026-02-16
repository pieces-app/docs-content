---
title: Download Local Models
path: /core-dependencies/local-models/download
visibility: PUBLIC
status: PUBLISHED
description: Learn how to download and manage local models for on-device AI inference with Conversational Search.
metaTitle: Download Local Models | Pieces Docs
metaDescription: Learn how to download and manage local models for on-device AI inference with Conversational Search.
---

## Downloading Local Models

Local models are an *optional* feature that enables local AI inference for Conversational Search and other AI-powered features in Pieces.

If you prefer to run LLMs on-device instead of using cloud-based AI, you can download local models directly through PiecesOS.

This guide will walk you through the download and verification process for local models across Windows, macOS, and Linux.

## Downloading Through Conversational Search

The easiest way to download and manage local models is directly from Conversational Search:

<Steps>
  <Step title="Open Conversational Search">
    Navigate to Conversational Search in the Pieces Desktop App.
  </Step>

  <Step title="Click Active Model">
    Click your active model button (e.g., `Gemini 3 Pro Preview`) in the bottom toolbar of the Conversational Search interface.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/using-conversational-search/model_selection_in_desktop_app.png" alt="" align="center" fullwidth="true" />

    > Clicking the active model button in Conversational Search to open the model dropdown
  </Step>

  <Step title="Select Manage Models">
    Click `Manage Models` from the dropdown menu that appears.
  </Step>

  <Step title="Browse Available Models">
    Scroll through the list of available models. You'll see all models organized by provider (OpenAI, Anthropic, Google, etc.), including both cloud and local models.
  </Step>

  <Step title="Enable Models">
    Toggle the switch next to any model you want to enable. Models that are already downloaded will be immediately available for use.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/configuration/models/enabling_a_model.png" alt="" align="center" fullwidth="true" />

    > Model management interface showing toggle switches to enable or disable models
  </Step>

  <Step title="Download Local Models">
    For local models you want but don't already have, click the `Download` button on the model card. Once the download completes, you can enable the model using its toggle switch.
  </Step>
</Steps>

## Downloading Through IDE Plugins

You can also download local models through any Pieces plugin or extension:

1. Open Conversational Search in your IDE plugin.

2. Click the **Active Model** or **Change Model** button.

3. Click `Manage Models` to access the full model management interface.

4. Browse the list of local models, download the ones you want, and enable them using the toggle switches.

<Callout type="info">
  Local models downloaded through any Pieces product are automatically available in all other Pieces products through PiecesOS.
</Callout>

## Managing Downloaded Models

### Delete Local Models

To free up storage space, you can delete downloaded local models directly from the model management interface:

<Steps>
  <Step title="Open Conversational Search">
    Navigate to Conversational Search in the Pieces Desktop App.
  </Step>

  <Step title="Click Active Model">
    Click your active model button (e.g., `Gemini 3 Pro Preview`) in the bottom toolbar of the Conversational Search interface.
  </Step>

  <Step title="Select Manage Models">
    Click `Manage Models` from the dropdown menu that appears.
  </Step>

  <Step title="Find Downloaded Model">
    Scroll or search through the list of available models to find the downloaded local model you want to delete. Downloaded models will have a trash icon visible on their model card.
  </Step>

  <Step title="Click Trash Icon">
    Click the trash icon on the model card to delete the downloaded model. Confirm the deletion when prompted to remove the model from your device.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/configuration/models/delete_local_model.png" alt="" align="center" fullwidth="true" />

    > Model management interface showing a downloaded model with trash icon visible for deletion
  </Step>
</Steps>

### Storage Requirements

Local models typically require:

* **Small models (2-4 GB)**: Suitable for quick queries and basic code generation
* **Medium models (4-6 GB)**: Balanced performance for most use cases
* **Large models (6-8+ GB)**: Best performance for complex queries and deep context

<Callout type="alert">
  Ensure you have sufficient storage space before downloading large models. Each model is stored only once and shared across all Pieces products.
</Callout>

## Verify Local Model Integration

Once downloaded, ensure PiecesOS can use your local models:

1. Open the **Pieces Quick Menu** from your system tray or menu bar.

2. Navigate to **ML Processing**.

3. Downloaded models will appear under **Local AI Models**.

If a model doesn't appear, try restarting PiecesOS through the Quick Menu.

## Next Steps

You can read documentation about what [local LLMs are currently available](/products/core-dependencies/local-models/supported-models) and supported by PiecesOS, or learn more about [using local vs cloud models](/products/core-dependencies/local-models#using-local-vs-cloud-models).
