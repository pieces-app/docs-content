---
title: Features Settings
path: /desktop/organizations-and-teams/settings-features
visibility: PUBLIC
status: PUBLISHED
description: Toggle organization-wide features that sync to team members' Pieces Desktop and PiecesOS installations.
metaTitle: Features Settings | Pieces Docs
metaDescription: Learn how to enable and disable features that sync across your team's Pieces installations.
---

## Features Settings

The Features settings tab allows you to control organization-wide feature toggles that automatically sync to all team members' Pieces Desktop and PiecesOS installations. These settings ensure consistent feature availability across your team.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/organization-settings/features_settings.png" alt="" align="center" fullwidth="true" />

> Features settings tab showing various feature toggles and processing options

<Callout type="info">
  All feature settings configured here automatically sync to team members' Pieces Desktop and PiecesOS installations, ensuring everyone has the same feature availability.
</Callout>

## Accessing Features Settings

Navigate to the Features settings tab to configure organization-wide feature toggles. These settings control what features are available to your entire team.

<Steps>
  <Step title="Open Settings">
    From your *organization overview* page, click `Settings` in the sidebar navigation.
  </Step>

  <Step title="Select Features Tab">
    Click the `Features` tab at the top of the *Settings* page.
  </Step>
</Steps>

## Feature Categories

Configure organization-wide features organized by category. All feature settings automatically sync to team members' Pieces Desktop and PiecesOS installations.

### External Cloud Features

Control cloud-related operations and features for your organization.

<Steps>
  <Step title="Locate External Cloud Section">
    Find the *External Cloud* section in the *Features settings* page.
  </Step>

  <Step title="Toggle External Cloud">
    Use the toggle switch next to *External Cloud* to enable or disable cloud connectivity, backup management (create, list, restore, delete), snippet sharing, and cloud allocation updates.
  </Step>

  <Step title="Save Changes">
    Click `Save` in the top right corner to save your changes. The setting will sync to all team members.
  </Step>
</Steps>

### Analytics Features

Configure analytics and reporting features for your organization.

<Steps>
  <Step title="Locate Analytics Section">
    Find the *Analytics* section in the *Features settings* page.
  </Step>

  <Step title="Toggle Telemetry">
    Use the toggle switch next to *Telemetry* to enable or disable BigQuery and Segment analytics integrations.
  </Step>

  <Step title="Toggle Internal Summary Reports">
    Use the toggle switch next to *Send Internal Summary Reports* to enable or disable sending internal summary reports to user team service.
  </Step>

  <Step title="Save Changes">
    Click `Save` to apply your analytics settings.
  </Step>
</Steps>

### External Provider Features

Control external provider and processing features for your organization.

<Steps>
  <Step title="Locate External Provider Section">
    Find the *External Provider* section in the *Features settings* page.
  </Step>

  <Step title="Toggle Customized Allowed Models">
    Use the toggle switch next to *Customized Allowed Models* to enable or disable customizing allowed models with an allow-list.
  </Step>

  <Step title="Toggle Denied Workstream Pattern Engine Sources">
    Use the toggle switch next to *Denied Workstream Pattern Engine Sources* to enable or disable denying specific workstream pattern engine sources.
  </Step>

  <Step title="Toggle Denied Workstream Pattern Engine Websites">
    Use the toggle switch next to *Denied Workstream Pattern Engine Websites* to enable or disable denying specific websites for workstream pattern engine.
  </Step>

  <Step title="Save Changes">
    Click `Save` to apply your external provider settings.
  </Step>
</Steps>

### Processing Capabilities

Configure processing capabilities for your organization.

<Steps>
  <Step title="Locate Processing Section">
    Find the *Processing* section in the *Features settings* page.
  </Step>

  <Step title="Select Processing Mode">
    Use the *dropdown* menu to select processing capabilities:
    * **LOCAL**: Process everything locally
    * **BLENDED**: Use a combination of local and cloud processing
  </Step>

  <Step title="Toggle Processing">
    Use the toggle switch to enable or disable processing capabilities based on your selected mode.
  </Step>

  <Step title="Save Changes">
    Click `Save` to apply your processing configuration.
  </Step>
</Steps>

***

## Next Steps

Now that you understand features settings, explore [API Keys Settings](/products/organizations-and-teams/settings-api-keys) to configure AI service credentials, or check out [Models Settings](/products/organizations-and-teams/settings-models) to control which AI models are available to your organization.
