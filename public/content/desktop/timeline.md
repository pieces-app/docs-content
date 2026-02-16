---
title: Pieces Timeline
path: /desktop/timeline
visibility: PUBLIC
status: PUBLISHED
description: Pieces Timeline is your central workspace for viewing all workflow events, summaries, and conversational searches captured by the Long-Term Memory (LTM-2.7) Engine.
metaTitle: Pieces Timeline | Pieces Docs
metaDescription: Access your workflow history, view summaries, and manage timeline events in Pieces Timeline—your central workspace for captured workflow context.
---

<Embed 
  src="https://youtu.be/Qqak02u_Xhw" 
  title="Pieces Timeline overview video demonstrating the interface, event types, filtering, and event management"
/>

***

## Overview

**Pieces Timeline** is your central workspace in the Pieces Desktop App for accessing all workflow context captured by the [Long-Term Memory (LTM-2.7)](/products/core-dependencies/pieces-os#ltm-27) Engine. Timeline displays a chronological view of your workflow events, including [timeline events](/products/desktop/timeline/timeline-events), [single-click summaries](/products/desktop/single-click-summaries), and [conversational searches](/products/desktop/conversational-search).

All events are organized chronologically from most recent at the top to oldest at the bottom, grouped by day. Each day section can be expanded or collapsed by clicking on it or using the caret icon. You can scroll through your timeline, filter events by type or source, and click any event to view its full content in the main view.

## Opening Pieces Timeline

Access Pieces Timeline from the main view to see all your workflow events and summaries.

<Steps>
  <Step title="Click Show Timeline Button">
    Click the `Show Timeline` button in the top left of the main view if Pieces Timeline isn't already open.
  </Step>
  <Step title="View Timeline">
    The Pieces Timeline opens on the left side, showing all your workflow events organized chronologically.
  </Step>
  <Step title="Close Timeline (Optional)">
    Click `Show Timeline` again to close Pieces Timeline and return to the main view.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/timeline/timeline-events/hovering_over_show_timeline.png" alt="" align="center" fullwidth="true" />

> Main view showing `Show Timeline` button in top left, with Pieces Timeline open displaying chronological events

## Understanding Timeline Contents

Pieces Timeline displays three main types of events, all organized chronologically from most recent to oldest:

* **Timeline Events** - Workflow moments captured by LTM-2.7, including code changes, document edits, and other activities from your connected applications. Timeline Events also include automatically generated summaries that capture your work patterns, such as `Day Recap`, `Morning Brief`, `Week Recap`, and `What's Top of Mind`. These events compile what you've been working on, conversations you've had, and activities you've completed.

* **Single-Click Summaries** - [Summaries you generate on demand](/products/desktop/single-click-summaries) by clicking summary cards on the homepage, including Standup Update, Custom Summary, AI Habits, and more. Once generated, they appear as Timeline Events in your timeline.

* **Conversational Searches** - [Chat conversations you have with your memories](/products/desktop/conversational-search). Each conversation appears as an event in Pieces Timeline, allowing you to revisit past conversations and their context.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/timeline/timeline-events/searching_through_timeline_events_slash_activities.png" alt="" align="center" fullwidth="true" />

> Pieces Timeline showing different event types: conversational search event, standup update summary, and timeline events with app icons

## Viewing Queued Summaries

When you generate single-click summaries, they appear under the current day in Pieces Timeline with a "Queued" status. Summaries are organized by day, and you can expand or collapse each day to view its contents.

<Steps>
  <Step title="Open Timeline">
    Click `Show Timeline` in the top left of the main view to expand Pieces Timeline if it's not already open.
  </Step>
  <Step title="Locate Current Day">
    The current day section appears at the top of Pieces Timeline, below the `Filter Timeline` search bar. It shows the date (e.g., "Today, Jan 21st") with a count of items.
  </Step>
  <Step title="Expand Day Section">
    Click on the current day section to expand it and view all summaries, timeline activities, and other events for that day.
  </Step>
  <Step title="View Queued Summaries">
    Queued summaries appear under the current day with a "Queued" status indicator. You can see which summaries are waiting to be processed and their position in the queue (e.g., "Queued (#3)", "Queued (#2)", "Next in queue").
  </Step>
  <Step title="Collapse Day Section">
    Click the `caret icon` (dropdown arrow) at the top of the day divider to collapse the day section and hide its contents.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/timeline/queued_summaries_in_timeline.png" alt="" align="center" fullwidth="true" />

> Pieces Timeline showing current day expanded with queued summaries visible, including "What's Top of Mind" showing "Queued (#3)", "Day Recap" showing "Queued (#2)", and "AI Habits" showing "Next in queue"

<Callout type="tip">
  Once summaries finish generating, they remain in the day section where they were queued. You can click on any summary to view its full content, whether it's queued, processing, or completed.
</Callout>

## Viewing Event Content

Click any event in Pieces Timeline to view its full content in the main view panel.

<Steps>
  <Step title="Select an Event">
    Click any event in Pieces Timeline—this can be a timeline event, summary, or conversational search.
  </Step>
  <Step title="View Content">
    The event's full content opens in the main view panel on the right, replacing the homepage view.
  </Step>
  <Step title="Navigate Between Events">
    Use the left and right arrow buttons in the event header to navigate to previous or next events without returning to Pieces Timeline.
  </Step>
  <Step title="Return to Timeline">
    Click the `home` icon or close the event view to return to browsing Timeline Events.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/timeline/timeline_summaries.png" alt="" align="center" fullwidth="true" />

> Event selected in Pieces Timeline (highlighted) with its full content displayed in the main view panel on the right

## Managing Event Groups

Events in Pieces Timeline are automatically grouped by day, making it easy to find activities from specific time periods.

### Understanding Day Groups

Events are organized into collapsible groups labeled by date:
* **Today** - Events from the current day
* **Yesterday** - Events from the previous day
* **[Date]** - Older events grouped by specific dates (e.g., "Jan 14th")

Each group header displays the date and a count of events in that group (e.g., "Today, Jan 15th (2)").

### Collapsing and Expanding Groups

Organize your Timeline view by collapsing groups you don't need to see.

<Steps>
  <Step title="Locate Group Header">
    Find the date group header you want to collapse (e.g., "Yesterday, Jan 14th").
  </Step>
  <Step title="Click to Collapse">
    Click the group header to collapse it. The group collapses, hiding all events within it.
  </Step>
  <Step title="Expand Group">
    Click the collapsed group header again to expand it and view all events.
  </Step>
</Steps>

### Jump to Summary in List

Quickly navigate to a specific event's position in the Timeline sidebar when viewing its content.

<Steps>
  <Step title="Open Event Content">
    Click an event in Timeline to view its content in the main view.
  </Step>
  <Step title="Click Jump Button">
    Click the `Jump to Summary in List` button (target icon) next to the `Filter List` button in Pieces Timeline header. This scrolls Pieces Timeline to show where the current event appears in the chronological list.
  </Step>
  <Step title="Collapse All Groups">
    Alternatively, click the `collapse` button to collapse all event groups at once, giving you a compact view of all dates.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/timeline/jump_to_summary_in_timeline.png" alt="" align="center" fullwidth="true" />

> Pieces Timeline showing day groups (Today expanded, Yesterday collapsed) with event counts, and `Jump to Summary in List` button visible in header

## Filtering Timeline Events

Filter your Timeline to focus on specific event types, sources, or applications. Use the Filter List button to access all filtering options.

<FancyCard title="Learn More" href="/products/desktop/timeline/filtering-events" colored={false}>
  Learn how to filter Timeline events by type, source, application, and favorites to find exactly what you need.
</FancyCard>

## Event Actions and Menus

Different event types have different actions available through the three-dots menu. Conversational searches have the most options, while summaries have simpler action sets.

<FancyCard title="Learn More" href="/products/desktop/timeline/event-actions" colored={false}>
  Learn how to favorite events, generate titles and summaries, delete events, and understand which actions are available for each event type.
</FancyCard>

***

If Pieces Timeline isn't what you're looking for, check out [Single-Click Summaries](/products/desktop/single-click-summaries) to learn how to generate instant summaries, or explore [Conversational Search](/products/desktop/conversational-search) to have conversations with your memories.
