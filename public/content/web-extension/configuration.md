---
title: Configuration
path: /web-extension/configuration
visibility: PUBLIC
status: PUBLISHED
description: Read the guide below to set up the Pieces Web Extension to fit your workflow and preferences.
metaTitle: Supported LLMs & Extension Settings
metaDescription: Discover 54+ local and cloud LLMs in the Pieces Web Extension, learn to configure Copilot runtimes, adjust settings, and switch models seamlessly.
---

## Supported LLMs

We regularly update and configure our plugins and extensions to work with the latest LLMs.

The Pieces Web Extension currently [supports a range of cloud-hosted and local LLMs](/products/large-language-models) from your favorite providers, such as Anthropic, Google, OpenAI, Microsoft, and more.

[Read documentation on switching your Pieces Copilot Runtime (LLM)](/products/web-extension/copilot/llm-settings#how-to-configure-your-llm-runtime) utilized by the Pieces Web Extension.

## Opening Pieces Settings

To open the settings within the Pieces Web Extension, follow these steps:

<Steps>
  <Step title="Open the Pieces Web Extension">
    From your browser’s extensions list, select the `Pieces icon`.
  </Step>

  <Step title="Click the Three Bars">
    In the top-right of the extension, select the `sandwich` icon.
  </Step>

  <Step title="Open the Settings">
    After opening the horizontal bar menu, select the `Settings` button. This will open the available settings for the Pieces Web Extension.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/web_extension/configuration/opening_settings.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

## Settings Overview

Below is a breakdown of each adjustable setting (preferences, behaviors, views, etc.) available in the Pieces Web Extension, updated according to the latest features.

### Account & Cloud Integrations (*Beta*)

Displays your Pieces account details and cloud‑integration status.

* **Profile & Early Access**: Your name, email, GitHub link, and Early Access enrollment

* **Personal Cloud**: Connection status, last sync time, and custom domain (e.g., `nolanworksat.pieces.cloud`)

### Backup & Restore Data

Trigger a manual backup of your local data to the cloud or restore from a snapshot.

### Copilot LLM Runtime

Choose which language model powers Copilot in the extension (e.g. GPT‑4o Mini, GPT‑4o).

<Callout type="tip">
  You can switch between local and cloud models here using the `cloud` and `desktop` icons.
</Callout>

### Accent Color

Select the UI accent color used throughout the extension (Blue, Green, Purple, etc.).

### Use Long‑Term Memory (LTM-2) Context by Default

When checked, your saved long‑term memory is automatically included in every Pieces Copilot query without needing to re-enable LTM chat-by-chat.

### Delete All Copilot Chats…

Clears all saved Pieces Copilot chat history inside the Pieces Web Extension.

<Callout type="alert">
  This action is *not reversible.* Clearing your chat history is a permanent action.
</Callout>

### Saved Material Auto‑Enrichment

Choose how much automatic enrichment occurs when saving materials. This can be beneficial for speed and performance on older systems, or if you’re utilizing local-only LLMs.

* **None**: No metadata

* **Low**: Basic metadata

* **Medium**: Intermediate metadata (3–6 data points)

* **High**: Extensive metadata (6+ data points)

### ML Processing

Choose how Pieces utilizes cloud and local LLMs to process context and power other Pieces features.

* **Processing Mode**: Cloud‑based / Local (on‑device) / Blended

* **Long‑Term Memory Engine**: On/off toggle and engine version (e.g., LTM‑2)

### Long‑Term Memory Source Control

When generating context, choose which sources (chats, visited pages, etc.) the LTM-2 engine draws context from.

This can also be done within the PiecesOS Quick Menu in the `Long-Term Memory Engine Access Control` panel.

### Clear Long‑Term Memory Engine Data…

Delete persisted memory captured by the LTM engine for a specified time range.

### Enable Pieces Buttons by Default

Automatically shows the floating Pieces button on every webpage, so your extension is always running.

### Enable Pieces Buttons for This Site

Toggle the Pieces toolbar on or off for just the current domain.

### Button Placement

Position the floating action button (Bottom Left, Bottom Right, etc.).

### Button Color

Use the action button's light or dark theme to match your browser.

### Minimum Number of Characters for a Code Block

Set the minimum character count before the extension recognizes a code block. This is helpful for blacklisting short, one-line code elements, like terminal commands.

### Code Block Actions

Configure which actions (copy, save snippet, run tests, etc.) appear on detected code blocks.

### Number of Recent Websites to Save Snippets For

Limit how many domains Pieces will track for snippet‑saving history.

### Append Recent Websites

If checked, newly visited domains are automatically added to your “recent websites” list.

### Save Visited Websites for Context

Include the page’s metadata and content whenever you save a snippet. These websites can then be referenced and added as context to future Pieces Copilot chats.

### Telemetry & Diagnostics

Opt in or out of sharing anonymous usage metrics and crash reports.

### Documentation

Quick link to the official extension documentation.

### Submit Feedback/Issues

Open the feedback form or GitHub issues page for bugs and feature requests.

### PiecesOS Version

Shows the version of your local PiecesOS service (e.g. 11.3.1).

### Check for PiecesOS Updates

Manually check for updates to your local PiecesOS installation.

### PiecesOS Port

Displays the port (default: 39300) on which your local PiecesOS server is actively listening & posting requests to.

***

For additional support resources, check out our [troubleshooting guide.](/products/web-extension/troubleshooting)