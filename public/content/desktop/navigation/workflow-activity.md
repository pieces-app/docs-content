---
title: Workflow Activity
path: /desktop/navigation/workflow-activity
visibility: HIDDEN
status: PUBLISHED
---

<Callout type="alert">
  The **Workflow Activity** view is currently live, but will soon be deprecated—stay tuned for more information, and don’t forget to check out the [Updates & Upcoming](/products/desktop/navigation/updates) view within the Pieces Desktop App.
</Callout>

***

## Accessing Workflow Activity

You can open the **Workflow Activity** page in several ways.

One approach is through the **Power Menu**—click the **Home** icon next to the search bar in the Pieces Desktop App, then select `Go to Workflow Activity`.

You can also press `⌘+return` (macOS) or `ctrl+enter` (Windows/Linux) to open the Power Menu, and choose `Workflow Activity` from the dropdown.

If you prefer a direct keyboard shortcut, use `⌘+shift+a` (macOS) or `ctrl+shift+a` (Windows/Linux) to jump straight to the **Workflow Activity** page.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/navigation/workflow_activity/pieces_workflow_activity_overview.png" alt="" align="center" fullwidth="true" />

## Main View

Once opened, you’ll see a timeline of chronological events as they relate to your **Pieces Drive** usage.

Each entry shows key details, such as the snippet name, the event type (created, updated, deleted, or referenced), and a timestamp.

A `Show: (All)` dropdown appears at the top, allowing you to filter using several *events:* `created`, `updated`, `deleted`, or `referenced`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/navigation/workflow_activity/pieces_workflow_activity_filter_dropdown.png" alt="" align="center" fullwidth="true" />

A `Refresh` button in the corner lets you reload the page to fetch the latest events, and a `Back` button returns you to the previous view.

## Searching for Events

At the top of the page, a search bar labeled *Find an Event* enables you to quickly locate specific items in your timeline.

As you type a query, the list filters in real time, displaying only events that match your search.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/navigation/workflow_activity/workflow_activity_search_deleted.png" alt="" align="center" fullwidth="true" />

## Right-Side Panels

To the right of the main activity list, you’ll find two panels—**Recent Searches** and **Top Materials.**

### Recent Searches

This panel shows your most recent event queries.

Hovering over a search term reveals options to `Search in Global Search`, `Copy Query`, or `Remove` the query from the list.

Clicking a recent search will also automatically initiate a global snippet search for that term.

### Top Materials

Here, Pieces displays your most frequently used or highest-ranked snippets, measured by *Productivity Points.*

Each snippet is accompanied by an icon and a productivity score (e.g., 113 points). Hovering over the productivity score icon reveals the exact number of points.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/navigation/workflow_activity/top_materials_info.png" alt="" align="center" fullwidth="true" />

### Productivity Points

A small `i` icon near the **Top Materials** heading provides an explanation of how *Productivity Points* are calculated.

Pieces uses a *heuristics-based system* to determine how often and in what ways a snippet is used, with higher scores indicating saved code materials that may be particularly useful given the task at hand.

## Opening Snippets

When you click on a snippet in **Top Materials** or in the main **Workflow Activity** list, Pieces immediately opens the Snippet View for that saved material.

Additionally, accessing any snippet triggers a new `Referenced` event in your timeline, confirming that you revisited or used that snippet.
