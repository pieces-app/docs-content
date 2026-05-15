---
title: Google Calendar Connector
path: /desktop/connectors/google-calendar
visibility: PUBLIC
status: PUBLISHED
description: Connect your Google Calendar to Pieces so Conversational Search can read your schedule and create, update, and cancel events on your behalf.
metaTitle: Google Calendar Connector | Pieces Connectors
metaDescription: Connect Google Calendar to Pieces to pull meeting context into Conversational Search and manage events—create, reschedule, invite attendees, and more—from chat.
---

## Google Calendar Connector

The *Google Calendar* connector links your Google account to Pieces so [Conversational Search](/products/desktop/conversational-search) can both **read** your schedule and **act** on it—creating events, inviting attendees, rescheduling meetings, and more.

Once connected, you can ask Pieces things like *"What do I have tomorrow afternoon?"* or *"Schedule a 30-minute sync with Alice next Tuesday at 2pm with a Google Meet link."*

## Connecting Google Calendar

Connect your Google account through a standard OAuth flow in your default browser.

<Steps>
  <Step title="Open Connectors Settings">
    In the Pieces Desktop App, open `Settings` and select `Connectors`.
  </Step>
  <Step title="Connect Google Calendar">
    Click `Connect` next to *Google Calendar*. Pieces opens your default browser to Google's authorization page.
  </Step>
  <Step title="Authorize Pieces">
    Sign in to the Google account you want to connect and grant the requested calendar permissions.
  </Step>
  <Step title="Return to Pieces">
    Once authorization completes, your browser redirects back to Pieces. The connector's button changes from `Connect` to `Disconnect`, confirming the account is linked.
  </Step>
</Steps>

## What You Can Do

Once connected, Conversational Search can use the *Google Calendar* connector to query your schedule, take actions, and enrich answers with calendar context.

| Feature | Example prompt |
| --- | --- |
| **View your schedule** | *"What's on my calendar this week?"* |
| **Inspect an event** | *"Show me the attendees, location, and description for my 2pm standup tomorrow."* |
| **Search events** | *"Find my most recent 1:1 with Alice."* |
| **Create an event** | *"Schedule a 30-minute sync with alice@example.com next Tuesday at 2pm and add a Google Meet link."* |
| **Create an all-day event** | *"Block Friday as an all-day focus day on my work calendar."* |
| **Reschedule** | *"Move my 3pm Friday meeting to Monday at 10am and notify attendees."* |
| **Update event details** | *"Add bob@example.com to my 4pm sync and update the description with the new agenda."* |
| **Cancel an event** | *"Cancel my 10am standup tomorrow and send cancellation emails."* |
| **Check availability** | *"When am I free for a 45-minute meeting this week?"* |
| **Scope to one account** | *"Show this week's events on my work calendar, not personal."* |
| **Query a shared calendar** | *"What's on the team calendar for next Monday?"* |
| **Combine with workflow context** | *"Summarize what I worked on during yesterday's 1:1 with Alice."* |

<Callout type="warning">
  Deleting an event is permanent. Pieces will always confirm before cancelling an event on your behalf.
</Callout>

## Using Calendar Context in Conversational Search

Beyond direct calendar management, Pieces uses your calendar to enrich answers.

* **Check availability** before suggesting meeting times.
* **Provide context** about upcoming or recent meetings when answering questions.
* **Cross-reference** calendar events with activity captured by [Long-Term Memory](/products/core-dependencies/pieces-os/long-term-memory).

## Calendar Context in Summaries

Once connected, your calendar events flow into [Single-Click Summaries](/products/desktop/single-click-summaries) that use workflow context, including *Morning Brief*, *Standup Update*, and *Day Recap*. These summaries reflect what was actually on your schedule rather than what happened to be visible on your screen.

The *Google Calendar* connector is also the foundation for [Meeting Prep](/products/desktop/single-click-summaries/default-types#meeting-prep), a summary type that looks ahead at your upcoming meetings, cross-references each event with your Long-Term Memory, and generates a structured pre-read.

Example prompts:

* *"When am I free for a 45-minute meeting this week?"*
* *"Summarize what I worked on during yesterday's 1:1 with Alice."*
* *"Move my 3pm to Friday morning and let the attendees know."*

## Managing Connected Accounts

You can connect multiple Google accounts and manage them from the connector's management screen.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Connectors/google_calendar_manage_modal.png" alt="Google Calendar Manage modal showing connected accounts and add account option" align="center" fullwidth="true" />

> Google Calendar Manage modal showing connected accounts, reconnect options, and add account button

<Steps>
  <Step title="Open Connectors Settings">
    In the Pieces Desktop App, open `Settings` and select `Connectors`.
  </Step>
  <Step title="Click Manage">
    Click the `Manage` button next to *Google Calendar* to open the management modal.
  </Step>
  <Step title="View Connected Accounts">
    The modal shows your **Connected Accounts** count and lists each linked account. You can also see accounts under **Needs Attention** if they've been disconnected and require reconnection.
  </Step>
</Steps>

### Adding Another Account

Connect additional Google accounts to access multiple calendars.

<Steps>
  <Step title="Open the Manage Modal">
    Click `Manage` next to *Google Calendar* in Connectors settings.
  </Step>
  <Step title="Click Add Account">
    Click `+ Add account` in the Connected Accounts section.
  </Step>
  <Step title="Authorize the New Account">
    Complete the OAuth flow for the additional Google account.
  </Step>
</Steps>

### Reconnecting a Disconnected Account

If an account appears under **Needs Attention**, you can reconnect it.

<Steps>
  <Step title="Open the Manage Modal">
    Click `Manage` next to *Google Calendar* in Connectors settings.
  </Step>
  <Step title="Find the Disconnected Account">
    Look under **Needs Attention** for accounts showing "Disconnected" status.
  </Step>
  <Step title="Click Reconnect">
    Click the `Reconnect` button next to the account to re-authorize access.
  </Step>
</Steps>

### Disconnecting an Account

Remove access for a specific Google account.

<Steps>
  <Step title="Open the Manage Modal">
    Click `Manage` next to *Google Calendar* in Connectors settings.
  </Step>
  <Step title="Find the Account">
    Locate the account you want to disconnect in the Connected Accounts list or Needs Attention section.
  </Step>
  <Step title="Click the Delete Icon">
    Click the `trash icon` next to the account to disconnect it. Pieces revokes the OAuth token and stops accessing that account's calendar.
  </Step>
</Steps>

## Limitations

The current release of the *Google Calendar* connector has the following limitations:

* **Invitation responses** — Pieces cannot accept or decline invitations on your behalf.
* **Calendar settings** — Pieces cannot manage calendar permissions or settings.
* **Recurring event rules** — Pieces cannot create recurrence rules, though it can read individual instances of recurring events.

***

## Next Steps

Learn more about how *Google Calendar* integrates with the rest of Pieces:

* [Conversational Search](/products/desktop/conversational-search) — where the *Google Calendar* connector is surfaced.
* [Add Context to Your Chats](/products/desktop/conversational-search/setting-context) — combine calendar data with LTM context.
* [Connectors Overview](/products/desktop/connectors) — see every available connector.
