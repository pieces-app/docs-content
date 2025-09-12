---
title: Introduction to Workstream Activity
path: /desktop/workstream-activity
visibility: PUBLIC
status: PUBLISHED
description: Workstream Activity is your main hub for viewing all summaries, workflow context, and related information gathered by the Long-Term Memory (LTM-2.7) Engine.
metaTitle: Introduction to Workstream Activity | Pieces Docs
metaDescription: Workstream Activity is your main hub for viewing all summaries, workflow context, and related information gathered by the Long-Term Memory (LTM-2) Engine.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/workstream_activity/new_workstreamsep-8/general_workstream.png" alt="" align="center" fullwidth="true" />

***

## Overview

The Workstream Activity view in the Pieces Desktop App integrates with the new-and-improved Long-Term Memory Engine (LTM-2.7) to capture and summarize your recent tasks, discussions, code reviews, and more.

By automatically generating concise roll-ups of your workflow, Workstream Activity aims to *eliminate* the repetitive context-setting required by most AI tools.

<Callout type="tip">
  LTM-2.7—also referred to as *Long-Term Memory Engine*—is available as part of PiecesOS, which is required for the Pieces Desktop App.

  Make sure you have the latest versions installed to take advantage of this feature.
</Callout>

## Main View

Once you access Workstream Activity, you’ll see two main UI elements:

1. **Activity Sidebar (Left Panel)**: A chronological list of your LTM roll-ups. Each roll-up is timestamped (e.g., “9:04 AM – 9:14 AM”) with a descriptive title (such as “Documentation & LTM-2.7 Prep”).

2. **Roll-Up Details (Right Panel)**: Selecting a roll-up displays its sections and bullet points, including embedded links, references, or code snippet IDs.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/workstream_activity/new_workstreamsep-8/different_general_workstream.png" alt="" align="center" fullwidth="true" />

### Long-Term Memory (LTM-2.7) Engine

Long-Term Memory is an advanced memory agent that captures your workflow context at repeated intervals and preserves it for up to *nine months*.

Instead of starting fresh with every AI query, you can use LTM-2.7’s persistent memory to pick up any past conversation, code snippet, or link you’ve encountered.

Visit our [Core Dependencies documentation](/products/core-dependencies) read more about LTM.

### LTM Roll-Ups

Each *roll-up* is a one-page summary that includes information and specific sections, such as:

* **Core Tasks & Projects**: A concise, but rich overview of projects, tasks or specific initiatives you’ve worked on—including problems and solutions (and how you came to that solution).

* **Key Decisions & Discussions**: Important conversations or choices you made, mentioning with whom you had discussions or meetings or who shared critical details that had implications on your workflow.

* **Documents & Code Reviewed**: References to any files, articles, or snippets you accessed, often deep-linked with clickable URLs (where applicable).

* **Follow-Up Actions**: Unfinished items, suggestions for next steps, and reminders.

* **NEW: "Formed with MCP" Indicator**: Workstream activities created through Model Context Protocol (MCP) integrations will display a "Formed with MCP" button/pill, indicating they were generated using external MCP tools like the Pieces MCP integration.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/workstream_activity/new_workstreamsep-8/mcp_tag.png" alt="" align="center" fullwidth="true" />

### Interacting with LTM Roll-Ups

Each roll-up offers multiple interaction points:

* `Start Copilot Chat`: Immediately open a Pieces Copilot Chat session scoped to that roll-up’s context; the summary is used as context right away so you don’t need to restate anything.

* `Export` (toolbar): Download the summary as `PDF`, `Markdown (.md)`, or `Plain Text (.txt)` directly from the toolbar.

* `More (three-dots)`: Access quick actions — `Edit` (opens the editor; see [Editing Workstream Activities](/desktop/workstream-activity/edit-workstream-activities)), `Copy to Clipboard`, or `Delete`.

* **NEW: macOS Share Feature**: On macOS, use the native Apple share feature to share workstream summaries directly to chats, AirDrop, and other macOS applications.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/workstream_activity/new_share_option.png" alt="" align="center" fullwidth="true" />

* `Deep Links`: Open references directly in your browser. If the roll-up mentions a specific blog or document, you can jump straight to it from within Pieces.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/workstream_activity/new_workstreamsep-8/deep_links_options.gif" alt="" align="center" fullwidth="true" />

### Editing Workstream Activities

You can edit and customize your workstream activities to better reflect your workflow context or add additional details that weren't automatically captured.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/workstream_activity/new_workstreamsep-8/editing_view.png" alt="" align="center" fullwidth="true" />


<Callout type="note">
  <strong>macOS native Share:</strong> On macOS, the clipboard/share action can invoke the system Share sheet to send a summary as <em>PDF</em>, <em>Markdown</em>, or <em>Plain Text</em> to recent contacts or apps like AirDrop, Mail, Messages, Notes, and other installed apps.
</Callout>

### Generating LTM Rollups

If your workflow context falls outside the default 30-minute roll-up window, you can generate a manual Workstream Rollup instead.

This is especially useful when you want to capture a broader time range—like **Today** or **This Afternoon**—which might span from 12:00 P.M. to 4:28 P.M., for example.

Creating a roll-up across a wider time frame offers a more comprehensive view of your recent work and contextual activity. It’s a great way to zoom out and get a high-level snapshot of what’s been accomplished, especially when shorter intervals don’t provide enough detail.

