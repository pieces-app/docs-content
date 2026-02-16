---
title: Pieces Desktop App
path: /desktop
visibility: PUBLIC
status: PUBLISHED
description: The Pieces Desktop Application features a set of AI tools designed to help users and knowledge workers make smart choices every day.
metaTitle: Pieces Desktop Application
metaDescription: Boost productivity with the Pieces Desktop App – AI-powered tools that use workflow context to enhance decision-making with generative AI.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/pfd_docs_figmas/all_logos.png" alt="" align="center" fullwidth="true" />

> Pieces Desktop App logos and branding

## Meet the Pieces Desktop App

The Pieces Desktop Application contains a suite of AI-powered tools designed to improve productivity by utilizing your workflow context and enabling you to make intelligent decisions on a day-to-day basis with Pieces Long-Term Memory.

Powered by [PiecesOS](/products/core-dependencies/pieces-os)—the heart and soul of Pieces—the Pieces Desktop app is the ultimate assistant for code, context, and creativity.

<CardGroup cols={2}>
  <Card title="Getting Started" image="/assets/icons/pieces_os_light.svg">
    Follow these instructions to download and install the Pieces Desktop Application for [macOS](/products/meet-pieces/macos-installation-guide), [Windows](/products/meet-pieces/windows-installation-guide), or [Linux](/products/meet-pieces/linux-installation-guide).
  </Card>

  <Card title="Support" image="/assets/icons/platform_logos/pieces_logo.png">
    Explore troubleshooting options, visit our [support page](/products/support), or <a target="_blank" href="https://calendar.app.google/WVUDtUfNy5Vst3sH7">book a call</a> directly with our engineers.
  </Card>
</CardGroup>

<guides-overview-card />

## Overview

The Pieces Desktop app is designed to act as a hub for the Pieces Suite, powered by PiecesOS and the [Long-Term Memory (LTM-2.7)](/products/core-dependencies/pieces-os#ltm-27) Engine.

With the Pieces Desktop App, you have access to dedicated views for the context captured by Long-Term Memory through [Pieces Timeline](/products/desktop/timeline).

## Pieces Timeline

Keep track of your workflow so you can access stored context from yesterday, last week, or even last month—whenever you need it. The [Long-Term Memory (LTM-2.7)](/products/core-dependencies/pieces-os#ltm-27) Engine ensures that nothing slips through the cracks.

[Pieces Timeline](/products/desktop/timeline) provides a sleek UI for interacting with saved data from up to 9 months ago in an easily digestible format, allowing you to view timeline events, workstream summaries, single-click summaries, and conversational searches.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/timeline/exploring_pieces_timeline.gif" alt="" align="center" fullwidth="true" />

> Pieces Timeline showing workflow events, summaries, and activity graph visualization

<FancyCard title="Learn More" href="/products/desktop/timeline" colored={false}>
  Explore Pieces Timeline features including filtering events, managing event actions, and understanding timeline contents.
</FancyCard>

## Single-Click Summaries

Generate instant, contextual summaries from your workflow using preset summary types. With [Single-Click Summaries](/products/desktop/single-click-summaries), you can instantly generate contextual summaries with one click. Choose from summary types like *What's Top of Mind*, *Standup Update*, *Custom Summary*, *Day Recap*, *AI Habits*, and *Discover*—to quickly access insights about your workflow without typing a single prompt.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/timeline/queued_summaries_in_timeline.png" alt="" align="center" fullwidth="true">

> Showing Pieces with Timeline open and Single-Click Summaries Generating

<FancyCard title="Learn More" href="/products/desktop/single-click-summaries" colored={false}>
  Discover all available summary types and learn how to generate, view, and manage your summaries.
</FancyCard>

## Conversational Search

Use [Conversational Search](/products/desktop/conversational-search) as your main chat interface, where you'll find suggested prompts to help you get started. Query your workflow memories and get AI-powered insights about your past activities.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/conversational_chat_view.png" alt="" align="center" fullwidth="true" />

> Conversational Search interface showing chat interface and suggested prompts

<FancyCard title="Learn More" href="/products/desktop/conversational-search" colored={false}>
  Learn how to use Conversational Search, integrate context, and chat with timeline events.
</FancyCard>

## Configuration

Customize your Pieces Desktop App experience through *Settings*, which includes options for Account (with Personal Cloud and Telemetry), Long-Term Memory, Models, Copilot Chats, Machine Learning, Model Context Protocol (MCP), Connected Applications, Views & Layouts, Appearance, and Troubleshooting.

<FancyCard title="Learn More" href="/products/desktop/configuration" colored={false}>
  Explore all configuration options to customize your Pieces Desktop experience.
</FancyCard>

## Model Context Protocol (MCP) Support

The Pieces suite, powered by the LTM-2.7 Engine through PiecesOS, also provides support for [Model Context Protocol (MCP) servers](/products/mcp/get-started) through Server-Sent Events (SSEs).

With the Pieces MCP, you can thread rich workflow context through to [Cursor](/products/mcp/cursor), [GitHub Copilot](/products/mcp/github-copilot), [Goose](/products/mcp/goose), and other IDEs and productivity tools, making Pieces a platform for using long-term context in other workflows outside of just the Pieces Desktop App.

<Callout type="tip">
  To integrate the Pieces MCP into one of the available integrations, copy the SSE endpoint URL and/or `.json` schema into your IDE of choice.

  You can find the MCP URL inside the *Model Context Protocol (MCP)* tab within *Settings*.
</Callout>

***

*Pieces MCP → Cursor*

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/misc/cursor_ask_about_youtube_tutorial.png" alt="" align="center" fullwidth="true" />

> Pieces MCP integration with Cursor showing workflow context threading

***

If Pieces Desktop isn't what you're looking for, check out [PiecesOS](/products/core-dependencies/pieces-os) to learn about the core engine powering Pieces, or explore [Extensions & Plugins](/products/extensions-plugins) to integrate Pieces into your favorite IDE or editor.
