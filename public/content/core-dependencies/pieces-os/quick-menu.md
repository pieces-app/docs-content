---
title: Quick Menu
path: /core-dependencies/pieces-os/quick-menu
visibility: PUBLIC
status: PUBLISHED
description: Manage PiecesOS settings, LTM, MCP, ML processing, and updates from the menu bar or system tray.
metaTitle: Quick Menu | PiecesOS
metaDescription: Use the PiecesOS Quick Menu to manage Long-Term Memory, MCP integrations, ML processing, updates, and more from your menu bar or system tray.
---

## Overview

The **Quick Menu** is a lightweight popover for interacting with PiecesOS, located in your menu bar (macOS & Linux) or system tray (Windows). Use it to manage your account, toggle Long-Term Memory, configure ML processing, and check for updates—all without launching a separate application.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/core-dependencies/pos_quick-menu_overview.png" alt="PiecesOS Quick Menu overview on macOS" align="center" fullwidth="true" />

> PiecesOS Quick Menu on macOS (Windows shares the same UI)

## Quick Menu at a Glance

| **Section** | **What it does** |
| --------------------------------- | -------------------------------------------------------------------------- |
| *Account* | Log in or log out of your Pieces account |
| *Version* | Check for and install PiecesOS updates |
| *Long-Term Memory Engine* | Enable, pause, or disable LTM |
| *Long-Term Memory Access Control* | Choose which apps LTM captures data from |
| *MCP Servers* | View the SSE endpoint URL and MCP documentation links |
| *Settings* | Launch on login, enabled apps, ML processing, telemetry, memory optimization |
| *Resources* | Links to documentation, support, and community |

## Account

At the top of the Quick Menu, log in or out of your Pieces account. Logging in enables cloud-connected features like preference syncing and cloud model processing. Logging out keeps PiecesOS running locally with saved configurations.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/core-dependencies/quick-menu_account_overview.png" alt="PiecesOS Quick Menu account login and logout options" align="center" fullwidth="true" />

## Checking for Updates

Below your account, the Quick Menu displays your current PiecesOS version. If an update is available, click `Update Available` to install it. Otherwise, a green check mark confirms you're current.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/core-dependencies/quick-menu_check_for_updates.png" alt="PiecesOS Quick Menu update status and version info" align="center" fullwidth="true" />

## Long-Term Memory

Toggle the [LTM-2.7 Engine](/products/core-dependencies/pieces-os/long-term-memory) on or off, manage [Audio ingestion](/products/core-dependencies/pieces-os/long-term-memory#ltm-audio), and control which apps LTM captures data from via [Access Control](/products/core-dependencies/pieces-os/long-term-memory#long-term-memory-access-control).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/core-dependencies/quick-menu_turn_off_ltm.png" alt="Toggling LTM engine on or off in the Quick Menu" align="center" fullwidth="true" />

For the full breakdown—pausing, disabling, Audio setup, per-app toggles—see the [LTM-2.7 Engine](/products/core-dependencies/pieces-os/long-term-memory) page.

## MCP Servers

Find the SSE endpoint URL for creating your own Pieces MCP instances, plus links to setup guides for [Cursor](/products/mcp/cursor), [VS Code](/products/mcp/github-copilot), and other IDEs.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/core-dependencies/quick-menu_mcp_options.png" alt="MCP Server options and SSE endpoint in the Quick Menu" align="center" fullwidth="true" />

## Settings

### ML Processing

Control how PiecesOS handles AI model inference. Switch between **Blended Mode** (local + cloud) and **Local Mode** (fully on-device, no cloud). Fine-tune enrichment levels per application.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/new_pos_media/ml_blending.png" alt="ML processing mode selection between Blended and Local" align="center" fullwidth="true" />

### Optimize Memory Usage

Adjusts memory allocation for PiecesOS to reduce resource consumption while maintaining performance.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/core-dependencies/quick-menu_ml_processing.png" alt="ML processing and memory optimization settings" align="center" fullwidth="true" />

### Launch on Login

Enable or disable automatic PiecesOS startup when your computer boots.

### Enabled Apps

View which applications have active Pieces MCP integrations.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/new_pos_media/enabled_apps.png" alt="List of enabled Pieces MCP integrations" align="center" fullwidth="true" />

### Telemetry Sharing

Enable or disable telemetry data collection per application or MCP integration.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/new_pos_media/telemetry_pos.png" alt="Telemetry sharing settings for individual applications" align="center" fullwidth="true" />

## Resources

Quick access to documentation, support, and community links.

<Tabs>
  <TabItem title="Links">
    * <a target="_blank" href="https://pieces.app/about">About</a>
    * <a target="_blank" href="/">Documentation</a>
    * <a target="_blank" href="/products/support">Support</a>
  </TabItem>

  <TabItem title="Follow Us">
    * <a target="_blank" href="https://discord.com/invite/ubn8JFAXQ7">Discord</a>
    * <a target="_blank" href="https://x.com/getpieces">X</a>
    * <a target="_blank" href="https://www.linkedin.com/company/getpieces">LinkedIn</a>
    * <a target="_blank" href="http://github.com/pieces-app">GitHub</a>
    * <a target="_blank" href="https://www.youtube.com/@getpieces">YouTube</a>
  </TabItem>
</Tabs>

## Linux

The Quick Menu on Linux has a reduced set of options:

* **Discover Integrations** — Opens the Pieces website with all [MCP integrations](/products/mcp)
* **About** — Launches the <a target="_blank" href="https://pieces.app/about">About</a> page
* **Documentation** — Opens the <a target="_blank" href="/">Pieces documentation</a>
* **Submit Feedback or Issues** — Opens a form for bug reports and feedback. You can also <a target="_blank" href="/products/support">visit our Support page</a>.
* **Optimize Memory Usage** — Reduce PiecesOS resource consumption
* **Quit** — Stops PiecesOS. Relaunch by typing `pieces-os` in your terminal.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/pieces_os_main/quick_menu/linux_quick_menu.png" alt="PiecesOS Quick Menu on Linux" align="center" fullwidth="true" />
