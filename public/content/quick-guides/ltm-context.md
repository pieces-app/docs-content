---
title: Using Long-Term Memory Context
path: /quick-guides/ltm-context
visibility: PUBLIC
status: PUBLISHED
description: Get started using the Pieces Long-Term Memory to recall information from a webpage.
metaTitle: How to use Long-Term Memory context | Pieces Docs
metaDescription: Discover how to use Long-Term Memory context in Pieces to effortlessly recall past work, retrieve information, and enhance productivity
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/quick_guides/quick_guides.png"
---

## Prerequisites

To complete this Quick Guide, you’ll need:

1. **The Pieces Desktop App** installed and actively running on your device.

2. **Long-Term Memory** enabled in the Pieces Desktop App.

To enable the LTM-2.5 Engine from PiecesOS, click the PiecesOS icon to open the [Quick Menu](/products/core-dependencies/pieces-os/quick-menu#ltm-2-engine) on Windows or macOS, then select `Enable Long-Term Memory Engine`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/quick_guides/using_long_term_memory_context/disabling_long_term_memory.gif" alt="" align="center" fullwidth="true" />

## In This Quick Guide

In this Quick Guide, you’ll use [Pieces Long-Term Memory](/products/core-dependencies/pieces-os#ltm-25) to save context from a website, then prompt the Pieces Copilot to tell you what it saw.

<Card title="Want a Sneak Peak?" image="/assets/icons/platform_logos/pieces_logo.png">
  Here’s a <a target="_blank" href="https://tsavo.hashnode.dev/temporal-nano-model-breakthrough">quick read on some of the nano-models</a> we develop that layer into the data retrieval pipeline for LTM-2.5 and the coming *LTM-2.7*
</Card>

This demonstrates how Pieces can capture information from any application and make it available to you in the Pieces Copilot.

### Capture Context

With LTM enabled, Pieces captures workflow context from every actively used window, including the browser you’re using to read this Quick Guide.

<Steps>
  <Step title="Generate a Secret Message">
    <a target="_blank" href="https://pieces.app/magic-moments/ltm">Click this link</a> to generate a message Pieces can capture in a new tab.
  </Step>

  <Step title="Let Pieces Capture Your Context">
    Read the message and give Pieces a second or two to capture the context from your browser.
  </Step>
</Steps>

### Prompt the Copilot

Now that Pieces has captured the message, you can prompt the Pieces Copilot through the Pieces Desktop App to retrieve the secret message.

<Steps>
  <Step title="Open the Pieces Desktop App">
    Open the Pieces Desktop App and start a new chat or use an existing chat.
  </Step>

  <Step title="Prompt the Pieces Copilot">
    Use the following prompt with the Pieces Copilot:

    ```plaintext
    What is my secret message?
    ```
  </Step>
</Steps>