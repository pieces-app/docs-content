---
title: General Settings
path: /desktop/organizations-and-teams/settings-general
visibility: PUBLIC
status: PUBLISHED
description: Configure basic organization information, contact details, domains, and SSO integration settings.
metaTitle: General Settings | Pieces Docs
metaDescription: Learn how to update organization details, configure domains, set up SSO, and manage organization deletion.
---

## General Settings

The General settings tab allows you to configure basic organization information, contact details, associated domains, SSO integration, and delete your organization. These settings control fundamental aspects of your organization's identity and access.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/new_media03-01-26/settings_overview_general_Tab.png" alt="" align="center" fullwidth="true" />

> General settings tab showing organization name, contact info, domains, and danger zone

## How to Get to General Settings

<Steps>
  <Step title="Open the Portal">
    Go to [portal.pieces.app](https://portal.pieces.app) and sign in. Select your organization from the *sidebar* dropdown if needed.
  </Step>
  <Step title="Open Settings">
    Click `Settings` in the *sidebar* navigation.
  </Step>
  <Step title="Select General Tab">
    Click the `General` tab at the top. It's the default tab when you open Settings.
  </Step>
</Steps>

## Configuring Organization Details

Update basic organization information, domains, and integration settings.

### Updating Organization Information

Modify your organization's basic details including name, contact information, and address.

<Steps>
  <Step title="Edit Organization Name">
    In the *Organization Name* field, update your organization's name as needed.
  </Step>

  <Step title="Update Contact Information">
    Update the following contact fields:
    * **Name** — Name of the primary contact person
    * **Email** — Primary email address for the organization
    * **Phone** — Contact phone number
  </Step>

  <Step title="Update Address">
    Fill in or modify the organization address fields:
    * **Country** — Select from the *dropdown*
    * **Street address** — Enter street address
    * **City** — Enter city name
    * **State** — Select state from *dropdown*
    * **ZIP Code** — Enter ZIP/postal code
  </Step>

  <Step title="Save Changes">
    A save reminder appears at the bottom of the page. Click `Save` to apply your changes.
  </Step>
</Steps>

### Configuring Associated Domains

Set up domains that are associated with your organization for automatic user assignment.

<Steps>
  <Step title="Add Domain">
    In the *Associated Domains* section, enter a domain name (e.g., `example.com`) in the *input* field.
  </Step>

  <Step title="Add Multiple Domains">
    Click the `+` button next to the *domain* field to add additional domains. You can add multiple domains to your organization.
  </Step>

  <Step title="Save Domains">
    A save reminder appears at the bottom of the page. Click `Save` to save your domain configuration.
  </Step>
</Steps>

### Setting Up SSO Integration

Configure SSO (Single Sign-On) integration using a tenant ID for *Descope* integration.

<Steps>
  <Step title="Enter Tenant ID">
    In the *Tenant ID* field, enter your *Descope* tenant ID for SSO integration (e.g., `tenant-1234567890`).
  </Step>

  <Step title="Save Configuration">
    A save reminder appears at the bottom of the page. Click `Save` to save your SSO configuration. This is optional and only needed if you're using *Descope* for SSO integration.
  </Step>
</Steps>

## Deleting an Organization

Permanently delete your organization and all associated data. This action cannot be undone.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/new_media02-27-26/deleting_org.png" alt="" align="center" fullwidth="true" />

<Callout type="alert">
  Deleting an organization is permanent and irreversible. This will permanently delete all organization data, member associations, and billing information. Subscriptions will be cancelled. Make sure you have backups of any important data before proceeding.
</Callout>

<Steps>
  <Step title="Navigate to Danger Zone">
    Scroll down to the bottom of the General settings tab to find the *Danger Zone* section, which is highlighted in red.
  </Step>

  <Step title="Read Warning">
    Review the warning message that explains what will be deleted:
    * All organization data and settings
    * All member associations
    * All billing and subscription information (subscriptions will be cancelled)
  </Step>

  <Step title="Enter Organization Name">
    Type your organization name exactly as it appears (e.g., "Pieces Test Organization") in the *confirmation* field to confirm deletion.
  </Step>

  <Step title="Delete Organization">
    Click the `Delete Organization` button. You'll be asked to confirm this action one more time before the organization is permanently deleted.
  </Step>
</Steps>

***

## Next Steps

Now that you understand general settings, explore other organization settings like [Features Settings](/products/organizations-and-teams/settings-features) to configure team-wide features, or check out [Models](/products/organizations-and-teams/settings-models) (including the API Keys tab) to configure AI providers and credentials.
