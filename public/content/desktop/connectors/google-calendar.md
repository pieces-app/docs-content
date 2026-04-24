---
title: Google Calendar Connector
path: /desktop/connectors/google-calendar
visibility: PRIVATE
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

Example prompts:

* *"When am I free for a 45-minute meeting this week?"*
* *"Summarize what I worked on during yesterday's 1:1 with Alice."*
* *"Move my 3pm to Friday morning and let the attendees know."*

## Disconnecting Google Calendar

Revoke access at any time from the same settings pane.

<Steps>
  <Step title="Open Connectors Settings">
    In the Pieces Desktop App, open `Settings` and select `Connectors`.
  </Step>
  <Step title="Disconnect">
    Click `Disconnect` next to *Google Calendar*. Pieces revokes the OAuth token and stops accessing your calendar.
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
* [Setting Additional Context](/products/desktop/conversational-search/setting-context) — combine calendar data with LTM context and chat pipelines.
* [Connectors Overview](/products/desktop/connectors) — see every available connector.