To do this, click the white `plus` icon at the bottom left of the **Workstream Activities** view.

This opens up a *Time Range Selection* menu, which allows you to generate a summary based on a wide variety of time ranges:

| **Range**              | **Example**                          |
| ---------------------- | ------------------------------------ |
| *Just Now*             | 4:35PM → 4:36 PM                     |
| *Last Couple Minutes*  | 4:33 PM → 4:35 PM                    |
| *Within the Last Hour* | 3:36PM → 4:33 PM                     |
| *Around Lunch*         | 12:00 PM → 1:00 PM                   |
| *Yesterday Afternoon*  | Yesterday 12:00PM → 5:00PM           |
| *Yesterday Morning*    | Yesterday 5:00AM → 12:00 PM          |
| *This Month*           | April 1, 12:00AM → April 17, 4:36 PM |

… and many more. In total, there are *31 time ranges* to select from to best fit your use case.

Then, select your desired time ranges, and click the `green checkmark` icon to generate the summary.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/workstream_activity/new_workstreamsep-8/generating_workstream_activity.gif" alt="" align="center" fullwidth="true" />

### Related Workstream Activities

Pieces Copilot uses memories and workflow context from the LTM engine to give you a relevant, context-rich answer. Below the response, you'll see Workstream Activity cards.

The cards link to past *Workstream Activity Rollups* that contain the context used to create that response.

This will use *Rollups* relevant to your question and what you're currently working on, as Pieces works to find all *Workstream Activity Rollups associated with the query.*

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/workstream_activity/new_workstreamsep-8/generate_a_rollup.png" alt="" align="center" fullwidth="true" />

<Callout type="tip">
  Clicking one of the surfaced context cards will take you to that specific Rollup in the **Workstream Activities** view.
</Callout>

## Use Cases

Workstream Activity turns your daily work into a rich, queryable memory—so you never have to waste time re-explaining, re-documenting, or retracing your steps.

<Card title="Why use the Workstream Activities feature?" image="/assets/icons/platform_logos/pieces_logo.png">
  The Workstream Activity feature centralizes your workflow context, tackling a major productivity blocker in AI-assisted development—*short-term memory.*

  It eliminates the need to repeat information to an AI assistant, ensures project continuity, provides a powerful search for past discussions or documents, and allows for flexible exports to share or store roll-ups.
</Card>

With support from the LTM-2.7 engine, it becomes easy to search, share, and summarize critical moments from your workflow.

Here are some practical ways to use it:

<AccordionGroup>
  <Accordion title="Create Context Packs for Onboarding New Team Members">
    Filter and export roll-ups related to a specific project or time range, and then share them with new hires so they can instantly understand decisions, architecture, and open tasks, without the need for lengthy handoffs.
  </Accordion>

  <Accordion title="Build AI-Ready Summaries for Async Standups and Check-Ins">
    Instead of writing updates from scratch, turn a roll-up into a formatted summary or paste it into Pieces Copilot for a clean, human-readable update.
  </Accordion>

  <Accordion title="Generate Internal Documentation from Real Workflows">
    Use LTM summaries as the base for internal docs or knowledge bases. Each roll-up captures exactly what was discussed, reviewed, or built—no guesswork needed afterward.
  </Accordion>

  <Accordion title="Recover Forgotten Context After a Break">
    If you’ve been away from a project for a few days (or weeks), scroll back through Workstream Activity to instantly recall what you were doing, what was pending, and what resources were relevant.
  </Accordion>

  <Accordion title="Audit Past Decisions and Review Rationale">
    Return to a past roll-up to see why a decision was made, who was involved, and what options were discussed—perfect for retrospectives or incident reviews.
  </Accordion>

  <Accordion title="Track Research and Learning Progress Over Time">
    Whether you’re exploring new tech, debugging a complex problem, or reviewing articles, your LTM-2.7 roll-ups capture the learning trail so you can build on it later—or share it with others.
  </Accordion>
</AccordionGroup>

Want to keep reading?

Check out this quick guide for more use cases, featuring in-depth, real-world scenarios on [using the Workstream Activities view.](/products/quick-guides/ltm-prompting/workstream-activity)

<Callout type="tip">
  If you remember that a teammate shared a solution link last month, you can locate that exact snippet, conversation, or link by searching the relevant keyword in Workstream Activity.
</Callout>

### Privacy & Source Control

<mark>Your data is yours to manage.</mark>

At any time, even after a summary has been generated, you can disable sources from which LTM captures workflow data. Since LTM is available for use outside of the Pieces Desktop App, there are two locations from which you can make these changes.

In the Workstream Activity view, there is an LTM Access Control modal designated by a grid-like icon—clicking this opens the modal, where you can toggle or un-toggle data capture from specific sources.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/workstream_activity/new_workstreamsep-8/access_settings.png" alt="" align="center" fullwidth="true" />

In the PiecesOS task bar window, you can [disable any sources you don’t wish to capture](/products/core-dependencies/pieces-os/quick-menu#quick-menu-actions) (e.g., personal browsing activity or data from messaging applications) through the LTM Access Control panel.

Events gathered from disabled sources will be *removed* from your roll-ups so they don’t appear in Workstream Activity or Pieces Copilot Chats.