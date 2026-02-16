---
title: Inviting Members
path: /desktop/organizations-and-teams/inviting-members
visibility: PUBLIC
status: PUBLISHED
description: Learn how to invite team members to your organization, assign roles, and use bulk invitation methods.
metaTitle: Inviting Members | Pieces Docs
metaDescription: Step-by-step guide to inviting members to your organization, including single invites, multiple invites, and CSV bulk uploads.
---

## Inviting Members

Add team members to your organization by sending invitations. You can invite members individually, add multiple members at once, or bulk upload invitations via CSV file. Each member must have an available seat in your subscription.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/managing-organizations/inviting-members/invite-to-org.png" alt="" align="center" fullwidth="true" />

> Invite members modal showing email input, role selection, and CSV upload option

## Understanding Member Roles

Before inviting members, understand the different roles available and what each role can do within your organization.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/managing-organizations/inviting-members/inviting_members_roles.png" alt="" align="center" fullwidth="true" />

> Member roles overview showing Owner, Admin, Write, and Read role descriptions

Each role has different permissions:

* **Owner** - Full control including organization deletion
* **Admin** - Full access except organization deletion
* **Write** - Can create and edit resources
* **Read** - View-only access

## Invitation Methods

Invite team members using different methods depending on your needs and team size.


### Inviting a Single Member

Invite one team member at a time with a specific role assignment.

<Steps>
  <Step title="Open Invite Modal">
    From the *organization overview* page, click the `Invite people` button in the top right corner.
  </Step>

  <Step title="Enter Email Address">
    In the *Invite Organization Members* modal, enter the email address of the person you want to invite in the *email input* field.
  </Step>

  <Step title="Select Role">
    Click the `Select a role...` *dropdown* next to the email field and choose the appropriate role (Owner, Admin, Write, or Read).
  </Step>

  <Step title="Send Invitation">
    Click the `Send Invites & Finish` button (or `Send Invitations` if available) to send the invitation. The member will receive an email with instructions to join.
  </Step>
</Steps>

### Inviting Multiple Members

Add multiple members in a single invitation flow.

<Steps>
  <Step title="Open Invite Modal">
    Click the `Invite people` button from the *organization overview* page.
  </Step>

  <Step title="Enter First Member">
    Enter the email address and select a role for the first member.
  </Step>

  <Step title="Add Another Member">
    Click the `+ Add another member` link below the first member's information.
  </Step>

  <Step title="Enter Additional Members">
    Repeat the process to add email addresses and roles for each additional member you want to invite.
  </Step>

  <Step title="Send All Invitations">
    Once all members are added, click `Send Invites & Finish` to send invitations to all members at once.
  </Step>
</Steps>

### Bulk Inviting via CSV

Upload a CSV file to invite multiple members at once, which is efficient for large teams.

<Steps>
  <Step title="Open Invite Modal">
    Click the `Invite people` button from the *organization overview* page.
  </Step>

  <Step title="Prepare CSV File">
    Create a CSV file with the format: `email,role` (one member per line). For example:
    ```
    john@example.com,Admin
    jane@example.com,Write
    bob@example.com,Read
    ```
  </Step>

  <Step title="Upload CSV">
    In the *invite* modal, find the *Upload CSV* section. Click the `Upload CSV` button or drag and drop your CSV file into the *upload* area.
  </Step>

  <Step title="Review and Send">
    Review the imported members and their roles, then click `Send Invites & Finish` to send all invitations.
  </Step>
</Steps>

## Understanding Seat Limitations

Your organization subscription includes a specific number of seats that determine how many active members you can have. Each active member uses one seat, and you cannot invite more members than you have available seats.

<Callout type="alert">
  You can only invite members if you have available seats in your subscription. If you see a "No seats available" warning, you'll need to upgrade your subscription or remove inactive members before inviting new ones.
</Callout>

### Checking Seat Availability

Before inviting members, check your current seat usage:

<Steps>
  <Step title="Navigate to Members Tab">
    From your *organization overview* page, click `Members` in the *sidebar* navigation.
  </Step>
  <Step title="View Seat Usage">
    At the top of the *Members* page, you'll see the *Seat Usage* card showing how many seats are used out of your total subscription (e.g., "1 of 1 seats used").
  </Step>
  <Step title="Upgrade if Needed">
    If you need more seats, navigate to the *Billing* tab to increase your seat count. You can also remove inactive members to free up seats.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/organizations-and-teams/managing-organizations/managing-members/members-overview.png" alt="" align="center" fullwidth="true" />

> Members tab showing seat usage card with current usage and total seats

### Seat Management

Understanding how seats work helps you manage your organization effectively:

* **Seat Usage** - View current seat usage in the *Members* tab
* **Upgrading Seats** - Increase seats from the *Billing* tab when you need to invite more members
* **Minimum Seats** - You must maintain at least one seat based on your number of active members
* **Available Seats** - Available seats = Total seats - Active members

***

## Next Steps

Now that you know how to invite members, learn about [managing members](/products/organizations-and-teams/managing-members) to update roles and handle member-related tasks, or explore [billing](/products/organizations-and-teams/billing) to manage your subscription and seat count.
