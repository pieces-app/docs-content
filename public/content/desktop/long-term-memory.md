---
title: Long-Term Memory
path: /desktop/long-term-memory
visibility: PUBLIC
status: PUBLISHED
description: Discover how Pieces Long-Term Memory (LTM-2.7) captures, enriches, and indexes your workflow context to power AI-driven insights.
metaTitle: Long-Term Memory (LTM-2.7) | Pieces Docs
metaDescription: Learn how Pieces Long-Term Memory Engine captures workflow context from your applications, browser, and code editor to provide personalized AI assistance.
---

<Embed
  src="https://youtu.be/vg4Mg8Xasn8"
  title="Introduction to Pieces Long-Term Memory and how to enable LTM Audio"
/>

***

## What is Long-Term Memory?

**Long-Term Memory (LTM-2.7)** is Pieces' on-device memory engine that continuously captures, enriches, and indexes contextual information from your daily workflow. LTM monitors your active applications, clipboard activity, screen captures, and audio input to build a comprehensive, searchable memory of your work.

Unlike traditional note-taking or code snippet tools that require manual saving, Long-Term Memory **automatically captures** workflow moments as they happen—storing code you copy, tracking conversations you have, and remembering decisions you make.

All captured context is processed and stored **entirely on your device**, ensuring your workflow data remains private and secure.

## How Long-Term Memory Works

LTM-2.7 uses on-device machine learning to process and enrich workflow events in real-time:

1. **Capture** - Monitors clipboard, screen, audio, and application activity
2. **Enrich** - Extracts text, code, URLs, and metadata from captured events
3. **Index** - Creates searchable vectors for semantic retrieval
4. **Connect** - Links related events, conversations, and code snippets

The result is a **personal, searchable knowledge graph** of your workflow that powers [Conversational Search](/products/desktop/conversational-search), [Timeline](/products/desktop/timeline), and context-aware AI interactions via [MCP integrations](/products/mcp).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/introducing_pieces_mcp/mcp-diagram.png" alt="Pieces Long-Term Memory architecture showing data flow from applications to PiecesOS to AI tools" align="center" fullwidth="true" />

> Long-Term Memory captures workflow context from your applications and makes it accessible to AI tools via PiecesOS

## What Gets Captured

Long-Term Memory tracks multiple types of workflow context:

### Clipboard Events
Code snippets, terminal commands, error messages, and text you copy are automatically captured and enriched with language detection, syntax highlighting, and related context.

### Screen Captures
Screenshots and screen recordings are analyzed with OCR (Optical Character Recognition) to extract visible text, making even visual content searchable through Conversational Search.

### Audio Transcription
With **LTM Audio** enabled, Pieces can transcribe system audio (meetings, videos, podcasts) and microphone input (your voice during calls) to capture spoken context from your workflow.

