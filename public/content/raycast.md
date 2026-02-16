---
title: Raycast Extension
path: /raycast
visibility: PUBLIC
status: PUBLISHED
description: Learn more about the Pieces Raycast Extension.
metaTitle: Using Pieces for Raycast | Pieces Docs
metaDescription: Understand the benefits and importance of using the Pieces Raycast Extension, and get started with Quickstart and Commands.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair/raycast/raycast.png" alt="" align="center" fullwidth="true" />

***

<Callout type="alert">
  V2 Documentation for the Pieces extension for the Raycast productivity tool is under construction.

  In the meantime, you can look at the V1 documentation for the Pieces for Raycast Extension below.\`
</Callout>

***

<pieces-pro-cta />

## Pieces for Raycast Extension

The Pieces Raycast Extension provides powerful features that allow you to streamline your workflow and boost productivity.

With just a few keystrokes, you can capture, search, and manage code snippets from anywhere on your desktop—*without switching context.*

## Prerequisites

* **PiecesOS** must be installed and running

* <a target="_blank" href="https://www.raycast.com">Raycast</a> must be installed on your Mac

### Sign in Required

Pieces requires all users to sign in before using any plugins or extensions. You'll be prompted to authenticate if you haven't already. For help, see our [sign-in guide](/products/meet-pieces/sign-into-pieces).

## PiecesOS Installation Guide

Before using the Pieces for Raycast Extension, you must install PiecesOS on your macOS device.

PiecesOS powers all of Pieces' core functionalities, including snippet saving, enrichment, and integration handling.

<Callout type="tip">
  Pieces captures *no identifiable user data.* Our local-only architecture means your data never has to leave your device.
</Callout>

[Download the standalone PiecesOS file](/products/core-dependencies/pieces-os/manual-installation#macos) for your macOS system’s ARM or Intel-based architecture to start the installation process.

*Your device must be updated to macOS 13.0 (Ventura) or higher.*

1. Download the correct PiecesOS file for your system’s architecture.

2. From your **Downloads** folder, double-click the installed PiecesOS file to open it.

3. Drag PiecesOS into the application folder if prompted, then open PiecesOS.

### Configuring Permissions

Two permission prompts will pop up on your screen when installing PiecesOS.

```markdown
PiecesOS is an app downloaded from the internet. Are you sure you want to open it?
```

Click `Open` to continue with the installation.

Then, you’ll see a second permissions pop-up message:

```markdown
PiecesOS is requesting to bypass the system private window picker and directly access your screen and audio. This will allow PiecesOS to record your screen and system audio, including personal or sensitive information that may be visible or audible.
```

Click `Allow`.

These permissions are required for [PiecesOS](/products/core-dependencies/pieces-os) to power the [Long-Term Memory Engine (LTM-2.7)](/products/core-dependencies/pieces-os#ltm-27).

PiecesOS will automatically open in your toolbar and pop up a *Notification preferences modal* in the upper right corner of your screen.

### Enabling the LTM-2.7 Engine

To do this, open the PiecesOS Quick Menu and click `Enable Long-Term Memory Engine`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/core-dependencies/quick-menu_turn_off_ltm.png" alt="" align="center" fullwidth="true" />

## Install the Pieces for Raycast Extension

If this is your first time installing a Raycast extension, refer to [Raycast’s extension install guide](https://developers.raycast.com/basics/install-an-extension).

To install the Pieces Extension:

1. Open **Raycast**

2. Navigate to the **Raycast Store**

3. Search for *“Pieces for Raycast”*

4. Click `Install`

### Launch and Use the Extension

Once the extension is installed on your device:

1. Open Raycast

2. Search for the command: `Search Saved Snippets`

3. Use this command to browse and reuse your saved code

<Callout type="tip">
  You can use a custom keyboard shortcut to quickly launch Raycast. See the [**Raycast Hotkey Manual** to learn more.](https://manual.raycast.com/hotkey)
</Callout>

## Features

The Raycast Extension lets you capture code snippets and other developer materials from multiple sources, reuse them on the fly, and manage your account without switching applications.

## Pieces Drive

[Pieces Drive](/products/meet-pieces/fundamentals#pieces-drive) is your personal, intelligent snippet library—automatically curated and enriched as you work.

In the Raycast Extension, Pieces Drive serves as the backend engine that stores, indexes, and organizes the content you capture through various commands.

By integrating tightly with [PiecesOS](/products/core-dependencies/pieces-os), Pieces Drive ensures your saved materials are enriched with metadata like language, source, and context. This makes your content instantly searchable and more valuable over time as your snippet collection grows.

### Search Saved Materials

Quickly search across all of your saved code snippets using Raycast’s minimal interface.

This command surfaces results enriched with metadata such as title, language, tags, and source (e.g., clipboard, browser, editor). It’s a fast way to rediscover useful context you’ve captured in the past, without digging through files, emails, or browser tabs.

<Image src="https://old.docs.pieces.app/assets/raycast/search_snippets.gif" alt="" align="center" fullwidth="true" />

Use this feature when:

* You want to reuse a snippet you saved earlier

* You don’t remember exactly where you used it but recall its purpose

* You want to avoid rewriting boilerplate or repeatedly googling common code

### Save Clipboard History

This command displays a timeline of your clipboard history—enriched with metadata and usage context.

You can scroll through recently copied content and selectively save high-value items as persistent snippets. Each saved snippet includes its origin, content type, and timestamp, helping you retain the most relevant fragments of your workday.

<Image src="https://old.docs.pieces.app/assets/raycast/save_clipboard_history.gif" alt="" align="center" fullwidth="true" />

### Save Clipboard to Pieces

You can quickly save the current content in your clipboard to Pieces.

This command is perfect for moments when you quickly copy a block of code, a command, or a snippet of text and want to ensure its preservation.

<Image src="https://old.docs.pieces.app/assets/raycast/save_clipboard.gif" alt="" align="center" fullwidth="true" />

### Save Browser History to Pieces

This command allows you to surface code snippets that you recently interacted with in your browser, such as on Stack Overflow, GitHub, or blog posts.

Pieces identifies these snippets in your browser activity and gives you the option to save them with proper enrichment and metadata.

<Image src="https://old.docs.pieces.app/assets/raycast/save_browser_history.gif" alt="" align="center" fullwidth="true" />

### Save Finder Selection

Select one or more files in macOS Finder and save them to Pieces with a single command.

Files are stored as artifacts in your Pieces Library and enriched with metadata like filename, extension, and path.

<Image src="https://old.docs.pieces.app/assets/raycast/save_finder_selection.gif" alt="" align="center" fullwidth="true" />

### Save Selection in Any App

Highlight any text in the currently active (frontmost) application—like VS Code, Terminal, Safari, or Slack—and instantly save it to Pieces.

This command enables frictionless, cross-app snippet capture without copy/paste.

<Image src="https://old.docs.pieces.app/assets/raycast/save_frontmost_selection.gif" alt="" align="center" fullwidth="true" />

## Account Access

Connecting your Pieces account allows you to unlock the full potential of the ecosystem, including cloud sync, cross-device access, and personalized context enrichment.

From within Raycast, you can quickly authenticate or sign out of your account to manage how your data is stored and accessed.

<Callout type="tip">
  While Pieces can be used fully offline, logging in enables advanced features such as secure backup, account-linked snippet history, and enhanced AI-powered enrichment.
</Callout>

### Sign-in to Pieces

This command securely authenticates your Pieces account from within Raycast, enabling cloud sync, cross-device access, and personalization features.

Once signed in, your saved snippets are backed up and available wherever Pieces is installed.

<Image src="https://old.docs.pieces.app/assets/raycast/sign_in_to_pieces.gif" alt="" align="center" fullwidth="true" />

### Sign out of Pieces

Log out of your Pieces account from Raycast.

<Image src="https://old.docs.pieces.app/assets/raycast/signout.gif" alt="" align="center" fullwidth="true" />

<Callout type="tip">
  This is useful for switching accounts, temporarily disabling cloud syncing, or handing off a machine to another developer.
</Callout>

## Configuration

While most of the configuration happens automatically, here are some helpful notes:

* **PiecesOS must be running** for the Raycast Extension to function.

* If you’re not signed in, use the `Sign into Pieces` command to authenticate.

* Advanced features like auto-enrichment and snippet metadata rely on PiecesOS settings, which can be adjusted via the [Pieces Desktop App](/products/desktop/configuration) or the [PiecesOS Toolbar.](/products/core-dependencies/pieces-os/quick-menu)

## Troubleshooting

Use this section to diagnose problems, follow step-by-step fixes, and understand when to escalate an issue to the support team.

Pieces is built with resilience, but we know bugs can happen, and we're here to help when they do.

### Node.js Installation Screen Appears

When you first use a Pieces command in Raycast, you may see a prompt to install Node.js. In some cases, this installation might fail or not complete.

<Steps>
  <Step title="Initial Attempt">
    Follow the on-screen prompts to install Node.js.
  </Step>

  <Step title="If Installation Fails">
    Fully close Raycast, then reopen Raycast and try the command again.
  </Step>

  <Step title="If the Issue Persists">
    Visit our [support page](/products/support) for help.
  </Step>
</Steps>

## Data Privacy & Security

All data captured by the Raycast Extension is saved locally by default and never shared externally unless you explicitly enable cloud sync.

Your clipboard contents, browser-captured snippets, and Finder selections are handled securely through PiecesOS.

Learn more in our [Privacy Policy and Security Documentation.](/products/privacy-security-your-data)

<on-device-storage />