---
title: API Keys Settings
path: /desktop/organizations-and-teams/settings-api-keys
visibility: PUBLIC
status: PUBLISHED
description: Configure API keys for AI services in the Models section. API Keys is a tab within Models (organization management for AI).
metaTitle: API Keys Settings | Pieces Docs
metaDescription: Learn how to configure API keys for OpenAI, Anthropic, and GCP in the API Keys tab within the Models section.
---

## API Keys Settings

The API Keys tab is one of two tabs within the *Models* section—the organization management area for AI configuration. From the API Keys tab, you configure credentials for model providers (OpenAI, Anthropic, GCP). These API keys automatically sync to all team members' Pieces Desktop and PiecesOS installations, enabling your team to use these services without individual configuration.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/new_media03-01-26/models_api_tab.png" alt="" align="center" fullwidth="true" />

> API Keys tab showing OpenAI, Anthropic, and GCP configuration sections

<Callout type="info">
  All API keys configured here automatically sync to team members' Pieces Desktop and PiecesOS installations, allowing your entire team to use these AI services with organization-managed credentials.
</Callout>

## How to Get to the API Keys Tab

<Steps>
  <Step title="Open the Portal">
    Go to [portal.pieces.app](https://portal.pieces.app) and sign in. Select your organization from the *sidebar* dropdown if needed.
  </Step>
  <Step title="Open Models">
    Click `Models` in the *sidebar* navigation.
  </Step>
  <Step title="Select API Keys Tab">
    On the Models page, click the `API Keys` tab at the top.
  </Step>
</Steps>

## Configuring API Keys

Set up API credentials for model providers. Each provider has its own configuration section: OpenAI, Anthropic (Claude), and GCP Configuration.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/new_media03-01-26/models_api_tab_Adding_apikey.png" alt="" align="center" fullwidth="true" />

### Configuring OpenAI

Set up OpenAI API credentials for your organization.

<Steps>
  <Step title="Locate OpenAI Section">
    Find the *OpenAI* section with the description "API credentials and organization settings."
  </Step>

  <Step title="Add API Key">
    Click the `+ Add API Key` button next to the OpenAI section.
  </Step>

  <Step title="Enter Credentials">
    Fill in the form with:
    * **Name** (required) — A descriptive name (e.g., "Personal Pro", "Production")
    * **API Key** (required) — Your OpenAI API key
    * **Organization ID** (optional) — For OpenAI org-specific usage
    * **Project ID** (optional) — For project-specific usage
    * **Custom API URL** (optional) — Defaults to `https://api.openai.com`
  </Step>

  <Step title="Save Configuration">
    A save reminder appears at the bottom of the page. Click `Save` to save your OpenAI credentials. The credentials will sync to all team members.
  </Step>
</Steps>

### Configuring Anthropic (Claude)

Set up Anthropic Claude API credentials for your organization.

<Steps>
  <Step title="Locate Anthropic Section">
    Find the *Anthropic (Claude)* section with the description "API credentials."
  </Step>

  <Step title="Add API Key">
    Click the `+ Add API Key` button next to the Anthropic section.
  </Step>

  <Step title="Enter Credentials">
    Fill in the Anthropic-specific credential form with your API key and any required configuration details.
  </Step>

  <Step title="Save Configuration">
    A save reminder appears at the bottom of the page. Click `Save` to save your Anthropic credentials.
  </Step>
</Steps>

### Configuring GCP

Set up GCP API keys and Vertex AI service accounts for your organization.

<Steps>
  <Step title="Locate GCP Section">
    Find the *GCP Configuration* section with the description "Manage GCP API keys and Vertex AI service accounts."
  </Step>

  <Step title="Add API Key">
    Click the `+ Add API Key` button next to the GCP Configuration section.
  </Step>

  <Step title="Enter Credentials">
    Fill in the GCP-specific credential form with your API key and service account details.
  </Step>

  <Step title="Save Configuration">
    A save reminder appears at the bottom of the page. Click `Save` to save your GCP credentials.
  </Step>
</Steps>

## Managing API Keys

View, edit, and remove existing API key configurations.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/new_media03-01-26/models_api_tab_editing_api_key.png" alt="" align="center" fullwidth="true" />

> Edit API Key form showing name, API key, and optional fields

<Steps>
  <Step title="View Configured Keys">
    Review all configured API keys in their respective sections. Each section shows "No API keys configured" if none are set up.
  </Step>

  <Step title="Edit or Remove Keys">
    Use the edit icon to modify an existing key or the delete icon to remove it. When editing, you can update the name, API key, Organization ID, Project ID, or Custom API URL.
  </Step>

  <Step title="Save Changes">
    A save reminder appears at the bottom of the page. Click `Save` to apply your changes. A warning appears if you have unsaved changes when navigating away.
  </Step>
</Steps>

***

## Next Steps

Now that you understand API keys settings, explore [Models Settings](/products/organizations-and-teams/settings-models) to configure processing mode and model access, or check out [Features Settings](/products/organizations-and-teams/settings-features) to configure team-wide feature toggles.
