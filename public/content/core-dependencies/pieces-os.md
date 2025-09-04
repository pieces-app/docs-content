---
title: Understanding PiecesOS
path: /core-dependencies/pieces-os
visibility: PUBLIC
status: PUBLISHED
description: Read about PiecesOS, the foundational layer that supports the whole Pieces for Developers Suite, and the core functionalities—like LTM-2.7, Pieces Drive, and Pieces Copilot.
metaTitle: Understanding PiecesOS | Pieces Docs
metaDescription: Read about PiecesOS, the foundational layer that supports the whole Pieces for Developers Suite, and the core functionalities—like LTM-2, Pieces Drive, and Pieces Copilot.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/core_dependencies/pieces_os.png"
---

## What is PiecesOS?

PiecesOS is a background service that runs on your machine. It orchestrates local data processing and manages the house-made machine learning (ML) models used within Pieces software.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/figma_mockups/longtermmemory_piecesdrive_piecescopilot.png" alt="" align="center" fullwidth="true" />

There are three core pillars of Pieces functionality powered by PiecesOS: [\[1\] LTM-2.7,](/products/core-dependencies/pieces-os#ltm-25) [\[2\] Pieces Drive,](/products/core-dependencies/pieces-os#pieces-drive) and [\[3\] Pieces Copilot.](/products/core-dependencies/pieces-os#pieces-copilot)

These components make up the Pieces experience and are essential to the modern AI-powered workflow.  

## The Role of PiecesOS

PiecesOS provides the intelligence and power behind Pieces software in two key ways: by (1) supplying the essential components of the Pieces infrastructure and supporting various processes, and (2) powering standalone Pieces plugins and extensions when used without the Pieces Desktop App.

This ‘brain’ is required to enable the 3 fundamental features of the Pieces development experience.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/figma_mockups/piecesos_bridging_all_products.png" alt="" align="center" fullwidth="true" />

### How Does PiecesOS Work?

Powered by PiecesOS, the Long-Term Memory (LTM-2.7) Engine tracks your development and workflow context using the Pieces Drive, allowing you to import and export materials as needed.

Then, with Pieces Copilot, you can use cloud-based or local LLMs through Ollama to start chats that include the context you need.

This way, all AI-powered elements work together to enhance your context and creativity, especially when you need a memory boost.

## Fundamental Components

Using the Pieces Desktop App or a Pieces plugin or extension for your favorite IDE requires PiecesOS, as it is a required dependency for memory and context preservation, storing and accessing materials, and interacting with generative AI.

## LTM-2.7

The **Long-Term Memory (LTM-2.7) Engine** is a powerful evolution of the original LTM system, designed to store and surface workflow context from up to **nine months** in the past.

<Card title="Want a Sneak Peak?" image="/assets/icons/platform_logos/pieces_logo.png">
  Here’s a <a target="_blank" href="https://tsavo.hashnode.dev/temporal-nano-model-breakthrough">quick read on some of the nano-models</a> we develop that layer into the data retrieval pipeline for LTM-2.7 and the coming *LTM-2.7*
</Card>

By combining automatic “roll-ups” with flexible “memories” browsing, LTM-2.7 ensures you don’t lose track of code, discussions, or references—even if you return to a project weeks or months later.

These workflow summaries can be found within the [Workstream Activities](/products/desktop/workstream-activity) view in the [Pieces Desktop App](/products/desktop).

***

*Pieces Copilot with LTM-2.7 Context —* Pieces Desktop App

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Other%20Environments/pieces_cross_threading.png" alt="" align="center" fullwidth="true" />

***

### Grounded Assistance

Long-Term Memory is designed to boost developer productivity by providing assistance that’s temporally grounded within the concrete context of your actual workflow, allowing the Pieces Copilot to better understand your development process over time.

This helps it offer more relevant and timely responses to queries, as it has a *local database* of information to work from.

Since LTM has a local database of information to work from, it can offer **relevant, timely** responses to your queries:

* Recall details from older tasks or code reviews without requiring you to re-describe them.

* Understand ongoing projects more holistically, anticipate next steps, and offer suggestions aligned with your actual workflow.

### How Context is Captured

Under the hood, LTM monitors your workflow at the operating system level, capturing data from:

* **IDEs** (e.g., changes, commits, open files)

* **Browsers** (e.g., opened tabs, reference links)

* **Collaboration tools** (e.g., messaging apps, file-sharing platforms)

LTM (through PiecesOS) extends your ability to [enable or disable specific sources](/products/core-dependencies/pieces-os/quick-menu#quick-menu-actions) for data capture—this way, you can decide exactly what gets tracked and stored, providing flexibility if you have sensitive or personal workflows.

<Callout type="tip">
  The data captured by LTM is processed and stored entirely on your device, so you don’t need to worry about privacy and security—[which you can read more about here.](/products/privacy-security-your-data)
</Callout>

### Less Context Switching

Traditionally, AI tools require you to restate your environment—what project you’re working on, the code you just wrote, or the documentation you’ve referenced.

However, with LTM-2.7’s temporal grounding, you have:

* **Reduced Manual Input**: No more duplicating the same context or re-pasting large code blocks.

* **Enhanced Continuity**: Your interactions flow seamlessly from one coding session to the next, letting you pick up exactly where you left off.

* **Intuitive Interactions**: Ask questions like “What was I working on with John last week?” or “How do I fix that same CocoaPods issue from last Tuesday?”

Pieces Copilot can reference stored LTM data to give you real-time, **context-aware** answers.

### Use Cases

Learn [how to use Pieces Long-Term Memory](/products/quick-guides/ltm-context) to capture information from your browser and retrieve it later with a simple prompt to the Pieces Copilot:

1. **Capture Website Content for Later Reference:** Automatically store information from webpages or browser tabs you’re viewing, without needing to copy-paste anything.

2. **Recall Important Details with a Single Prompt:** [Ask the Pieces Copilot to retrieve content it previously saw](/products/quick-guides/copilot-with-context#prompt-pieces-copilot)—like secret messages, documentation, or key details from web apps.

3. **Track and Summarize Research Across Multiple Sites:** Let Pieces Long-Term Memory log what you’ve read across different websites and use that context to generate summaries or next steps.

4. **Simplify Context Sharing with Teammates:** Capture context once, then have the Pieces Copilot summarize it or export it for others—great for asynchronous collaboration or hand-offs.

5. **Bridge Gaps Between Tools:** Pull in information from any browser-based tool or document viewer, and make it accessible directly inside Pieces Copilot chats.

<Card title="Pieces + MCP" image="/assets/icons/platform_logos/pieces_logo.png">
  Here’s another use case for you—try combining the power of Pieces Long-Term Memory with Model Context Protocol (MCP) servers with the brand new [Pieces MCP.](/products/mcp/get-started)
</Card>

## MCP Support

The Model Context Protocol (MCP) is an open framework that lets Large Language Models (LLMs) access relevant data from your device.

Created by Anthropic, MCP removes the need for custom integrations by enabling tools like Claude, ChatGPT, GitHub Copilot, and Cursor to request and receive detailed, structured context.

[MCP is fully supported within the Pieces ecosystem](/products/mcp/get-started) and acts as the link between PiecesOS and external applications that need real-time, local context.

***

*Pieces MCP —> Cursor*

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/pieces_os_main/cursor_change_documentation_from_conversation_2_agentic_demo_screenshot.png" alt="" align="center" fullwidth="true" />

***

## Workstream Activity

In the [Pieces Desktop App](/products/desktop), the 2nd-generation LTM comes with an incredibly powerful feature called [Workstream Activity](/products/desktop/workstream-activity).

The Workstream Activity view is a dedicated interface in the Pieces Desktop App that provides a continuous snapshot of your recent tasks, discussions, and code or document reviews, captured by the **Long-Term Memory (LTM-2.7)** **Engine.**

Every 20 minutes, LTM generates a *roll-up* that summarizes your workflow context for that period, highlighting details such as major tasks, key decisions, and follow-up actions.

***

*Reviewing a LTM Roll-up —* Pieces Desktop App

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Desktop%20App/gif_of_exploring_rollups.gif" alt="" align="center" fullwidth="true" />

***

In addition to offering a timeline of roll-ups, the Workstream Activity view [lets you search for keywords, open references or links, and even launch Pieces Copilot Chats](/products/desktop/workstream-activity#interacting-with-roll-ups) directly from a summarized entry.

By surfacing relevant data right when you need it, the Workstream Activity feature [eliminates the frustration of recounting your background](/products/quick-guides/ltm-prompting/workstream-activity) or re-pasting massive prompts every time you want AI assistance—empowering you to focus on high-value work instead.

### Use Cases

Explore real-world scenarios that highlight how Workstream Activities can make collaboration easy, enhance product documentation, and simplify project context sharing:

1. **Capture and Share Project Contexts:** Filter activities by project keyword to create a history of actions and conversations. Share as text, markdown, or use Pieces Copilot for a summary.

2. **Generate Documentation from Workflow:** Use Workstream Activity Rollups to log your process and export a searchable summary with links and context.

3. **Build Standup Reports or PR Summaries:** Log ticket reviews, create an activity with links and context, and use Copilot to summarize it for updates.

4. **Collaborate Asynchronously with Markdown Snapshots:** Export activities as markdown for teammates to load into their Pieces Copilot with full context.

5. **Use Filtered Snapshots in Copilot Chats:** Filter activities by keyword or task and inject them into a chat for insights and documentation help.

<Callout type="tip">
  This means you can revisit precisely what you worked on in the past, even if you step away from a project for *weeks* or *months.*

  Check out some of the [additional use cases for the Workstream Activity view.](/products/quick-guides/ltm-prompting/workstream-activity)
</Callout>

### On-Device Data Storage

All data captured by the LTM is stored locally on your device. It never leaves your device or becomes accessible to anyone, including the Pieces team, unless you choose to share it.

LTM applies on-device machine learning algorithms to filter out sensitive information and secrets, maintaining high levels of performance, security, and privacy.

For advanced components that require blended processing, user preferences can be set to leverage a cloud-powered Large Language Model as the Copilot’s runtime. 

## Pieces Drive

Pieces Drive is an intelligent and interactive material manager baked into PiecesOS that allows you to save, manage, and share important developer resources such as notes, useful code snippets, links, and more within your personal local repository.

You can view, edit, reuse, and share these materials via Pieces Shareable Links from this repository. 

***

*Viewing Saved Materials with Pieces Drive —* Pieces Desktop App

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Drive/Searching%20%26%20Filtering%20Materials/pieces_drive.png" alt="" align="center" fullwidth="true" />

***

### Multi-Tool Integration

With PiecesOS, you can use Pieces Drive in tools like [Obsidian](/products/obsidian) and [Raycast](/products/raycast), as well as your favorite code editors, such as <a target="_blank" href="/products/extensions-plugins/jetbrains">IntelliJ</a>, <a target="_blank" href="/products/extensions-plugins/visual-studio-code">Visual Studio Code</a>, and <a target="_blank" href="/products/extensions-plugins/sublime">Sublime Text</a>.

You can also view and adjust metadata saved with your materials in the Applet View of Pieces plugins or the Pieces Desktop App.

### AI-Powered Enrichment

When you save code or other useful materials to Pieces Drive, AI automatically enriches them with a wide variety of useful metadata.

The enrichment process, powered by on-device ML models, provides:

* annotations

* anchors

* shareable links

* related links

* related people

* suggested searches

* tags

* sensitive information

* date created

* source of origin

<Callout type="alert">
  Pieces will also identify and flag any sensitive information, like API keys or personal data, and flag this information under **Sensitive Information.**
</Callout>

## Pieces Copilot

Like Pieces Drive, Pieces Copilot can be found nested within Pieces plugins and extensions or the Pieces Desktop App.

It can generate code, answer questions, add code documentation, and serve as the bridge between you and your workflow context, as captured by the LTM-2.7.

***

*Pieces Copilot for Code Generation —* Pieces Desktop App

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/new_pos_media/generating_code.png" alt="" align="center" fullwidth="true" />

***

### Introducing Context to Chats

If you encounter a scenario where you need to recall a specific URL to a Firestore database that was used during a live demo with another coworker, you can use Pieces Copilot (with LTM enabled) to recall that *exact link.*

### Understanding Code

Pieces Copilot helps you comprehend complex code snippets by providing explanations, detailing how specific functions work, and suggesting alternative implementations for that code.

Try asking it alternative ways to handle logging, or more robust methods of error handling—give it an entire file, an entire *project,* or just a function.

### Code Generation

By specifying your requirements for a function or script, Pieces Copilot can generate code that seamlessly fits into your active file.

Use Pieces Copilot and Pieces Drive together to generate boilerplate code or adjust a function. Then, save it to the Pieces Drive with enriched metadata for future use, saving time.

### Error Handling

Debugging, checking logs, and handling errors are often the toughest parts of coding. But with Pieces Copilot, you can debug code thoroughly using the Pieces Desktop App or your preferred plugin.

Context-based debugging is powerful because generative AI, whether cloud-based or local, can understand code semantics beyond what's visible and within the project's scope to find solutions and fixes.

You might even be able to finally center that `div`—seriously, we’ve actually done it.
