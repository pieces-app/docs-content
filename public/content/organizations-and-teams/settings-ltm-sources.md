---
title: Long Term Memory Settings
path: /desktop/organizations-and-teams/settings-ltm-sources
visibility: PUBLIC
status: PUBLISHED
description: Configure Long Term Memory context capture, application sources, denied websites, and default models for your organization.
metaTitle: Long Term Memory Settings | Pieces Docs
metaDescription: Learn how to configure LTM context capture, application sources, denied websites, and default models for memory processing.
---

## Long Term Memory Settings

The Long Term Memory section allows you to configure context capture settings, manage which applications and websites Pieces can access, and set default models for memory processing. These settings automatically sync to all team members' Pieces Desktop and PiecesOS installations. Long Term Memory is a top-level section in the organization sidebar.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/new_media03-01-26/ltm_applications.png" alt="" align="center" fullwidth="true" />

> Long Term Memory section showing Memory Formation toggles and Default Models

<Callout type="info">
  All Long Term Memory settings configured here automatically sync to team members' Pieces Desktop and PiecesOS installations, ensuring consistent context capture and model configuration across your team.
</Callout>

<Callout type="tip">
  To enable LTM websites or applications: turn **on** the corresponding toggle in the General tab, then use the *Applications* or *Websites* tab to manage what's blocked. To fully turn off: turn the toggle **off** in the General tab.
</Callout>

## How to Get to Long Term Memory

<Steps>
  <Step title="Open the Portal">
    Go to [portal.pieces.app](https://portal.pieces.app) and sign in. Select your organization from the *sidebar* dropdown if needed.
  </Step>
  <Step title="Open Long Term Memory">
    Click `Long Term Memory` in the *sidebar* navigation.
  </Step>
  <Step title="Choose a Tab">
    The *General* tab shows Memory Formation toggles and Default Models. Use *Applications* and *Websites* tabs to manage blocked apps and sites after enabling their toggles.
  </Step>
</Steps>

## Enabling Memory Formation Toggles

The *General* tab has three toggles that control how Pieces captures context. Turn them on or off as needed.

<Steps>
  <Step title="Enable Audio Context Capture">
    In the *General* tab, find *Audio Context Capture* and turn the toggle **on** to let Pieces process audio (meetings, conversations) for memory. Turn **off** to disable.
  </Step>
  <Step title="Enable Organization Managed Application Sources">
    Turn the *Organization managed application sources* toggle **on** to control which applications Pieces can access. When on, click `Manage applications` or open the *Applications* tab to allow or block apps. Turn **off** to disable organization-managed app control.
  </Step>
  <Step title="Enable Organization Managed Denied Websites">
    Turn the *Organization managed denied websites* toggle **on** to block specific websites from Long Term Memory. When on, click `Manage websites` or open the *Websites* tab to add blocked sites. Turn **off** to disable organization-managed website blocking.
  </Step>
  <Step title="Save">
    A save reminder appears at the bottom of the page. Click `Save` to apply. Settings sync to all team members.
  </Step>
</Steps>

## Configuring Default Models

Default models are used for memory event processing, auto-generated summaries, and audio transcription. Configure them after setting up API keys in [Models](/products/organizations-and-teams/settings-models).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/new_media03-01-26/default_models_overview_on_ltm_tab.png" alt="" align="center" fullwidth="true" />

> Default Models section on the LTM General tab showing model assignment options

<Steps>
  <Step title="Click Manage Models">
    In the *General* tab, find the *Default Models* section and click the `Manage models` button.
  </Step>
  <Step title="Assign Models">
    For each feature (Memory event processing, Auto-generated summaries, Audio transcription), choose a primary model and optional fallback. Models come from your enabled providers and API keys.
  </Step>
  <Step title="Save">
    A save reminder appears at the bottom of the page. Click `Save` to apply. Default models sync to all team members.
  </Step>
</Steps>

## Managing Application Access

When *Organization managed application sources* is enabled in the General tab, click the `Manage applications` button or select the *Applications* tab to manage which applications Pieces can access for context capture.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/new_media03-01-26/long_term_memory_tab_overview.png" alt="" align="center" fullwidth="true" />

> Available applications list showing application names, bundle IDs, and toggle switches

### Viewing Applications

The *Applications* tab shows two sections: *Blocked Applications* (apps blocked from context capture) and *Available Applications* (apps that can be allowed or blocked). Each application has a toggle to enable or disable it for context capture.

<Steps>
  <Step title="Select Applications Tab">
    Click the `Applications` tab at the top of the Long Term Memory page.
  </Step>

  <Step title="Review Application List">
    The *Available Applications* section displays applications Pieces can access. Each application shows:
    * Application name
    * Global tag (if applicable)
    * Related bundle IDs and identifiers
  </Step>

  <Step title="Search Applications">
    Use the search bar at the top with the placeholder "Search applications by name..." to quickly find specific applications.
  </Step>

  <Step title="View Application Status">
    Each application has a toggle switch. Turn it **on** to allow context capture from that application, or **off** to block it.
  </Step>
</Steps>

### Adding New Applications

Add custom applications to control access for specific tools your team uses.

<Steps>
  <Step title="Click Add Application">
    Click the `+ Add Application` button at the top of the *Applications* tab.
  </Step>

  <Step title="Enter Application Name">
    In the *Add New Application* modal, enter the application name in the *Application Name* field (e.g., "Chrome", "Safari", "Firefox").
  </Step>

  <Step title="Add Bundle IDs">
    In the *Bundle IDs* field, enter bundle identifiers to help identify specific applications (e.g., `com.example.app`). Click the `+` icon to add multiple bundle IDs.
  </Step>

  <Step title="Create Application">
    Click the `Create` button to add the application to your list. The application will appear in the *Available Applications* section.
  </Step>
</Steps>

### Enabling or Disabling Applications

Toggle access on or off for specific applications. Enable an application to allow context capture from it; disable it to block it from Long Term Memory.

<Steps>
  <Step title="Locate Application">
    Find the application in the *Blocked Applications* or *Available Applications* list.
  </Step>

  <Step title="Toggle Access">
    Use the toggle switch next to the application name. Turn **on** to allow context capture, or **off** to block it.
  </Step>

  <Step title="Save Changes">
    A save reminder appears at the bottom of the page. Click `Save` to apply. The settings will sync to all team members.
  </Step>
</Steps>

## Understanding Global vs Organization Settings

Some applications may have a *Global* tag, indicating they are system-wide applications. Organization-specific settings allow you to override or supplement global settings for your team.

* **Global Applications** - System-wide applications that affect all users
* **Organization Settings** - Your organization's specific access controls that sync to team members

***

## Next Steps

Now that you understand LTM sources settings, explore [LTM Websites Settings](/products/organizations-and-teams/settings-ltm-websites) to configure which websites Pieces is denied from accessing, or check out [Features Settings](/products/organizations-and-teams/settings-features) to configure team-wide features.
