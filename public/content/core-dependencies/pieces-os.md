---
title: Understanding PiecesOS
path: /core-dependencies/pieces-os
visibility: PUBLIC
status: PUBLISHED
description: Read about PiecesOS, the foundational layer that supports the whole Pieces Suite, and the core functionalities—like LTM-2.7 and Timeline.
metaTitle: Understanding PiecesOS | Pieces Docs
metaDescription: Read about PiecesOS, the foundational layer that supports the whole Pieces Suite, and the core functionalities—like LTM-2.7 and Timeline.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/core_dependencies/pieces_os.png"
---

## What is PiecesOS?

PiecesOS is a background service that runs on your machine. It orchestrates local data processing and manages the house-made machine learning (ML) models used within Pieces software.

The core functionality powered by PiecesOS is [LTM-2.7](/products/core-dependencies/pieces-os#ltm-27), which enables the [Timeline](/products/desktop/timeline) feature in the Pieces Desktop App.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/figma_mockups/longtermmemory_piecesdrive_piecescopilot.png" alt="" align="center" fullwidth="true" />

> PiecesOS powering core Pieces functionality

## The Role of PiecesOS

PiecesOS provides the intelligence and power behind Pieces software in two key ways. First, it supplies the essential components of the Pieces infrastructure and supports various processes. Second, it powers standalone Pieces plugins and extensions when used without the Pieces Desktop App.

This 'brain' is required to enable the fundamental features of the Pieces development experience.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/figma_mockups/piecesos_bridging_all_products.png" alt="" align="center" fullwidth="true" />

> PiecesOS bridging all Pieces products and services

### How PiecesOS Works

Powered by PiecesOS, the Long-Term Memory (LTM-2.7) Engine tracks your development and workflow context, allowing you to access your workflow history through the Timeline.

With [Conversational Search](/products/desktop/conversational-search), you can have conversations with your captured workflow context. All AI-powered elements work together to enhance your context and creativity.

## Fundamental Components

Using the Pieces Desktop App or a Pieces plugin or extension for your favorite IDE requires PiecesOS. It is a required dependency for memory and context preservation, storing and accessing materials, and interacting with generative AI.

## LTM-2.7

The Long-Term Memory (LTM-2.7) Engine is a powerful evolution of the original LTM system, designed to store and surface workflow context from up to nine months in the past.

By automatically capturing workflow context and providing flexible memory browsing, LTM-2.7 ensures you don't lose track of code, discussions, or references—even if you return to a project weeks or months later. These workflow events and summaries can be found within the [Timeline](/products/desktop/timeline) view in the [Pieces Desktop App](/products/desktop).

<Card title="Want a Sneak Peak?" image="/assets/icons/platform_logos/pieces_logo.png">
  Here's a [quick read on some of the nano-models](https://tsavo.hashnode.dev/temporal-nano-model-breakthrough) we develop that layer into the data retrieval pipeline for LTM-2.7.
</Card>

### Deep Study

LTM-2.7 includes a powerful Deep Study feature that provides comprehensive analysis of your recent workstream activities.

Deep Study goes beyond standard workflow summaries to provide detailed insights into your development patterns, project progress, and workstream activities. This feature analyzes your recent context more thoroughly than standard summaries, helping you understand your workflow trends and identify areas for optimization.

#### Using Deep Study

Deep Study is built in by default for Pieces Pro users. In any [Conversational Search](/products/desktop/conversational-search) chat, use Deep Study by asking questions like "Can you perform a deep study on what I've done for the last few days?"

Deep Study reports typically take 10–20 minutes to generate. While running, progress indicators show a `Thinking` state and multiple cooperating agents. You can expand chevrons to view each agent's intermediate steps.

#### Model and Runtime

Deep Study always runs on a dedicated cloud LLM managed by Pieces (currently a Google model, subject to change). Changing the selected LLM via the standard runtime modal does not affect Deep Study generations.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/single-click-summaries/deep_study_actions.png" alt="" align="center" fullwidth="true" />

> Deep Study in action showing progress indicators and cooperating agents

### Grounded Assistance

Long-Term Memory is designed to boost developer productivity by providing assistance that's temporally grounded within the concrete context of your actual workflow.

This allows [Conversational Search](/products/desktop/conversational-search) to better understand your development process over time and offer more relevant and timely responses to queries, as it has a local database of information to work from. Since LTM has a local database of information to work from, it can offer relevant, timely responses to your queries:

* Recall details from older tasks or code reviews without requiring you to re-describe them
* Understand ongoing projects more holistically, anticipate next steps, and offer suggestions aligned with your actual workflow

### How Context is Captured

Under the hood, LTM monitors your workflow at the operating system level, capturing data from IDEs (e.g., changes, commits, open files), browsers (e.g., opened tabs, reference links), and collaboration tools (e.g., messaging apps, file-sharing platforms).

LTM (through PiecesOS) extends your ability to [enable or disable specific sources](/products/core-dependencies/pieces-os/quick-menu#quick-menu-actions) for data capture—this way, you can decide exactly what gets tracked and stored, providing flexibility if you have sensitive or personal workflows.

<Callout type="info">
  LTM data is stored on your device. Processing depends on your [processing mode](/products/desktop/configuration/models) and model choice: **Local** does most processing on-device but can still use an external cloud model. **Blended** and **Cloud** send context to cloud providers. [Learn more about privacy and security.](/products/privacy-security-your-data)
</Callout>

### Less Context Switching

Traditionally, AI tools require you to restate your environment—what project you're working on, the code you just wrote, or the documentation you've referenced.

However, with LTM-2.7's temporal grounding, you have reduced manual input, enhanced continuity, and intuitive interactions. [Conversational Search](/products/desktop/conversational-search) can reference stored LTM data to give you real-time, context-aware answers.

### Use Cases

Learn [how to use Pieces Long-Term Memory](/products/quick-guides/ltm-context) to capture information from your browser and retrieve it later with [Conversational Search](/products/desktop/conversational-search):

* **Capture Website Content for Later Reference** - Automatically store information from webpages or browser tabs you're viewing, without needing to copy-paste anything
* **Recall Important Details with a Single Prompt** - [Ask Conversational Search to retrieve content it previously saw](/products/quick-guides/copilot-with-context#prompt-pieces-copilot)—like secret messages, documentation, or key details from web apps
* **Track and Summarize Research Across Multiple Sites** - Let Pieces Long-Term Memory log what you've read across different websites and use that context to generate summaries or next steps
* **Simplify Context Sharing with Teammates** - Capture context once, then have Conversational Search summarize it or export it for others—great for asynchronous collaboration or hand-offs
* **Bridge Gaps Between Tools** - Pull in information from any browser-based tool or document viewer, and make it accessible directly inside Conversational Search chats

<Card title="Pieces + MCP" image="/assets/icons/platform_logos/pieces_logo.png">
  Here's another use case for you—try combining the power of Pieces Long-Term Memory with Model Context Protocol (MCP) servers with the brand new [Pieces MCP.](/products/mcp/get-started)
</Card>

## MCP Support

The Model Context Protocol (MCP) is an open framework that lets Large Language Models (LLMs) access relevant data from your device. Created by Anthropic, MCP removes the need for custom integrations by enabling tools like Claude, ChatGPT, GitHub Copilot, and Cursor to request and receive detailed, structured context.

[MCP is fully supported within the Pieces ecosystem](/products/mcp/get-started) and acts as the link between PiecesOS and external applications that need real-time, local context.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/pieces_os_main/cursor_change_documentation_from_conversation_2_agentic_demo_screenshot.png" alt="" align="center" fullwidth="true" />

> Pieces MCP integration with Cursor showing context-aware documentation changes

## Timeline

In the [Pieces Desktop App](/products/desktop), the 2nd-generation LTM comes with an incredibly powerful feature called [Timeline](/products/desktop/timeline). The Timeline view is a dedicated interface in the Pieces Desktop App that provides a continuous snapshot of your recent tasks, discussions, and code or document reviews, captured by the Long-Term Memory (LTM-2.7) Engine.

LTM continuously captures workflow context as you work, creating timeline events that summarize your activities, highlighting details such as major tasks, key decisions, and follow-up actions.

The Timeline view [lets you search for keywords, open references or links, and even launch Conversational Search chats](/products/desktop/timeline) directly from timeline events.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/timeline/exploring_pieces_timeline.gif?w=1200&format=webp&q=85" alt="" align="center" fullwidth="true" />

> Exploring timeline events in the Timeline view

### Use Cases

Explore real-world scenarios that highlight how Timeline can make collaboration easy, enhance product documentation, and simplify project context sharing:

* **Capture and Share Project Contexts** - Filter activities by project keyword to create a history of actions and conversations. Share as text, markdown, or use Conversational Search for a summary
* **Generate Documentation from Workflow** - Use Timeline events to log your process and export a searchable summary with links and context
* **Build Standup Reports or PR Summaries** - Log ticket reviews, create an activity with links and context, and use Conversational Search to summarize it for updates
* **Collaborate Asynchronously with Markdown Snapshots** - Export activities as markdown for teammates to load into their Conversational Search with full context
* **Use Filtered Snapshots in Conversational Search** - Filter activities by keyword or task and inject them into a chat for insights and documentation help

<Callout type="tip">
  This means you can revisit precisely what you worked on in the past, even if you step away from a project for weeks or months. Check out some of the [additional use cases for the Timeline view.](/products/quick-guides/ltm-prompting/workstream-activity)
</Callout>

### On-Device Data Storage

All data captured by LTM is stored locally on your device. It never leaves your device or becomes accessible to anyone, including the Pieces team, unless you choose to share it.

LTM applies on-device machine learning algorithms to filter out sensitive information and secrets, maintaining high levels of performance, security, and privacy.

## Pieces Drive

[Pieces Drive](/products/desktop/drive) is a legacy material manager that allows you to save, manage, and share developer resources. This feature will be merged with Timeline in a future update.

***

Check out the [Pieces Desktop App](/products/desktop) to see how these components work together, or explore [Conversational Search](/products/desktop/conversational-search) to learn how to talk with your memories.
