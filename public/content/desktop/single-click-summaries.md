---
title: Single-Click Summaries
path: /desktop/single-click-summaries
visibility: PUBLIC
status: PUBLISHED
description: Generate instant, contextual summaries from your workflow using preset summary types in Pieces.
metaTitle: Single-Click Summaries | Pieces Docs
metaDescription: Generate instant, contextual summaries from your workflow using preset summary types in Pieces Desktop.
---

<Embed 
  src="https://youtu.be/qpQKW2T36nI" 
  title="Single-Click Summaries overview video demonstrating the summary types, generating summaries, and viewing results"
/>

***

## Overview

Single-Click Summaries are quick-access actions prominently displayed when you first open the Pieces Desktop App. These summaries generate instant, contextual insights from your workflow captured by the [Long-Term Memory (LTM-2.7)](/products/core-dependencies/pieces-os#ltm-27) Engine.

Each summary type adapts dynamically to your workflow, meaning the same summary type generates different results based on your current activities, captured memories, and work patterns. This makes Single-Click Summaries powerful tools for understanding your productivity, tracking progress, and identifying patterns in your work.

## Generating Summaries

Click any summary card on the homepage and after a few minutes, you'll see your summary in the [Pieces Timeline](/products/desktop/timeline).

<Callout type="tip">
  You can run several Single-Click Summaries at once. Start a *Day Recap*, *Standup Update*, and *Meeting Prep* together and let them generate side by side. You no longer need to wait for one to finish before starting the next.
</Callout>

### Viewing Queued Summaries

When you generate a summary, it appears under the current day in Pieces Timeline with a "Queued" or generating status. Expand the day section to track progress. The Timeline stays responsive while summaries generate, so you can keep scrolling and reading even with several in flight.

<Steps>
  <Step title="Open Timeline">
    Click `Show Timeline` in the top left of the main view to expand Pieces Timeline if it's not already open.
  </Step>
  <Step title="Expand Current Day">
    Click on the current day section to expand it and view all summaries, timeline activities, and other events for that day.
  </Step>
  <Step title="View Queued Summaries">
    Queued summaries appear with a "Queued" status indicator showing their position in the queue (e.g., "Queued (#3)", "Next in queue").
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/timeline/queued_summaries_in_timeline.png" alt="Timeline with queued Single-Click Summaries for the current day" align="center" fullwidth="true" />

> Pieces Timeline showing current day expanded with queued summaries visible

### Canceling a Summary

Locate the summary you want to cancel under the current day in Pieces Timeline and click the red cancel button (hovering shows `Stop Generating`).

### Viewing Completed Summaries

When a summary finishes generating, it remains in the day section where it was queued. Click it to view detailed insights, related activities, and artifacts from your workflow.

Summaries are based on **memories from a given time frame**—not a guess from whatever was on screen. Those memories can include vision, audio, clipboard activity, browser URLs you visited, files you opened, and people you collaborated with. A completed summary usually includes a high-level overview of that context plus people, URLs, files, next steps, and tasks. Files and sites cited in a summary are **clickable**, so you can open them directly.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/single-click-summaries/completed_summary_view_with_results.png" alt="Completed summary with insights, related activities, and document links" align="center" fullwidth="true" />

> Completed summary view showing full results with insights, related activities, and links to relevant documents

### People, Tags & Files

Pieces detects people mentioned in your workstream and people you have collaborated with, then turns each name in a summary into a rich, hoverable reference. Hover any name to open a **persona card** showing who they are, how to reach them, their role, and how you two have worked together over time.

*Tags* and *files/folders* in summaries work the same way: live references instead of plain text.

This is especially useful when:

* A summary mentions someone you've met once and can't quite place
* You're walking into a meeting and want context on an attendee without leaving the page
* You need to recall what you and a teammate last decided together

***

## Explore Single-Click Summaries

<FancyCard title="Default Types" href="/products/desktop/single-click-summaries/default-types" colored={false}>
  Browse all built-in summary types—Day Recap, Standup Update, Time Breakdown, AI Habits, and more.
</FancyCard>

<FancyCard title="Customization & Templates" href="/products/desktop/single-click-summaries/customization-templates" colored={false}>
  Create custom summaries with specific time ranges, save reusable templates, and request new summary types.
</FancyCard>

<FancyCard title="Scheduling" href="/products/desktop/single-click-summaries/scheduling" colored={false}>
  Schedule summaries to run automatically—daily or on specific days of the week.
</FancyCard>
