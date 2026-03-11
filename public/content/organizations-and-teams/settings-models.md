---
title: Models Settings
path: /desktop/organizations-and-teams/settings-models
visibility: PUBLIC
status: PUBLISHED
description: Organization management for AI—control model access, processing mode, and API keys. Models is the parent section; API Keys is a tab within it.
metaTitle: Models Settings | Pieces Docs
metaDescription: Learn how to manage model access, processing mode, and API keys in the Models section (organization management for AI).
---

## Models Settings

The Models section is the organization management area for AI. From here you control which models are available, enable or disable providers (Google, OpenAI, etc.), configure processing mode, and set up API keys. All settings sync to team members' Pieces Desktop and PiecesOS.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/new_media03-01-26/models_overview.png" alt="" align="center" fullwidth="true" />

> Models page showing provider sections (Google, OpenAI) with model lists and toggles

<Callout type="info">
  All model settings configured here automatically sync to team members' Pieces Desktop and PiecesOS installations.
</Callout>

## How to Get to the Models Page

<Steps>
  <Step title="Open the Portal">
    Go to [portal.pieces.app](https://portal.pieces.app) and sign in. Or from Pieces Desktop, click your `User Profile` → `Settings` → `Account` to reach your workspace.
  </Step>
  <Step title="Select Your Organization">
    In the *sidebar*, click the *organization dropdown* at the top and select your organization.
  </Step>
  <Step title="Open Models">
    Click `Models` in the *sidebar* navigation. The Models page opens with the *Models* tab selected. Use the `API Keys` tab to add provider credentials.
  </Step>
</Steps>

## Enabling the Customized Model Allow-List

By default, all models from enabled providers are available. To control which providers and models members can use, you must first enable the customized model allow-list. **The provider toggles (Google, OpenAI, etc.) are only active when the allow-list is enabled.**

<Steps>
  <Step title="Enable Customized Model Allow-List">
    On the Models page, find the *Customized Model Allow-List* toggle and turn it **on**.
  </Step>
  <Step title="Save">
    A save reminder appears at the bottom of the page. Click `Save` to apply. The provider sections below become active so you can enable or disable providers and select specific models.
  </Step>
</Steps>

## Enabling or Disabling a Provider (Google, OpenAI, etc.)

<Callout type="info">
  The customized model allow-list must be enabled for provider toggles to be active. See the section above.
</Callout>

Each provider (Google, OpenAI, Anthropic, etc.) has a toggle at the top of its section. Turn it on to make that provider's models available; turn it off to disable them.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/new_media03-01-26/models_show_models.png" alt="" align="center" fullwidth="true" />

> Provider sections with on/off toggles for Google, OpenAI, and other providers

<Steps>
  <Step title="Enable Allow-List First">
    Ensure the *Customized Model Allow-List* toggle is **on** near the top of the Models page. Provider toggles are inactive until the allow-list is enabled.
  </Step>
  <Step title="Locate the Provider Section">
    On the Models page, scroll to the provider you want to change (e.g., *Google*, *OpenAI*).
  </Step>
  <Step title="Toggle the Provider">
    Use the toggle switch at the top right of the provider section. Turn it **on** to enable that provider's models for your organization, or **off** to disable them.
  </Step>
  <Step title="Save">
    A save reminder appears at the bottom of the page. Click `Save` to apply. Changes sync to all team members.
  </Step>
</Steps>

## Selecting Allowed Models

With the allow-list and provider toggles configured, choose which specific models members can use.

<Steps>
  <Step title="Scroll to Provider Sections">
    On the Models page, scroll to each enabled provider (e.g., *Google*, *OpenAI*).
  </Step>
  <Step title="Select Models">
    Use the checkboxes or controls next to each model to include or exclude it. Only models you explicitly allow will be available to members.
  </Step>
  <Step title="Save">
    A save reminder appears at the bottom of the page. Click `Save` to apply.
  </Step>
</Steps>

## Setting Organization-Wide Processing Mode

Control whether your organization uses local, cloud, or blended processing for AI features.

<Steps>
  <Step title="Enable Organization Managed Processing Mode">
    On the Models page, find the *Organization Managed Processing Mode* toggle and turn it **on**.
  </Step>
  <Step title="Choose Processing Mode">
    Use the *Organization-Wide Processing Mode* dropdown to select:
    * **BLENDED** — Mix of local and cloud (recommended)
    * **Local** — Process locally only (limits features)
  </Step>
  <Step title="Save">
    A save reminder appears at the bottom of the page. Click `Save` to apply. The chosen mode applies to all organization members.
  </Step>
</Steps>

<Callout type="tip">
  Blended mode is recommended. Local-only mode severely limits AI features.
</Callout>

## Adding API Keys for Providers

To use models from OpenAI, Anthropic, or GCP, you need to add API keys. Switch to the API Keys tab within Models.

<Steps>
  <Step title="Open API Keys Tab">
    On the Models page, click the `API Keys` tab at the top.
  </Step>
  <Step title="Add a Key">
    Find the provider section (OpenAI, Anthropic, GCP) and click `+ Add API Key`. Enter your credentials and click `Save`.
  </Step>
  <Step title="Return to Models">
    Switch back to the *Models* tab to enable that provider and choose which models to use.
  </Step>
</Steps>

For full API key instructions, see [API Keys Settings](/products/organizations-and-teams/settings-api-keys).

***

## Next Steps

Add credentials in [API Keys](/products/organizations-and-teams/settings-api-keys), or configure [Long Term Memory](/products/organizations-and-teams/settings-ltm-sources) for context capture and default models.
