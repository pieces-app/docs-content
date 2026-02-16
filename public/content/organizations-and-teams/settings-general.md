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

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/organization-settings/organization_settings.png" alt="" align="center" fullwidth="true" />

> General settings tab showing organization name, contact info, domains, and danger zone

## Accessing General Settings

Navigate to the General settings tab to configure organization details. This is the default tab when you first open Settings.

<Steps>
  <Step title="Open Settings">
    From your *organization overview* page, click `Settings` in the *sidebar* navigation.
  </Step>

  <Step title="Select General Tab">
    Click the `General` tab at the top of the *Settings* page. This is the default tab when you first open Settings.
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
    * **Organization Contact**: Name of the primary contact person
    * **Organization Email**: Primary email address for the organization
    * **Organization Phone**: Contact phone number
  </Step>

  <Step title="Update Address">
    Fill in or modify the organization address fields:
    * **Organization Country**: Select from the *dropdown*
    * **Organization Street Address**: Enter street address
    * **Organization City**: Enter city name
    * **Organization State**: Select state from *dropdown*
    * **Organization ZIP Code**: Enter ZIP/postal code
  </Step>

  <Step title="Save Changes">
    Click the `Save` button in the top right corner to save all your changes.
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
    Click `Save` to save your domain configuration. Domains associated with this organization enable automatic user assignment for users with matching email domains.
  </Step>
</Steps>

### Setting Up SSO Integration

Configure SSO (Single Sign-On) integration using a tenant ID for *Descope* integration.

<Steps>
  <Step title="Enter Tenant ID">
    In the *Tenant ID* field, enter your *Descope* tenant ID for SSO integration (e.g., `tenant-1234567890`).
  </Step>

  <Step title="Save Configuration">
    Click `Save` to save your SSO configuration. This is optional and only needed if you're using *Descope* for SSO integration.
  </Step>
</Steps>

## Deleting an Organization

Permanently delete your organization and all associated data. This action cannot be undone.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/organization-settings/deleting_org.png" alt="" align="center" fullwidth="true" />

<Callout type="alert">
  Deleting an organization is permanent and irreversible. This will permanently delete all organization data, team data, member associations, and billing information. Subscriptions will be cancelled. Make sure you have backups of any important data before proceeding.
</Callout>

<Steps>
  <Step title="Navigate to Danger Zone">
    Scroll down to the bottom of the General settings tab to find the *Danger Zone* section, which is highlighted in red.
  </Step>

  <Step title="Read Warning">
    Review the warning message that explains what will be deleted:
    * All organization data and settings
    * All team data within this organization
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

Now that you understand general settings, explore other organization settings like [Features Settings](/products/organizations-and-teams/settings-features) to configure team-wide features, or check out [API Keys Settings](/products/organizations-and-teams/settings-api-keys) to configure AI service credentials.
