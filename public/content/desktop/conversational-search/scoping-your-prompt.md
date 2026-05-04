---
title: Scoping Your Prompt
path: /desktop/conversational-search/scoping-your-prompt
visibility: PUBLIC
status: PUBLISHED
description: Use Sources, Time Ranges, and Modalities filters to narrow which memories Conversational Search draws from when answering your questions.
metaTitle: Scoping Your Prompt | Conversational Search
metaDescription: Narrow your Conversational Search results using Sources, Time Ranges, and Modalities filters to get more focused, accurate answers.
---

## Scoping Your Prompt

Filter by specific apps, time ranges, or modalities to narrow your search scope and get more focused answers. Filters control *which memories* Conversational Search draws from when answering your questions.

## Sources Filter

Limit searches to memories from specific applications. Use this when you want answers based only on specific apps.

<Steps>
  <Step title="Click Sources Button">
    Click the `Sources` button in the *bottom toolbar* to open the filter modal.
  </Step>

  <Step title="Select Apps">
    Check the apps you want to include. You can select multiple apps at once.
  </Step>

  <Step title="Apply Filter">
    Selected sources apply to your current chat and all future messages until you change them.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/conversational_search_filter_sources.png" alt="Sources filter modal with app checkboxes, Chrome and VS Code selected" align="center" fullwidth="true" />

> Sources filter modal showing list of apps with checkboxes, with Chrome and VS Code selected

## Time Ranges Filter

Focus searches on specific time periods. Use this when you need information from a specific period.

<Steps>
  <Step title="Click Time Ranges Button">
    Click the `Time Ranges` button in the *bottom toolbar* to open the filter modal.
  </Step>

  <Step title="Select Time Range">
    Choose from 31+ preset options (e.g., "Yesterday", "This week", "Last month") or use the calendar view for custom date ranges. You can select multiple ranges at once.
  </Step>

  <Step title="Apply Filter">
    Selected time ranges apply to your current chat and all future messages until you change them.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/conversational_search_filter_time.png" alt="Time Ranges modal showing preset options and calendar view" align="center" fullwidth="true" />

> Time Ranges modal showing preset options and calendar view

## Modalities Filter

Restrict searches to specific types of captured context—what you've seen, copied, said, or scheduled. Use this when you want answers grounded in a particular *kind* of memory rather than a particular app.

<Steps>
  <Step title="Click Modalities Button">
    Click the `Modalities` button in the *bottom toolbar* to open the **Refine by Modality** panel.
  </Step>

  <Step title="Select Modalities">
    Check any combination of the available modalities:

    - **Vision** — what you've seen (screen context captured by LTM).
    - **Clipboard** — what you've copied and pasted.
    - **Audio** — what you've said and heard.
    - **Google Calendar** — events and meeting context from connected calendars.
  </Step>

  <Step title="Manage Connections">
    Click **Manage Connections** at the bottom of the panel to enable, disable, or authorize the integrations that power each modality (for example, connecting a Google Calendar account).
  </Step>

  <Step title="Apply Filter">
    Selected modalities apply to your current chat and all future messages until you change them.
  </Step>
</Steps>

> Some modalities depend on connected integrations or permissions (e.g. Google Calendar, microphone access for Audio). If a modality is unavailable, open **Manage Connections** to finish setup.

## Combining Filters

Use Sources, Time Ranges, and Modalities together for precise queries—for example, "Chrome browsing from yesterday afternoon," or "anything I copied from Slack last week," or "meetings on my Google Calendar this month."

## Scoping a Chat to One Event

To focus the assistant on **one** specific memory or summary, open that item in [Pieces Timeline](/products/desktop/timeline), open the **three-dots menu** (⋮), and choose **`Chat`**. This opens Conversational Search with that event's context pre-loaded. See [Chat from a summary](/products/desktop/timeline/event-actions#chat-from-a-summary) for details.

For broader scoping across many memories, use **Sources**, **Time Ranges**, and **Modalities** above.

***

Learn how to set additional context for your conversations in [Setting Additional Context](/products/desktop/conversational-search/setting-context).
