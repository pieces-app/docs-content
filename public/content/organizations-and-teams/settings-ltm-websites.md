---
title: LTM Websites Settings
path: /desktop/organizations-and-teams/settings-ltm-websites
visibility: PUBLIC
status: PUBLISHED
description: Configure which websites are blocked from Long Term Memory context capture.
metaTitle: LTM Websites Settings | Pieces Docs
metaDescription: Learn how to enable LTM website management and block specific websites from Long Term Memory.
---

## LTM Websites Settings

The LTM Websites settings allow you to configure which websites are blocked from Long Term Memory. You must **enable** *Organization managed denied websites* in the General tab first; then use the *Websites* tab to add blocked sites. **Disable** the toggle to fully turn off organization-managed website blocking. These settings automatically sync to all team members' Pieces Desktop and PiecesOS installations.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/new_media03-01-26/ltm_websites.png" alt="Blocked websites list with add input and CSV upload" align="center" fullwidth="true" />

> Blocked websites list with add input and CSV upload

<Callout type="info">
  All LTM website settings configured here automatically sync to team members' Pieces Desktop and PiecesOS installations, ensuring consistent blocked website lists across your team.
</Callout>

## Accessing LTM Websites Settings

Enable the toggle in the General tab, then use the Websites tab to manage blocked sites.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/new_media03-01-26/enabling_ltm_website_and_website.png" alt="Enabling organization-managed denied websites in the General tab" align="center" fullwidth="true" />

> Enabling Organization managed denied websites in the General tab

<Steps>
  <Step title="Open Long Term Memory">
    From your organization's `Home` page, click `Long Term Memory` in the *sidebar* navigation.
  </Step>

  <Step title="Enable Organization Managed Denied Websites">
    In the *General* tab, turn on the *Organization managed denied websites* toggle in the Memory Formation section. You can also click the `Manage websites` button to jump to the Websites tab.
  </Step>

  <Step title="Open Websites Tab">
    Click the `Websites` tab at the top of the Long Term Memory page to add or manage blocked websites.
  </Step>
</Steps>

## Managing Blocked Websites

The *Blocked websites* section lists sites that will not be tracked or used for Long Term Memory. Add websites individually or upload multiple sites via CSV.

### Adding Blocked Websites Manually

Add individual websites to the blocked list.

<Steps>
  <Step title="Enter Website URL">
    In the input field (placeholder: "example.com or https://example.com"), enter the URL or domain you want to block (e.g., `example.com` or `https://example.com`).
  </Step>

  <Step title="Add Website">
    Click the `+ Add` button to add the website to your blocked list.
  </Step>

  <Step title="Save Changes">
    A save reminder appears at the bottom of the page. Click `Save` to apply. Your blocked websites list will sync to all team members.
  </Step>
</Steps>

### Bulk Uploading Blocked Websites

Upload multiple websites at once using a CSV file. Format: one website per line.

<Steps>
  <Step title="Prepare CSV File">
    Create a CSV file with one website URL or domain per line. For example:
    ```
    https://example.com
    another-site.com
    third-site.com
    ```
  </Step>

  <Step title="Upload CSV">
    Click the `Upload CSV` button or drag and drop your CSV file into the upload area.
  </Step>

  <Step title="Review and Save">
    Review the imported websites. A save reminder appears at the bottom of the page. Click `Save` to add them to your blocked list.
  </Step>
</Steps>

### Removing Blocked Websites

To allow a website for Long Term Memory again, remove it from the blocked list.

<Steps>
  <Step title="Locate Website">
    Find the website in the *Blocked websites* list.
  </Step>

  <Step title="Remove Website">
    Click the trash icon next to the website to remove it from the blocked list.
  </Step>

  <Step title="Save Changes">
    A save reminder appears at the bottom of the page. Click `Save` to apply your changes.
  </Step>
</Steps>

## Understanding Blocked Websites

When a website is added to the *Blocked websites* list, it will not be tracked or used for Long Term Memory. This helps you control what information Pieces can collect and use.

* **Privacy Control** — Prevent Pieces from accessing sensitive or private websites
* **Team Consistency** — All team members share the same blocked website list
* **Fully Disable** — Turn off the *Organization managed denied websites* toggle in the General tab to disable organization-managed website blocking entirely

***

## Next Steps

Now that you understand LTM websites settings, explore [LTM Applications](/products/organizations-and-teams/settings-ltm-sources) to control which applications are blocked or allowed for context capture, or check out [Features Settings](/products/organizations-and-teams/settings-features) to configure team-wide features.
