---
title: Troubleshooting
path: /web-extension/troubleshooting
visibility: PUBLIC
status: PUBLISHED
description: This page shows you how to fix common issues with the Pieces Web Extension and how to connect with the Pieces support team or community.
metaTitle: Troubleshoot Pieces Web Extension Issues
metaDescription: "Troubleshoot common issues with the Pieces Web Extension: verify that PiecesOS is running, refresh Copilot chats, and resolve cloud‑based LLM errors quickly."
---

## Having Trouble with the Pieces Web Extension?

If you're having issues with the Pieces Web Extension, try the following quick fixes and dependency checks.

<Callout type="info">
Starting with Chrome version 142 and later, you may need to grant the localhost network access permission to the extension to ensure it functions properly and has access to all of its features. Learn how to grant these permissions [here](/products/web-extension/get-started#localhost-network-access).
</Callout>

<on-device-storage />

## Check PiecesOS Status

PiecesOS, a required dependency, can cause issues with the Pieces Web Extension or other extensions and plugins if it is not installed or running.

### Run or Restart PiecesOS

Make sure PiecesOS is running on your device.

To double-check that Pieces OS is running, ensure the Pieces logo is present in your toolbar (on macOS) or your taskbar (Windows/Linux).

If it isn't there, please launch PiecesOS by double-clicking PiecesOS in your Applications folder.

### Install PiecesOS

For the Pieces Web Extension to run, PiecesOS is required. This dependency communicates with the Web Extension and provides context and other necessary data for on-device machine learning, cloud and local-hosted model usage, cloud connectivity, and more.

If you need to download and install PiecesOS, [click here.](/products/core-dependencies/pieces-os/manual-installation)

## Refreshing Copilot Chats

If you're using the Pieces Copilot chat and disconnect from WiFi or encounter issues with a cloud-based LLM, you may need to refresh the chat.

This can resolve issues such as the LLM appearing to "hang" (e.g., generating a response that turns out to be an infinite loop).

To refresh the chat, click the three vertical dots at the top-right corner of your Copilot Chat window and select `Refresh`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/web_extension/troubleshooting/hovering_refresh.png" alt="" align="center" fullwidth="true" />

## Missing Quick Actions Buttons

You may be missing the Pieces Quick Actions buttons under eligible code blocks for two main reasons:

### Disabled Buttons

Navigate to the **Settings** view to double-check that you haven't disabled the Pieces buttons from the site in your active tab. If you enable them, the page will automatically refresh, and the buttons should appear.

### No Detectable Code

On specific pages, even on sites where code block elements are frequently embedded in the Document Object Model (DOM), such as Stack Overflow, there may not be eligible code blocks under which to render the Pieces Quick Action buttons.