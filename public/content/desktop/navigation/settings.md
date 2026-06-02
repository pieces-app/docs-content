---
title: Settings
path: /desktop/navigation/settings
visibility: PUBLIC
status: PUBLISHED
description: Customize, adjust, and configure PiecesOS and the Pieces Desktop App to suit your workflow and privacy preferences. 
metaTitle: Navigating Pieces Desktop Settings | Pieces Docs
metaDescription: Customize your Pieces Desktop experience with settings for workflow optimization, integrations, and AI-powered assistance.
---

## Overview

The `Settings` page in Pieces contains all configurable options, adjustable preferences, and modifiable behaviors for the Desktop Application.

You can customize the Pieces Desktop App to your coding workflow by integrating external services or customizing the interface.

## Accessing Settings

To access settings, press `⌘+,` (macOS) or `ctrl+,` (Windows/Linux).

You can also open the **Power Menu**, type ‘settings’ in the search field, and select `Go To Settings` from the dropdown menu.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Settings/settings.png" alt="Settings window with category sidebar" align="center" fullwidth="true" />

## Understanding the Settings Layout

When you open **Settings**, you'll see categories in the left sidebar and an `All` tab at the top.

In Pieces 6.0, the sidebar includes **Account**, **Long-Term Memory**, **MCP**, **Connectors**, **Appearance**, and **Troubleshooting**. Click any category to show its options, or select `All` to view every setting at once.

From your profile menu, quick paths jump directly to **LTM-2.7**, **LTM Sources**, **LTM Audio**, or full **Settings**.

### Account & Integrations

In this section, you can integrate external services with Pieces and adjust your user details, beginning with [Account Information.](/products/desktop/configuration/account)

This area displays your email address and any linked accounts.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Settings/Account%20%26%20Cloud/account_integrations.png" alt="Accounts and Cloud Integrations modal" align="center" fullwidth="true" />

If you’re interested in testing upcoming features, the **Early Access Program** lets you join beta releases and stay ahead of the curve.

### Personal Cloud

The Personal Cloud settings are now part of the [Account](/products/desktop/configuration/account) tab and control how your snippets and materials sync across devices.

You'll see a status for your cloud connection (including the last sync time), plus options to set or modify your personal domain.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Configure/disconnect_cloud.png" alt="Personal Cloud connect and disconnect controls" align="center" fullwidth="true" />

There's also a `Backup & Restore Data` feature to preserve or retrieve your snippets from the cloud whenever needed.

* `Status`: Check if your cloud is connected and see when it last synced.

* `Domain`: Update your personal domain.

* `Backup & Restore Data`: Protect your snippets and data.

### Long-Term Memory

The [Long-Term Memory](/products/desktop/configuration/long-term-memory) settings allow you to manage the Long-Term Memory Engine, control which applications Pieces can access, manage system permissions, optimize performance, and clear stored data.

* `Long-Term Memory Engine`: Toggle the engine on or off to control workflow context capture.

* `App Access Control`: Manage which applications the Long-Term Memory Engine interacts with.

* `System Permissions`: Manage accessibility and screen permissions for LTM.

* `Optimize System RAM Usage`: Unload local machine learning models from memory.

* `Clear LTM Data`: Remove persisted data captured by the Long-Term Memory Engine.

### Model Context Protocol (MCP)

The [MCP](/products/desktop/configuration/mcp) tab shows server URLs and setup links for integrating Pieces with Cursor, GitHub Copilot, Goose, and other MCP-compatible tools.

### Connectors

[Connectors](/products/desktop/connectors) link external services (such as Google Calendar) so Pieces can read calendar context and perform actions on your behalf.

* `Connect`: Authorize a service from the Connectors pane.

* `Status`: See which connectors are connected.

### Models (in chat)

In Pieces 6.0, you choose AI models from the picker in [Conversational Search](/products/desktop/conversational-search/models), not from a top-level Settings category. For Ollama setup and processing modes, see [Models settings](/products/desktop/configuration/models) if your build still exposes that page.

### Appearance

In the [Appearance](/products/desktop/configuration/appearance) tab, customize the overall appearance of Pieces.

Switch between light or dark mode, select an accent color for UI highlights, adjust font size and weight, and configure visual density to control spacing and layout.

These controls help you create a comfortable coding environment for extended sessions.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Settings/Aesthetics/changing_colors.png" alt="Accent color picker in Appearance settings" align="center" fullwidth="true" />

### Troubleshooting

The [Troubleshooting](/products/desktop/configuration/troubleshooting) settings provide access to support resources, documentation links, version information, and feedback channels.

You can view PiecesOS and Desktop App version information, check for updates, access product documentation, report issues on GitHub, book support calls, and control how much crash or compliance data is shared under Privacy settings in Account.

* `Online Resources`: Access product documentation and GitHub issues.

* `Get In Touch`: Book support calls, contact the team, or visit the support hub.

* `PiecesOS Information`: View version, port, and check for updates.

* `Desktop App Information`: View version, platform details, and check for updates.

* `Privacy`: Configure telemetry and diagnostics settings (found in Account settings).