---
title: Features Settings
path: /desktop/organizations-and-teams/settings-features
visibility: PUBLIC
status: PUBLISHED
description: Toggle organization-wide features that sync to team members' Pieces Desktop and PiecesOS installations.
metaTitle: Features Settings | Pieces Docs
metaDescription: Learn how to enable and disable features that sync across your team's Pieces installations.
---

***

The Features settings tab allows you to control organization-wide feature toggles that automatically sync to all team members' Pieces Desktop and PiecesOS installations. These settings ensure consistent feature availability across your team.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/new_media03-01-26/features_tab_settings.png" alt="Features settings tab with feature toggles and processing options" align="center" fullwidth="true" />

> Features settings tab showing various feature toggles and processing options

<Callout type="info">
  All feature settings configured here automatically sync to team members' Pieces Desktop and PiecesOS installations, ensuring everyone has the same feature availability.
</Callout>

## How to Get to Features Settings

<Steps>
  <Step title="Open the Portal">
    Go to [portal.pieces.app](https://portal.pieces.app) and sign in. Select your organization from the *sidebar* dropdown if needed.
  </Step>
  <Step title="Open Settings">
    Click `Settings` in the *sidebar* navigation.
  </Step>
  <Step title="Select Features Tab">
    Click the `Features` tab at the top of the Settings page.
  </Step>
</Steps>

## Feature Categories

Configure organization-wide features organized by category. All feature settings automatically sync to team members' Pieces Desktop and PiecesOS installations. Model access, processing mode, and API keys are configured in the [Models](/products/organizations-and-teams/settings-models) section (organization management for AI).

### External Cloud

Control cloud-related operations and features for your organization.

<Steps>
  <Step title="Locate External Cloud Section">
    Find the *External Cloud* section in the *Features* tab.
  </Step>

  <Step title="Toggle External Cloud">
    Use the toggle switch next to *External Cloud* to enable or disable cloud connectivity, backup management (create, list, restore, delete), snippet sharing, and cloud allocation updates.
  </Step>

  <Step title="Save Changes">
    A save reminder appears at the bottom of the page. Click `Save` to apply. The setting will sync to all team members.
  </Step>
</Steps>

### Analytics

Configure analytics and reporting features for your organization.

<Steps>
  <Step title="Locate Analytics Section">
    Find the *Analytics* section in the *Features* tab.
  </Step>

  <Step title="Toggle Telemetry">
    Use the toggle switch next to *Telemetry* to enable or disable BigQuery and Segment analytics integrations.
  </Step>

  <Step title="Toggle Send Internal Summary Reports">
    Use the toggle switch next to *Send Internal Summary Reports* to enable or disable sending internal summary reports to user team service.
  </Step>

  <Step title="Save Changes">
    A save reminder appears at the bottom of the page. Click `Save` to apply your analytics settings.
  </Step>
</Steps>

***

## Next Steps

Now that you understand features settings, explore [Models and API Keys](/products/organizations-and-teams/settings-models) to configure AI providers and processing mode, or check out [Long Term Memory](/products/organizations-and-teams/settings-ltm-sources) to configure context capture and default models.
