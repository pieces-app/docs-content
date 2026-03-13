---
title: Onboarding Users
path: /enterprise/onboarding
visibility: PUBLIC
status: PUBLISHED
description: Step-by-step guide for admins to onboard their team and for members to get set up with Pieces.
metaTitle: Onboarding Users | Enterprise | Pieces Docs
metaDescription: Standalone enterprise onboarding guide—invite team members, get Pieces installed, and start collaborating.
---

## Onboarding Users

This guide walks admins through getting their team set up with Pieces and walks team members through accepting their invitation and installing Pieces. Share this page directly with your team to get everyone onboarded.

## Setting Up Your Team

As an organization owner or admin, you'll invite team members, ensure you have enough seats, and share resources to help your team get started.

### Creating Your Organization

If you haven't created your organization yet, you'll need to do that first. The process involves choosing a name, selecting seats, picking a subscription plan, and completing checkout.

<Steps>
  <Step title="Start the Creation Flow">
    Click your `User Profile` in the top left of Pieces Desktop, then click `Settings` and select `Account`. Scroll down to the *Organizations & Teams* section and click `+ Create an organization`. You can also start directly at [portal.pieces.app](https://portal.pieces.app).
  </Step>
  <Step title="Configure Your Organization">
    Enter your organization name, choose the number of seats, and select a subscription plan (Enterprise Seat Yearly, Quarterly, or Monthly). Complete checkout to create your organization.
  </Step>
</Steps>

For the full creation walkthrough, see [Creating and Joining Organizations](/products/organizations-and-teams/creating-and-joining-organizations).

### Inviting Team Members

Once your organization is set up, invite your team by email. Each invited member needs an available seat in your subscription.

<Steps>
  <Step title="Open the Invite Modal">
    Click `Members` in the *sidebar*, then click the `Invite people` button in the top right corner.
  </Step>
  <Step title="Add Members and Assign Roles">
    Enter email addresses and select a role for each member:
    * **Owner** — Full control including organization deletion
    * **Admin** — Full access except organization deletion
    * **Write** — Can create and edit resources
    * **Read** — View-only access
  </Step>
  <Step title="Send Invitations">
    Click `Send Invites & Finish` to send the invitations. Each member will receive an email with instructions to join.
  </Step>
</Steps>

<Callout type="tip">
  For large teams, you can bulk invite members by uploading a CSV file with the format `email,role` (one member per line). Click the `Upload CSV` option in the invite modal.
</Callout>

### Sharing Download Links

You can also share direct download links with your team so they can install Pieces before or after accepting their invitation:

* **macOS** — [Download for Mac](/products/meet-pieces/macos-installation-guide)
* **Windows** — [Download for Windows](/products/meet-pieces/windows-installation-guide)
* **Linux** — [Download for Linux](/products/meet-pieces/linux-installation-guide)

Alternatively, team members can download Pieces directly from the organization's Home page in the Pieces portal after they accept their invitation.

### Managing Seats

Make sure you have enough seats for your team before sending invitations. You can view current seat usage on the `Members` page and add seats from the `Billing` page. See [Billing](/products/organizations-and-teams/billing) for details on adjusting seat counts.

## For Team Members: Getting Started

If you've received an invitation to join a Pieces organization, follow these steps to get set up.

<Callout type="info">
  Onboarding users need to sign in with the same email the invitation was sent to.
</Callout>

### Accepting Your Invitation

<Steps>
  <Step title="Check Your Email">
    You'll receive an email invitation from your organization's admin. The email includes details about the organization and your assigned role.
  </Step>
  <Step title="Click the Invitation Link">
    Click the link in the email to accept. You'll be taken to the Pieces portal to sign in or create an account.
  </Step>
  <Step title="Create Your Account">
    If you don't already have a Pieces account, create one using the email address the invitation was sent to. If you already have an account, sign in with your existing credentials.
  </Step>
</Steps>

### Installing Pieces

After accepting your invitation, you'll land on your organization's Home page in the Pieces portal. The *Setup* section at the top provides everything you need to get Pieces installed.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/new_media03-01-26/organization_overview.png" alt="" align="center" fullwidth="true" />

> Organization Home page showing Setup section with download links and sign-in instructions

<Steps>
  <Step title="Download or Launch Pieces">
    If Pieces is already installed, click `Open Pieces Desktop` to launch it. If not, click `Download for Mac` (or your platform) to download the installer. Links for Windows and Linux are also available under *Other platforms*.
  </Step>
  <Step title="Install PiecesOS and Pieces Desktop">
    Run the downloaded installer, which sets up both Pieces Desktop and PiecesOS (the background service that powers Pieces). Follow the on-screen prompts to complete installation.
  </Step>
  <Step title="Sign In to Sync">
    After installation, sign in to Pieces Desktop and PiecesOS with the same email address associated with your organization. The Home page will remind you which email to use — look for the message that says "Sign in with [your-email] in Desktop & PiecesOS to stay in sync."
  </Step>
</Steps>

<Callout type="info">
  Signing in with your organization email ensures your settings, models, API keys, and features configured by your admin automatically sync to your installation.
</Callout>

### Exploring Resources

The *Resources* section on the Home page provides quick links to help you get the most out of Pieces:

* **Documentation** — Guides and API reference at [docs.pieces.app](https://docs.pieces.app)
* **Pro tip guides** — Tips and best practices for using Pieces effectively
* **Support** — Get help and contact the Pieces team
* **GitHub** — Explore repos and open source projects

## SSO & Provisioning

Enterprise plans support Single Sign-On (SSO) and SCIM user provisioning for streamlined onboarding. SSO lets users sign in with your identity provider, and SCIM provisioning automates user lifecycle management.

Admins can configure SSO by adding a *Descope* Tenant ID in [General Settings](/products/organizations-and-teams/settings-general). For Associated Domains, add your company's email domain to enable automatic user assignment.

<Callout type="info">
  For help setting up SSO or SCIM provisioning, contact [sales@pieces.app](mailto:sales@pieces.app).
</Callout>

***

## Next Steps

Once your team is set up, explore [Organization Settings](/products/organizations-and-teams/organization-settings) to configure features, API keys, models, and LTM sources for your entire team, or see [Features](/products/enterprise/features) for a full overview of enterprise capabilities.
