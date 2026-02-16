---
title: LTM Sources Settings
path: /desktop/organizations-and-teams/settings-ltm-sources
visibility: PUBLIC
status: PUBLISHED
description: Manage which applications Pieces can access for the workstream pattern engine.
metaTitle: LTM Sources Settings | Pieces Docs
metaDescription: Learn how to control which applications Pieces can access for LTM functionality.
---

## LTM Sources Settings

The LTM Sources settings tab allows you to manage which applications Pieces can access for the workstream pattern engine. You can view available applications, add new applications, toggle access on or off, and these settings automatically sync to all team members' Pieces Desktop installations.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/organization-settings/ltm_sources.png" alt="" align="center" fullwidth="true" />

> LTM Sources settings tab showing available applications and access controls

<Callout type="info">
  All LTM source settings configured here automatically sync to team members' Pieces Desktop installations, ensuring consistent application access control across your team.
</Callout>

## Accessing LTM Sources Settings

Navigate to the LTM Sources settings tab to configure application access. These settings control which applications Pieces can access for the workstream pattern engine.

<Steps>
  <Step title="Open Settings">
    From your *organization overview* page, click `Settings` in the sidebar navigation.
  </Step>

  <Step title="Select LTM Sources Tab">
    Click the `LTM Sources` tab at the top of the *Settings* page.
  </Step>
</Steps>

## Managing Application Access

View, add, and control which applications Pieces can access for the workstream pattern engine.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/organization-settings/turning_off_ltm_settings.png" alt="" align="center" fullwidth="true" />

> Available applications list showing application names, bundle IDs, and toggle switches

### Viewing Available Applications

See all applications that Pieces can potentially access for the workstream pattern engine.

<Steps>
  <Step title="Review Application List">
    The *LTM Sources* page displays all available applications in the *Available Applications* section. Each application shows:
    * Application name
    * Global tag (if applicable)
    * Related bundle IDs and identifiers
  </Step>

  <Step title="Search Applications">
    Use the search bar at the top with the placeholder "Search applications by name..." to quickly find specific applications.
  </Step>

  <Step title="View Application Status">
    Each application has a toggle switch indicating whether Pieces has access to it (on) or is denied access (off).
  </Step>
</Steps>

### Adding New Applications

Add custom applications to control access for specific tools your team uses.

<Steps>
  <Step title="Click Add Application">
    Click the `+ Add Application` button at the top of the *LTM Sources* page.
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

### Managing Application Access

Toggle access on or off for specific applications to control what Pieces can access.

<Steps>
  <Step title="Locate Application">
    Find the application you want to configure in the *Available Applications* list.
  </Step>

  <Step title="Toggle Access">
    Use the toggle switch next to the application name to grant (on) or deny (off) Pieces access to that application for the workstream pattern engine.
  </Step>

  <Step title="Save Changes">
    Click `Save` in the top right corner to save your access changes. The settings will sync to all team members.
  </Step>
</Steps>

## Understanding Global vs Organization Settings

Some applications may have a *Global* tag, indicating they are system-wide applications. Organization-specific settings allow you to override or supplement global settings for your team.

* **Global Applications** - System-wide applications that affect all users
* **Organization Settings** - Your organization's specific access controls that sync to team members

***

## Next Steps

Now that you understand LTM sources settings, explore [LTM Websites Settings](/products/organizations-and-teams/settings-ltm-websites) to configure which websites Pieces is denied from accessing, or check out [Features Settings](/products/organizations-and-teams/settings-features) to configure team-wide features.
