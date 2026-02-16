---
title: LTM Websites Settings
path: /desktop/organizations-and-teams/settings-ltm-websites
visibility: PUBLIC
status: PUBLISHED
description: Configure which websites Pieces is denied from accessing for the workstream pattern engine.
metaTitle: LTM Websites Settings | Pieces Docs
metaDescription: Learn how to manage denied websites and control Pieces' access to specific URLs.
---

## LTM Websites Settings

The LTM Websites settings tab allows you to configure which websites Pieces is denied from accessing for the workstream pattern engine. You can add individual URLs or bulk upload via CSV, and these settings automatically sync to all team members' Pieces Desktop installations.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/organization-settings/ltm_websites.png" alt="" align="center" fullwidth="true" />

> LTM Websites settings tab showing denied websites list and upload options

<Callout type="info">
  All LTM website settings configured here automatically sync to team members' Pieces Desktop installations, ensuring consistent website access control across your team.
</Callout>

## Accessing LTM Websites Settings

Navigate to the LTM Websites settings tab to configure denied websites. These settings control which websites Pieces is denied from accessing for the workstream pattern engine.

<Steps>
  <Step title="Open Settings">
    From your *organization overview* page, click `Settings` in the sidebar navigation.
  </Step>

  <Step title="Select LTM Websites Tab">
    Click the `LTM Websites` tab at the top of the *Settings* page.
  </Step>
</Steps>

## Managing Denied Websites

Add websites to the denied list to prevent Pieces from accessing them. You can add websites individually or upload multiple sites via CSV.

### Adding Denied Websites Manually

Add individual websites to the denied list to prevent Pieces from accessing them.

<Steps>
  <Step title="Enter Website URL">
    In the *website input* field, enter the URL of the website you want to deny access to (e.g., `https://example.com` or `example.com`).
  </Step>

  <Step title="Add Website">
    Click the `add` button or press Enter to add the website to your *denied* list.
  </Step>

  <Step title="Save Changes">
    Click `Save` in the top right corner to save your *denied websites* list.
  </Step>
</Steps>

### Bulk Uploading Denied Websites

Upload multiple websites at once using a CSV file for efficient management.

<Steps>
  <Step title="Prepare CSV File">
    Create a CSV file with one website URL per line. For example:
    ```
    https://example.com
    https://another-site.com
    https://third-site.com
    ```
  </Step>

  <Step title="Upload CSV">
    Click the `Upload CSV` button or drag and drop your CSV file into the *upload* area on the *LTM Websites settings* page.
  </Step>

  <Step title="Review Imported Websites">
    Review the list of websites that were imported from your CSV file.
  </Step>

  <Step title="Save Changes">
    Click `Save` to save all imported websites to your *denied* list.
  </Step>
</Steps>

### Managing Denied Websites List

View and manage your current list of denied websites.

<Steps>
  <Step title="View Denied List">
    Review all websites currently in your *denied* list on the *LTM Websites settings* page.
  </Step>

  <Step title="Remove Websites">
    Use the remove option (typically an X icon or delete button) next to each website to remove it from the *denied* list if needed.
  </Step>

  <Step title="Save Changes">
    Click `Save` to apply any changes to your *denied websites* list.
  </Step>
</Steps>

## Understanding Website Denial

When a website is added to the *denied* list, Pieces will not access data from that website for the workstream pattern engine. This helps you control what information Pieces can collect and use.

* **Privacy Control** - Prevent Pieces from accessing sensitive or private websites
* **Team Consistency** - Ensure all team members have the same website access restrictions
* **Automatic Sync** - Settings automatically apply to all team members' installations

***

## Next Steps

Now that you understand LTM websites settings, explore [LTM Sources Settings](/products/organizations-and-teams/settings-ltm-sources) to control which applications Pieces can access, or check out [Features Settings](/products/organizations-and-teams/settings-features) to configure team-wide features.
