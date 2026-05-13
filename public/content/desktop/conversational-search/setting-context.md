---
title: Add Context to Your Chats
path: /desktop/conversational-search/setting-context
visibility: PUBLIC
status: PUBLISHED
description: Control LTM context, chat from Timeline Events, and manage how Conversational Search accesses your workflow history.
metaTitle: Add Context to Your Chats | Conversational Search
metaDescription: Control LTM context, start chats from Timeline Events, and configure how Conversational Search uses your workflow history.
---

## LTM Context Toggle

Control whether Conversational Search includes Long-Term Memory context in your conversations. When enabled, your chats automatically draw from up to 9 months of captured workflow context.

<Callout type="info">
  LTM must be enabled to access the chat feature in Pieces Desktop. If LTM is off, chat does not work. LTM is enabled by default in conversations.
</Callout>

### Enabling or Disabling LTM Context

<Steps>
  <Step title="Click User Profile">
    Click your `User Profile` in the top left of the Pieces Desktop App.
  </Step>
  <Step title="Hover Over LTM-2.7">
    Hover over `LTM-2.7` in the dropdown menu that appears.
  </Step>
  <Step title="Toggle LTM">
    To keep LTM active, ensure it is not paused or turned off. To disable, select a pause duration (15 minutes, 1 hour, 6 hours, 12 hours, or 24 hours) or choose `Turn Off`. When paused or off, Conversational Search will not include workflow history context.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/context-integration/hovering_over_ltm_turnoff.png" alt="Toggling LTM context for Conversational Search" align="center" fullwidth="true" />

> User profile menu showing LTM-2.7 hover menu with pause and turn off options

You can also set whether LTM context is on by default for new chats in the LLM runtime settings gear.

## Starting a Conversation from a Timeline Event

Start context-specific chats directly from any Timeline Event. When you start a conversation with a Timeline Event, it opens in Conversational Search with that event's full context pre-loaded and displayed as an information card.

<Steps>
  <Step title="View Timeline Event">
    Click any event in the Pieces Timeline to view its summary in the *main panel*.
  </Step>
  <Step title="Start Related Chat">
    Click `Start Related Chat` in the bottom right of the Timeline Event detail view to open Conversational Search with that event's context loaded.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/chat-with-timeline-events/chat_with_timeline_event.png" alt="Timeline Event detail with Start Related Chat opening Conversational Search" align="center" fullwidth="true" />

> Timeline Event detail showing Start Related Chat opening Conversational Search with pre-loaded context

You can also use the **three-dots menu** (⋮) on any event and choose `Chat` to scope a conversation to that item. See [Chat from a summary](/products/desktop/timeline/event-actions#chat-from-a-summary).

## Viewing the Relevant Summaries Sidebar

After receiving a response, see exactly which Timeline Events were used to generate it.

<Steps>
  <Step title="Find Relevant Summaries Button">
    Look for the `Relevant Summaries` button at the bottom of a chat response.
  </Step>
  <Step title="Open Sidebar">
    Click the button to open the sidebar on the right side. Each entry shows the Timeline Event title, description, timestamp, and related applications.
  </Step>
  <Step title="Sort Summaries (Optional)">
    Click the sort dropdown in the top right of the sidebar—options include `Suggested`, `Recent`, and `Most Viewed`.
  </Step>
  <Step title="Click a Timeline Event">
    Click any Timeline Event to view full details about when it was captured and what context it contains.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/relevant_summaires_conversational_chat.png" alt="Relevant Summaries button showing source Timeline Events" align="center" fullwidth="true" />

> Relevant Summaries sidebar showing Timeline Events used to generate the response

***

Learn how to choose and manage AI models in [Models](/products/desktop/conversational-search/models).
