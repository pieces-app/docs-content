---
title: Get Started
path: /extensions-plugins/visual-studio-code/get-started
visibility: PUBLIC
status: PUBLISHED
description: Follow the steps below to install and use the Pieces for VS Code Extension.
metaTitle: Getting started with the Pieces for Visual Studio Code Extension
metaDescription: Learn how to install and set up the Pieces for VS Code Extension to manage snippets and leverage AI-powered assistance in your coding workflow.
---

<pieces-pro-cta />

## Prerequisites

Before installation, you'll need:

* **PiecesOS:** The main engine that powers Pieces for VS Code functionality. [Learn more about PiecesOS.](/products/core-dependencies/pieces-os)

* **VS Code:** Visual Studio Code should already be installed on your development machine.

<Callout type="alert">
  PiecesOS must be installed to enable the Pieces for VS Code Extension. For enhanced functionality, we also recommend the Pieces Desktop App.
</Callout>

### Sign in Required

Pieces requires all users to sign in before using any plugins or extensions. You'll be prompted to authenticate if you haven't already. For help, see our [sign-in guide](/products/meet-pieces/sign-into-pieces).

## Setting Up PiecesOS

To use the <a target="_blank" href="https://marketplace.visualstudio.com/items?itemName=MeshIntelligentTechnologiesInc.PiecesVisualStudio">Pieces for VS Code Extension</a>, you must install <a target="_blank" href="/products/core-dependencies/pieces-os">PiecesOS</a> on your operating system.

Follow the specific setup steps below:

<get-started-install />

## Installation

1. Open VS Code and navigate to the **Extensions** view, then search for **Pieces for VS Code** and click `Install`

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair_2/visual_studio_code/vsc_marketplace.png" alt="" align="center" fullwidth="true" />

<Callout type="info">
  Alternatively, download the .VSIX installer from the <a target="_blank" href="https://marketplace.visualstudio.com/items?itemName=MeshIntelligentTechnologiesInc.PiecesVisualStudio">VS Code Marketplace</a> and install it manually.
</Callout>

2. Restart VS Code after installing the extension to complete the setup.

3. Enable **Pieces Tool Windows** by going to `View`, then `Tool Windows`, and enable whichever Pieces Windows that best suit your workflow

### Updating

The <a target="_blank" href="https://marketplace.visualstudio.com/items?itemName=MeshIntelligentTechnologiesInc.PiecesVisualStudio">Pieces for VS Code Extension</a> will automatically update when a new version is available.

<Callout type="tip">
  The `Auto Update` setting is enabled by default.
</Callout>

### Pieces Cloud

Connecting to the Pieces Cloud is optional. However, it **provides additional features** like **data backups, shareable links, and more.** You can enjoy the main functionalities of Pieces without an account.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/updated_vs_screenshots/main/connect_to_cloud.png" alt="" align="center" fullwidth="true" />

Disconnecting from the Pieces Cloud logs you out of your Pieces account.

To disconnect from the Pieces Cloud:

<Steps>
  <Step title="Open the Command Palette">
    Open the command palette in VS Code with `⌘+shift+p` (macOS) or `ctrl+shift+p` (Windows/Linux)
  </Step>

  <Step title="Disconnect from the Cloud">
    Enter `Pieces: Disconnect from Pieces Cloud` and choose the option
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/get_started/disconnect_from_pieces_cloud.gif" alt="" align="center" fullwidth="true" />

## Onboarding

The Pieces for VS Code extension includes an interactive walkthrough that shows the different steps in one panel. This onboarding page will teach you how to save, view, and use saved materials and fully utilize Pieces for Visual Studio Code.

### Save Your First Material

When you click `Save Your First Material`, Pieces automatically opens the [Pieces Drive](/products/extensions-plugins/visual-studio-code/drive) and stores a sample snippet to show you how everything works.

You’ll see that snippet immediately in the Saved Materials list, giving you a quick demonstration of how Pieces captures items and organizes themes.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/get_started/opening_example_snippet.png" alt="" align="center" fullwidth="true" />

### View Your Saved Materials

By clicking `View Your Saved Materials`, Pieces Drive will open up to your **Saved Materials**—showing you any saved snippets you had before and the newly generated saved snippet.

### Check Out the Pieces Copilot

Clicking `Open Your Copilot` triggers the Pieces Copilot side panel, as shown in the screenshots. In the Pieces Copilot, you’ll find **suggested prompts**, options to set context from folders or files, and quick links to your saved materials.

Once you open the Copilot, the onboarding step is marked as complete. You're ready to ask [questions about your code](/products/extensions-plugins/visual-studio-code/copilot/chat), [document it](/products/extensions-plugins/visual-studio-code/copilot/documenting-code), or [refactor a selected material](/products/extensions-plugins/visual-studio-code/copilot/refactoring)—all within the VS Code interface.

### Ask Copilot with Your Material

When you click `Ask Copilot about Your Material`, Pieces automatically adds the newly saved snippet to the Copilot chat with a sample prompt (like “What does this code do?”). Press `Enter` to send your snippet to the Copilot, and you’ll immediately receive an explanation or suggested improvements.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/get_started/ask_about_material.png" alt="" align="center" fullwidth="true" />

### Supercharge Your Workflow

Clicking `Pieces Documentation` opens our guide with advanced tips, setup instructions, and best practices. Choosing `View All Steps` lets you revisit any onboarding step at any time.

The right side includes extra resources and helpful videos, including community channels and tutorials, to help you master Pieces and maintain a smooth development flow.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/get_started/supercharge_workflow.png" alt="" align="center" fullwidth="true" />

<Callout type="info">
  If you need extra support, you can find [helpful resources here](/products/support).
</Callout>

## Uninstallation

To uninstall the Pieces for VS Code Extension, press `⌘+shift+x` (macOS) or `ctrl+shift+x` (Windows/Linux) to open the extensions tab. Then, search for the `Pieces for VS Code` extension and click `Uninstall`.

<Callout type="alert">
  Restart your VS Code IDE after removing the extension to complete the uninstallation process.
</Callout>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair_2/visual_studio_code/vsc_marketplace_uninstall.png" />