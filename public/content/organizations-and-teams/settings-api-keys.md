---
title: API Keys Settings
path: /desktop/organizations-and-teams/settings-api-keys
visibility: PUBLIC
status: PUBLISHED
description: Configure API keys for AI services that sync to team members' Pieces Desktop and PiecesOS installations.
metaTitle: API Keys Settings | Pieces Docs
metaDescription: Learn how to configure API keys for OpenAI, Gemini, Claude, Bedrock, and Azure OpenAI that your team can use.
---

## API Keys Settings

The API Keys settings tab allows you to configure API credentials for various AI services. These API keys automatically sync to all team members' Pieces Desktop and PiecesOS installations, enabling your team to use these services without individual configuration.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/organization-settings/api_keys_overview.png" alt="" align="center" fullwidth="true" />

> API Keys settings tab showing configuration options for different AI platforms

<Callout type="info">
  All API keys configured here automatically sync to team members' Pieces Desktop and PiecesOS installations, allowing your entire team to use these AI services with organization-managed credentials.
</Callout>

## Accessing API Keys Settings

Navigate to the API Keys settings tab to configure AI service credentials. These credentials enable your team to use various AI services without individual configuration.

<Steps>
  <Step title="Open Settings">
    From your *organization overview* page, click `Settings` in the sidebar navigation.
  </Step>

  <Step title="Select API Keys Tab">
    Click the `API Keys` tab at the top of the *Settings* page.
  </Step>
</Steps>

## Configuring API Keys

Set up API credentials for various AI services. Each service has its own configuration section.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/organization-settings/api_keys_add_kehy.png" alt="" align="center" fullwidth="true" />

### Configuring OpenAI

Set up OpenAI API credentials for your organization.

<Steps>
  <Step title="Locate OpenAI Configuration">
    Find the *OpenAI Configuration* section in the *API Keys settings* page.
  </Step>

  <Step title="Add Credential">
    Click the `+ Add Credential` button next to the *OpenAI Configuration* section.
  </Step>

  <Step title="Enter Credentials">
    Fill in the OpenAI-specific *credential* form with your API key and any required configuration details.
  </Step>

  <Step title="Save Configuration">
    Click `Save` to save your OpenAI credentials. The credentials will sync to all team members.
  </Step>
</Steps>

### Configuring Gemini

Set up Google Gemini API credentials for your organization.

<Steps>
  <Step title="Locate Gemini Configuration">
    Find the *Gemini Configuration* section in the *API Keys settings* page.
  </Step>

  <Step title="Add Credential">
    Click the `+ Add Credential` button next to the *Gemini Configuration* section.
  </Step>

  <Step title="Enter Credentials">
    Fill in the Gemini-specific *credential* form with your API key and any required configuration details.
  </Step>

  <Step title="Save Configuration">
    Click `Save` to save your Gemini credentials.
  </Step>
</Steps>

### Configuring Claude

Set up Anthropic Claude API credentials for your organization.

<Steps>
  <Step title="Locate Claude Configuration">
    Find the *Claude Configuration* section in the *API Keys settings* page.
  </Step>

  <Step title="Add Credential">
    Click the `+ Add Credential` button next to the *Claude Configuration* section.
  </Step>

  <Step title="Enter Credentials">
    Fill in the Claude-specific *credential* form with your API key and any required configuration details.
  </Step>

  <Step title="Save Configuration">
    Click `Save` to save your Claude credentials.
  </Step>
</Steps>

### Configuring Bedrock

Set up AWS Bedrock access credentials and API keys for your organization.

<Steps>
  <Step title="Locate Bedrock Configuration">
    Find the *Bedrock Access Credentials* and *Bedrock API Keys* sections in the *API Keys settings* page.
  </Step>

  <Step title="Add Access Credentials">
    Click the `+ Add Credentials` button next to *Bedrock Access Credentials* to configure AWS access credentials for Bedrock service.
  </Step>

  <Step title="Add API Keys">
    Click the `+ Add API Key` button next to *Bedrock API Keys* to configure API keys for Bedrock service.
  </Step>

  <Step title="Enter Credentials">
    Fill in the Bedrock-specific *credential* forms with your AWS access credentials and API keys.
  </Step>

  <Step title="Save Configuration">
    Click `Save` to save your Bedrock credentials.
  </Step>
</Steps>

### Configuring Azure OpenAI

Set up Azure OpenAI API configuration for your organization.

<Steps>
  <Step title="Locate Azure Configuration">
    Find the *Manage Azure OpenAI API configuration* section in the *API Keys settings* page.
  </Step>

  <Step title="Add Configuration">
    Click the `+ Add Configuration` button next to the *Azure OpenAI* section.
  </Step>

  <Step title="Enter Configuration">
    Fill in the Azure OpenAI-specific *configuration* form with your Azure endpoint, API key, and deployment details.
  </Step>

  <Step title="Save Configuration">
    Click `Save` to save your Azure OpenAI configuration.
  </Step>
</Steps>

## Managing API Keys

View and manage existing API key configurations.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/organization-settings/modifying_keys.png" alt="" align="center" fullwidth="true" />

<Steps>
  <Step title="View Configured Keys">
    Review all configured API keys in their respective *sections*. Each section shows "No credentials configured" or "No API keys configured" if none are set up.
  </Step>

  <Step title="Edit or Remove Keys">
    Use the options available for each configured credential to edit or remove API keys as needed.
  </Step>

  <Step title="Save All Changes">
    Click `Save` in the top right corner to save any changes made to API key configurations.
  </Step>
</Steps>

***

## Next Steps

Now that you understand API keys settings, explore [Models Settings](/products/organizations-and-teams/settings-models) to control which AI models are available to your organization, or check out [Features Settings](/products/organizations-and-teams/settings-features) to configure team-wide features.
