---
title: Context & Project Integration
path: /desktop/conversational-search/context-integration
visibility: PUBLIC
status: PUBLISHED
description: Toggle LTM context, open Conversational Search scoped to a Timeline summary via Chat, and review source Timeline Events.
metaTitle: Context & Project Integration | Conversational Search
metaDescription: Control LTM context in Conversational Search, scope a chat from a Timeline summary with Chat, and verify which Timeline Events informed a response.
---

## Context & Project Integration

Control whether Conversational Search includes Long-Term Memory context in your conversations. When enabled, Conversational Search has access to 9 months of captured workflow context from your [Long-Term Memory (LTM-2.7)](/products/core-dependencies/pieces-os#ltm-27) Engine, including code you've written, conversations you've had, and decisions you've made.

<Callout type="info">
  LTM must be enabled to access the chat feature in Pieces Desktop. If LTM is off, chat does not work. LTM is enabled by default in conversations.
</Callout>

## LTM Context Toggle

Enable or disable Long-Term Memory context for Conversational Search. When enabled, your chats automatically include workflow history context. When disabled, conversations use only the current context without historical data.

### Enabling LTM Context

Turn on Long-Term Memory context to include workflow history in your chats:

<Steps>
  <Step title="Click User Profile">
    Click your `User Profile` in the top left of the Pieces Desktop App.
  </Step>
  <Step title="Hover Over LTM-2.7">
    Hover over `LTM-2.7` in the dropdown menu that appears.
  </Step>
  <Step title="Manage LTM-2.7">
    A menu will appear with options to pause LTM-2.7 or turn it off. To enable LTM context for Conversational Search, ensure LTM-2.7 is not paused or turned off.
  </Step>
</Steps>

### Disabling LTM Context

Turn off Long-Term Memory context when you want conversations without historical workflow data:

<Steps>
  <Step title="Click User Profile">
    Click your `User Profile` in the top left of the Pieces Desktop App.
  </Step>
  <Step title="Hover Over LTM-2.7">
    Hover over `LTM-2.7` in the dropdown menu.
  </Step>
  <Step title="Pause or Turn Off">
    Select a pause duration (15 minutes, 1 hour, 6 hours, 12 hours, or 24 hours) or choose `Turn Off` to disable LTM-2.7. When LTM-2.7 is paused or turned off, Conversational Search will not include workflow history context in conversations.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/context-integration/hovering_over_ltm_turnoff.png" alt="Toggling LTM context for Conversational Search" align="center" fullwidth="true" />

> User profile menu showing LTM-2.7 hover menu with pause and turn off options

## Understanding LTM Context

When LTM-2.7 is enabled, Conversational Search automatically includes relevant workflow context from your Long-Term Memory. This means your conversations can reference:

* Code you've written and changes you've made
* Conversations and decisions from your workflow history
* Activities captured by LTM-2.7 from connected applications
* Timeline Events and summaries from your workflow

When LTM-2.7 is paused or turned off, Conversational Search operates without access to this historical context, providing responses based only on the current conversation.

<Card title="Want to learn more about using LTM Context?" image="/assets/icons/platform_logos/pieces_logo.png">
  Check out the [LTM Prompting Guide](/products/quick-guides/ltm-prompting) or learn how to use [Conversational Search with LTM Context](/products/quick-guides/copilot-with-context) via these Quick Guides.
</Card>

## Scoping a chat from Timeline

Conversational Search does **not** let you attach arbitrary local **files** or **folders** to a chat. To work with a **specific** captured memory—such as a workflow summary or Timeline Event—open it in [Pieces Timeline](/products/desktop/timeline), then use the **`Chat`** action on that item’s **three-dots menu** (⋮). That opens Conversational Search with that memory in scope.

For the full walkthrough, see [Chat from a summary](/products/desktop/timeline/event-actions#chat-from-a-summary) on the Event Actions page.

You can still narrow **which** memories are in play across a normal chat with **Sources** and **Time Ranges**; see [Filtering your searches](/products/desktop/conversational-search/using-conversational-search#filtering-your-searches).

## Related Timeline Events

View which Timeline Events were used to generate responses by opening the Relevant Summaries sidebar.

Conversational Search draws from your LTM memories to provide accurate responses. The Relevant Summaries sidebar shows you exactly which Timeline Events were used to generate each response, helping you verify the source of information and discover related work.

### Viewing Related Timeline Events

Open the Relevant Summaries sidebar to see which Timeline Events were used in a response:

<Steps>
  <Step title="Find Relevant Summaries Button">
    After receiving a response in Conversational Search, look for the `Relevant Summaries` button at the bottom of the chat response.
  </Step>
  <Step title="Open Sidebar">
    Click the `Relevant Summaries` button to open the sidebar on the right side of the interface.
  </Step>
  <Step title="Review Timeline Events">
    The sidebar displays a list of relevant Timeline Events that were used to generate the response. Each entry shows the Timeline Event title, description, timestamp, and related applications.
  </Step>
  <Step title="Sort Summaries (Optional)">
    Click the sort dropdown in the top right of the sidebar to change how summaries are organized. Options include `Suggested`, `Recent`, and `Most Viewed`.
  </Step>
  <Step title="Click a Timeline Event">
    Click any Timeline Event in the sidebar to view full details about that event, including when it was captured and what specific context it contains.
  </Step>
  <Step title="Close Sidebar">
    Click the `X` icon in the top left of the sidebar to close it and return to the main chat view.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/relevant_summaires_conversational_chat.png" alt="Relevant Summaries button showing source Timeline Events" align="center" fullwidth="true" />

> Relevant Summaries sidebar open showing Timeline Events used to generate the response, with sort dropdown visible in the top right

***

## Next Steps

Now that you know how to control LTM context in Conversational Search, learn how to start context-specific conversations directly from your workflow memories.

[Starting a conversation with a Timeline Event →](/products/desktop/conversational-search/chat-with-timeline-events)
