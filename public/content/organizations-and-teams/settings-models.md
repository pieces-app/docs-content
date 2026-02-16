---
title: Models Settings
path: /desktop/organizations-and-teams/settings-models
visibility: PUBLIC
status: PUBLISHED
description: Control which AI models are available to your organization and sync to team members' installations.
metaTitle: Models Settings | Pieces Docs
metaDescription: Learn how to manage model access and control which AI models your team can use in Pieces.
---

## Models Settings

The Models settings tab allows you to control which AI models are available to your organization. You can toggle entire model providers on or off, manage individual models, and these settings automatically sync to all team members' Pieces Desktop and PiecesOS installations.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/organization-settings/models_settings.png" alt="" align="center" fullwidth="true" />

<Callout type="info">
  All model settings configured here automatically sync to team members' Pieces Desktop and PiecesOS installations, ensuring everyone has access to the same models.
</Callout>

## Accessing Models Settings

Navigate to the Models settings tab to configure model access.

<Steps>
  <Step title="Open Settings">
    From your *organization overview* page, click `Settings` in the sidebar navigation.
  </Step>

  <Step title="Select Models Tab">
    Click the `Models` tab at the top of the *Settings* page.
  </Step>
</Steps>

## Managing Model Access

Control which AI models are available to your organization by toggling providers and managing individual models.

### Toggling Model Providers

Enable or disable entire model providers for your organization.

<Steps>
  <Step title="Locate Model Provider">
    Find the model provider you want to configure (e.g., ANTHROPIC, GOOGLE, OPENAI).
  </Step>

  <Step title="Review Provider Description">
    Read the description that explains these models will use the Pieces default configurations.
  </Step>

  <Step title="Toggle Provider">
    Use the toggle switch next to the provider name to turn the entire provider on or off. When off, none of that provider's models will be available to your organization.
  </Step>

  <Step title="Save Changes">
    Click `Save` in the top right corner to save your changes.
  </Step>
</Steps>

### Managing Individual Models

View and understand individual models within each provider.

<Steps>
  <Step title="View Model List">
    Under each enabled provider, you'll see a list of available models with their descriptions and labels.
  </Step>

  <Step title="Understand Model Labels">
    Models are labeled with their characteristics:
    * **Accurate** (green badge): Models optimized for accuracy and detailed analysis
    * **Fast** (blue badge): Models optimized for speed and efficiency
  </Step>

  <Step title="Review Model Descriptions">
    Each model includes a description explaining its capabilities, context window, and use cases.
  </Step>
</Steps>

### Using Toggle All Functions

Quickly enable or disable all models at once.

<Steps>
  <Step title="Locate Toggle Buttons">
    Find the `Toggle All On` and `Toggle All Off` buttons at the top of the *Model Access* section.
  </Step>

  <Step title="Toggle All On">
    Click `Toggle All On` to enable all model providers and their models at once.
  </Step>

  <Step title="Toggle All Off">
    Click `Toggle All Off` to disable all model providers and their models at once.
  </Step>

  <Step title="Save Changes">
    Click `Save` to apply your changes after using the toggle all functions.
  </Step>
</Steps>

## Example Model Providers

Common model providers you may see include:

* **ANTHROPIC**: Claude models (4.5 Opus, 4.5 Sonnet, 4.5 Haiku, 4 Sonnet, 3.7 Sonnet, 3.5 Sonnet, 3.5 Haiku)
* **GOOGLE**: Gemini models (3 Pro Preview, 3 Flash Preview, 2.5 Pro, 2.5 Flash, 2.5 Flash Lite, 2 Flash Lite)
* **OPENAI**: GPT models (5.2 Pro, 5.2, 5.1, GPT-5 Thinking, GPT-5, GPT-5 Fast, o4 Mini, o3 Pro, o3 Mini, o3, o1, GPT-4.1, GPT-4o, GPT-4o Mini)

Each provider's models use the Pieces default configurations and sync to your team members' installations.

***

## Next Steps

Now that you understand models settings, explore [LTM Sources Settings](/products/organizations-and-teams/settings-ltm-sources) to control which applications Pieces can access, or check out [API Keys Settings](/products/organizations-and-teams/settings-api-keys) to configure AI service credentials.