<Callout type="info">
  LTM Audio is a Preview feature requiring system permissions. See [LTM Audio setup](/products/desktop/configuration/long-term-memory#ltm-audio) for platform-specific instructions.
</Callout>

### Application Activity
The Long-Term Memory Engine monitors which applications you use, what windows you focus on, and what URLs you visit—providing temporal context for when and where workflow events occurred.

## Use Cases and Benefits

### Context-Aware AI Assistance

When using [Conversational Search](/products/desktop/conversational-search) or [MCP-integrated AI tools](/products/mcp), Long-Term Memory enables AI assistants to understand your project history, past decisions, and workflow patterns.

**Example queries:**
- *"What did we decide about authentication in last week's standup?"*
- *"Show me the error message I saw yesterday when deploying to staging"*
- *"Have I encountered this React hook issue before?"*

### Timeline & Workflow Insights

Long-Term Memory powers [Timeline](/products/desktop/timeline), which organizes your workflow events chronologically and generates automatic summaries like Day Recap, Morning Brief, and What's Top of Mind.

### Cross-Application Context

Because LTM captures context from multiple sources (IDE, browser, terminal, meetings), Pieces can connect related information across applications—showing you code snippets related to a bug you discussed in a meeting, or documentation you read while debugging.

### Privacy-First Design

All Long-Term Memory processing happens **on your device**. Your workflow context never leaves your machine unless you explicitly choose to:
- Share materials via [Pieces Drive (legacy)](/products/desktop/drive)
- Use cloud models in [Conversational Search](/products/desktop/conversational-search)
- Enable cloud sync (optional)

Learn more about [privacy and data storage](/products/core-dependencies/on-device-storage).

## Enabling Long-Term Memory

Long-Term Memory is enabled by default when you install Pieces Desktop. You can verify or toggle LTM status in settings:

<Steps>
  <Step title="Open User Profile">
    Click your `User Profile` in the top left of Pieces Desktop.
  </Step>

  <Step title="Navigate to Settings">
    Hover over `Settings` and select `Long-Term Memory`.
  </Step>

  <Step title="Verify LTM Status">
    Check that "Long-Term Memory Engine: On" shows with a green indicator. If off, click the toggle to enable.
  </Step>
</Steps>

For detailed configuration options, see [Long-Term Memory Settings](/products/desktop/configuration/long-term-memory).

## Controlling What Gets Captured

You have fine-grained control over what Long-Term Memory captures:

### App Access Control
Choose which applications LTM can monitor. Disable specific apps (like password managers or private browsing) to exclude them from capture.

### System Permissions
Grant or revoke accessibility and screen recording permissions on macOS, Windows, or Linux to control LTM's ability to capture screen and application context.

### Clear Stored Data
Remove captured LTM data for specific time ranges (last 7 days, last 30 days, or all time) without disabling the engine.

See [LTM Configuration](/products/desktop/configuration/long-term-memory) for step-by-step guides.

## How AI Tools Access LTM

Long-Term Memory is accessible to AI assistants via **two pathways**:

### 1. Conversational Search (Pieces Desktop)
Chat with your memories directly in the Pieces Desktop app. Ask questions about your workflow, and Pieces retrieves relevant context from LTM.

<FancyCard title="Conversational Search" href="/products/desktop/conversational-search" colored={false}>
  Chat with your Long-Term Memory to ask questions about your workflow, retrieve past context, and get AI-powered insights.
</FancyCard>

### 2. MCP Integrations (IDEs & AI Tools)
Connect AI coding assistants like Cursor, VS Code, and GitHub Copilot to your Long-Term Memory via Model Context Protocol. Your AI assistant can query LTM to provide context-aware code suggestions and answers.

<FancyCard title="MCP Server" href="/products/mcp" colored={false}>
  Connect 20+ AI tools and IDEs to your Long-Term Memory for context-aware coding assistance.
</FancyCard>

## Performance and Resource Usage

Long-Term Memory runs efficiently in the background with minimal impact:

- **CPU Usage:** Low-priority background processing during idle time
- **Memory:** ~200-500 MB RAM for ML models (unloaded when inactive)
- **Storage:** Variable based on captured content (typically 1-5 GB)

You can optimize system resource usage by unloading ML models from memory when not in use. See [Performance Settings](/products/desktop/configuration/long-term-memory#performance).

## Learn More

<FancyCard title="LTM-2.7 Engine (PiecesOS)" href="/products/core-dependencies/pieces-os/long-term-memory" colored={false}>
  Enable, pause, and control LTM from the PiecesOS Quick Menu—including Audio and Access Control.
</FancyCard>

<FancyCard title="Privacy & On-Device Storage" href="/products/core-dependencies/on-device-storage" colored={false}>
  Understand how Pieces stores data locally and what privacy controls you have.
</FancyCard>

<FancyCard title="LTM Settings" href="/products/desktop/configuration/long-term-memory" colored={false}>
  Configure app access control, system permissions, LTM Audio, and clear stored data.
</FancyCard>

***

## Next Steps

Now that you understand Long-Term Memory, explore how to use the context it captures:

- **[Timeline](/products/desktop/timeline)** - View chronological workflow events and auto-generated summaries
- **[Conversational Search](/products/desktop/conversational-search)** - Chat with your memories to retrieve past context
- **[MCP Integrations](/products/mcp)** - Connect AI coding assistants to your Long-Term Memory

***

If you need help troubleshooting Long-Term Memory, visit [Pieces Support](/products/support) for guides and community resources.
