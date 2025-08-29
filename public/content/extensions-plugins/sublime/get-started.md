---
title: Get Started
path: /extensions-plugins/sublime/get-started
visibility: PUBLIC
status: PUBLISHED
description: Follow the steps below to install and use the Pieces for Sublime Text Plugin.
metaTitle: Getting Started with Pieces for Sublime | Pieces Docs
metaDescription: Install and set up the Pieces for Sublime Text Plugin to integrate AI-powered assistance into your coding workflow.
---

<pieces-pro-cta />

## Sublime Prerequisites

Before you begin, make sure you have:

* **PiecesOS:** The core engine that powers all Pieces extensions. [Learn more about PiecesOS.](/products/core-dependencies/pieces-os)

* **Sublime Text:** Make sure you’ve installed Sublime Text on your development machine.

You must have <a target="_blank" href="https://beta.docs.pieces.app/products/core-dependencies/pieces-os">**PiecesOS**</a> to use the Pieces for Sublime Plugin. We also recommend downloading the Pieces for Developers Desktop App.

### Sign in Required

Pieces requires all users to sign in before using any plugins or extensions. You'll be prompted to authenticate if you haven't already. For help, see our [sign-in guide](/products/meet-pieces/sign-into-pieces).

## Installing the Pieces for Sublime Text Plugin

Start by installing Package Control, a required dependency for installing plugins and other tools within the Sublime Text environment.

Visit the <a target="_blank" href="https://packagecontrol.io/installation">Package Control installation page</a> and follow the instructions to install Package Control in Sublime Text.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair_2/sublime/marketplace_page_sublime.png" alt="" align="center" fullwidth="true" />

<Steps>
  <Step title="Open Command Palette">
    Use the shortcut `⌘+shift+p` (macOS) or `ctrl+shift+p` (Windows/Linux) to open the command palette
  </Step>

  <Step title="Install Pieces Plugin">
    Using the command palette, search for `Package Control: Install Package`, then search for `Pieces` and select it
  </Step>

  <Step title="Restart Sublime">
    After installing the Pieces Plugin, restart the Sublime editor to ensure all the dependencies are loaded properly
  </Step>
</Steps>

### Setting up PiecesOS

<a target="_blank" href="/products/core-dependencies/pieces-os">PiecesOS</a> is required for the <a target="_blank" href="https://packagecontrol.io/packages/Pieces">Pieces for Sublime Text Plugin</a> to work.

If you haven’t installed it yet, click the buttons to download PiecesOS via the recommended method, or follow the alternative steps below.

## Updating

The Pieces for Sublime Text Plugin will automatically update when a new version is available via `Package Control`.

When the plugin updates, you’ll see a small success message pop-up in the center of your Sublime Text Editor.

<Callout type="tip">
  **Update notifications** cover updates for both the Pieces for Sublime Text and PiecesOS.
</Callout>

You can also manually update the plugin by opening your Command window in Sublime Text by using `⌘+shift+p` (macOS) or `ctrl+shift+p` (Windows/Linux), locating the `Package Control: Upgrade Package`, and clicking the option.

This will auto-update the Pieces for Sublime Text Plugin.

## Disconnect from Pieces Cloud

Connecting to the Pieces Cloud is optional. However, it **provides additional features** like **data backups, shareable links, and more.** You can enjoy the main functionalities of Pieces without an account.

<Callout type="info">
  Disconnecting from the Pieces Cloud logs you out of your Pieces account.
</Callout>

To disconnect from the Pieces Cloud:

<Steps>
  <Step title="Open the Command Palette">
    Open the command palette
  </Step>

  <Step title="Disconnect the Cloud">
    Select `Pieces: Disconnect from Pieces Cloud`

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/getting_started/disconnect_from_pieces_cloud_sublime.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

## Onboarding

The Pieces for Sublime Text plugin has an interactive walkthrough that shows all the steps in one panel. This onboarding page guides you on saving, viewing, and using saved materials, helping you get the most out of the Pieces for Sublime Text plugin.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/getting_started/whole_onboarding.png" alt="" align="center" fullwidth="true" />

### PiecesOS Installation

If PiecesOS is not installed or running on your system, you can launch it here. This section allows you to install or open PiecesOS directly from within Sublime.

### Create your First Snippet

When you click `creation`, Pieces will automatically generate you a sample snippet in a new tab and give you a few steps that will walk you through saving a snippet—right click on the snippet, hover over `Pieces`, and select `Save to Pieces`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/getting_started/save_first_snippet.png" alt="" align="center" fullwidth="true" />

### View your Saved Snippets

Click `View Your Saved Materials`—Pieces Drive will open to your **Saved Materials**, displaying any snippets you saved before and the newly generated snippet.

### Search for your Saved Snippet

After clicking `searching`, a prompt window opens up where you can search for your snippet with [three optional ways to search](/products/extensions-plugins/sublime/drive/search-reuse).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/getting_started/seearching_snippets.png" alt="" align="center" fullwidth="true" />

### Ask for Help

After clicking the prompt, `Ask for help and get those bugs fixed`, PiecesOS will open a new snippet with a hidden bug in a new window and guide you through the process of fixing it. You can `right-click` the snippet, hover over `Pieces`, go to `Quick Actions`, and select `Fix a bug`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/getting_started/fixing_bug_onboarding.gif" alt="" align="center" fullwidth="true" />

### Pieces Copilot

This is when you're introduced to opening Pieces Copilot. When you select `Copilot`, Pieces will open a new tab with Pieces Copilot ready for a prompt!

Once you open the Copilot, the onboarding step is done. You can now ask [questions about your code](/products/extensions-plugins/sublime/copilot/chat), [document it](/products/extensions-plugins/sublime/copilot/documenting-code), [debug errors](/products/extensions-plugins/sublime/copilot/debugging-errors), or [refactor selected material](/products/extensions-plugins/sublime/copilot/refactoring)—all within the Sublime Text interface.

### Explain

You might encounter some sections of code, whether from GitHub or something you haven't looked at in a while. Pieces provides an explanation feature to help you understand what's going on in the code—this section shows you how to use it.

When you click `explanation`, a new tab will open. Right-click, hover over `Pieces`, go to `Ask Copilot`, and select `Explain`.

### Explore the Features

The final three steps provide useful information to help you use PiecesOS without any problems. Select `documentation` to access this guide and learn more about Pieces for Sublime Text.

If you encounter more issues than expected, select `Pieces: Get Support` to access our support right away.

If you have more questions or want to join the Pieces community, select `Pieces: About` in step 10, which will open a tab with all our community and support links.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/getting_started/pieces_about.png" alt="" align="center" fullwidth="true" />

## Uninstalling

To uninstall the Pieces for Sublime Text Plugin, open your Command window in Sublime Text by using `⌘+shift+p` (macOS) or `ctrl+shift+p` (Windows/Linux), locating the `Package Control: Remove Package`, looking for the option `Pieces` and clicking the option.

In order for Pieces to be completely uninstalled from the Sublime Text, you'll need to restart the IDE.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/getting_started/uninstalling_pieces_sublime_plugin.gif" alt="" align="center" fullwidth="true" />

<Callout type="tip">
  Restart your Sublime Text editor after uninstalling the plugin to complete to uninstallation process.
</Callout>