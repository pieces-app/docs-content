---
title: Troubleshooting Organizations & Teams
path: /desktop/organizations-and-teams/troubleshooting
visibility: PUBLIC
status: PUBLISHED
description: Resolve common issues when working with organizations, including authentication problems and workspace loading issues.
metaTitle: Troubleshooting Organizations & Teams | Pieces Docs
metaDescription: Find solutions to common organization access issues and authentication problems.
---

## Troubleshooting Organizations & Teams

If you encounter issues when creating, accessing, or managing organizations, use this guide to resolve common problems.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/organization-settings/support_orgs.png" alt="" align="center" fullwidth="true" />

> Troubleshooting guide showing common issues and solutions

### "Loading your workspace..." Stuck Issue

If you get stuck on a "Loading your workspace..." screen when trying to access your organization, you can resolve this by forcing a logout and re-authenticating.


<Steps>
  <Step title="Navigate to Logout Page">
    In your browser, navigate directly to [portal.pieces.app/auth/logout](https://portal.pieces.app/auth/logout). This will forcefully sign you out of your current session.
  </Step>

  <Step title="Wait for Logout">
    Wait for the logout process to complete. You should be redirected to a sign-in page or see a confirmation that you've been logged out.
  </Step>

  <Step title="Sign Back In">
    Navigate to [portal.pieces.app/auth/login](https://portal.pieces.app/auth/login) and sign back in with your account credentials.
  </Step>

  <Step title="Access Your Workspace">
    After signing back in, you should be able to access your Personal Workspace and organizations without the loading issue.
  </Step>
</Steps>

### Cannot Access Organization After Creation

If you've created an organization but cannot access it:

<Steps>
  <Step title="Check Email Confirmation">
    Verify that you received a success email confirming your organization creation. Check your spam folder if you don't see it.
  </Step>

  <Step title="Verify Authentication">
    Ensure you're signed in to the correct account that was used to create the organization.
  </Step>

  <Step title="Try Logout and Login">
    Use the logout/login process described above to refresh your session.
  </Step>

  <Step title="Check Organization Dropdown">
    In your Personal Workspace, check the *organization dropdown* in the sidebar to see if your organization appears in the list.
  </Step>
</Steps>

### Cannot Accept Organization Invitation

If you're having trouble accepting an organization invitation:

<Steps>
  <Step title="Check Email Link">
    Make sure you're clicking the invitation link from the email sent by the organization owner or admin.
  </Step>

  <Step title="Verify Account">
    Ensure you're signed in to the account that matches the email address the invitation was sent to.
  </Step>

  <Step title="Try Direct Login">
    If the invitation link doesn't work, try logging in directly at [portal.pieces.app/auth/login](https://portal.pieces.app/auth/login), then check your Personal Workspace for the organization.
  </Step>

  <Step title="Contact Organization Admin">
    If you still cannot accept the invitation, contact the organization owner or admin to verify the invitation status and resend if needed.
  </Step>
</Steps>

### Cannot Use Pieces After Joining Organization

If you've joined a new organization but cannot use Pieces until you configure models:

<Steps>
  <Step title="Open Settings">
    In Pieces Desktop, navigate to *Settings* by clicking your profile picture in the top left and selecting `Settings`, or use the keyboard shortcut `⌘+,` (macOS) or `ctrl+,` (Windows/Linux).
  </Step>

  <Step title="Navigate to Models Tab">
    In the *Settings* sidebar, click on the `Models` tab or category.
  </Step>

  <Step title="Configure Models">
    Toggle all models on, or select the specific models you want to use from the available options.
  </Step>

  <Step title="Save Changes">
    Click the `Save` button to save your model selections. After saving, you should be able to use Pieces with your organization.
  </Step>
</Steps>

### Organization Not Appearing in Dropdown

If your organization doesn't appear in the organization dropdown:

<Steps>
  <Step title="Refresh Page">
    Try refreshing your browser page to reload the organization list.
  </Step>

  <Step title="Check Multiple Organizations">
    If you belong to multiple organizations, scroll through the *dropdown* list to find the one you're looking for.
  </Step>

  <Step title="Verify Membership">
    Confirm that you're still a member of the organization. Contact the organization owner or admin if you believe you should have access.
  </Step>

  <Step title="Try Logout and Login">
    Use the logout/login process to refresh your session and organization list.
  </Step>
</Steps>

### Settings Not Syncing to Desktop

If organization settings aren't appearing in your Pieces Desktop installation:

<Steps>
  <Step title="Verify Organization Membership">
    Confirm that you're a member of the organization and that settings have been configured by an Owner or Admin.
  </Step>

  <Step title="Check Desktop Connection">
    Ensure your Pieces Desktop is connected to your account and signed in.
  </Step>

  <Step title="Restart Desktop Application">
    Try restarting your Pieces Desktop application to allow settings to sync.
  </Step>

  <Step title="Check Settings Tab">
    In Pieces Desktop, check if there's an *organization settings* section that shows synced settings.
  </Step>

  <Step title="Contact Support">
    If settings still don't sync, contact support for assistance with organization settings synchronization.
  </Step>
</Steps>

## Getting Additional Help

If you continue to experience issues after trying the solutions above, here are additional resources:

* **Account Settings Documentation** - Check the [Account Settings](/products/desktop/configuration/account) documentation for account-related issues
* **Setup Guide** - Review the [Creating and Joining Organizations](/products/organizations-and-teams/creating-and-joining-organizations) guide for setup issues
* **Support Team** - [Set up a call with our support team](https://calendar.app.google/WVUDtUfNy5Vst3sH7) to get personalized assistance
* **Organization Admin** - Reach out to your organization Owner or Admin for organization-specific issues

***

## Next Steps

If you've resolved your issue, learn about [managing organizations](/products/organizations-and-teams/managing-organizations) to explore admin features, or check out [creating and joining organizations](/products/organizations-and-teams/creating-and-joining-organizations) if you're setting up a new organization.
