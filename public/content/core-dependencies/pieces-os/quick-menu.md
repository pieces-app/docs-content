---
title: PiecesOS | Quick Menu
path: /core-dependencies/pieces-os/quick-menu
visibility: PUBLIC
status: PUBLISHED
description: Read the documentation and see visual demonstrations of the PiecesOS Quick Menu for macOS, Windows, and Linux.
metaTitle: PiecesOS | Quick Menu
metaDescription: Read documentation and see visuals demonstrations of the PiecesOS Quick Menu for macOS, Windows, and Linux.
---

## Overview

The **Quick Menu** is a lightweight interface for interacting with PiecesOS, located in your menu bar (macOS & Linux) or system tray (Windows).

This popover lets you manage your PiecesOS settings, Long-Term Memory (LTM-2.7) Engine configurations, and application integrations.

It enables you to monitor PiecesOS status, toggle memory and AI processing settings, and access critical resources without launching a separate application, among other features.

[For Linux users, available options are currently more limited.](/products/core-dependencies/pieces-os/quick-menu#linux)

## Quick Menu Actions

There are several views and buttons you can click to expand or enter in the PiecesOS Quick Menu on macOS and Windows:

***

| **View / Button**                 | **Explanation**                                                                                                                            |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| *Account*                         | You can log in or log out of your Pieces Account.                                                                                          |
| *Version*                         | Check for and automatically install available PiecesOS updates.                                                                            |
| *Long-Term Memory Engine*         | Enable or disable LTM.                                                                                                                     |
| *Long-Term Memory Access Control* | Enable or disable sources from which LTM captures contextual workflow data.                                                                |
| *Settings*                        | Adjust settings like launch on login, enabled Pieces products, ML processing configurations, telemetry permissions, or optimize RAM usage. |
| *Resources*                       | Find links to documentation and Pieces social accounts.                                                                     |

***

*PiecesOS Quick Menu on macOS*

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/core-dependencies/pos_quick-menu_overview.png" alt="" align="center" fullwidth="true" />

<Callout type="alert">
  The PiecesOS Quick Menu shares the same user interface (UI) as the Quick Menu on Windows.

  Media for this Quick Menu documentation has been **captured exclusively on macOS.**
</Callout>

### Logging In & Out

At the top of the Quick Menu, you can **log in or log out** of your Pieces account. Logging in allows access to cloud-connected features, such as:

* Syncing preferences across devices

* Cloud model processing (if enabled)

* Accessing saved snippets across devices

If you log out, PiecesOS will continue running locally with saved configurations but will not sync to the cloud.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/core-dependencies/quick-menu_account_overview.png" alt="" align="center" fullwidth="true" />

### Checking for Updates

Directly under your account information, the Quick Menu displays your current PiecesOS version and whether it is up to date.

* If a new update is available, you will see an `Update Available` button. Clicking it will initiate the update process.

* If PiecesOS is up to date, the menu will display a green check mark and show the active version—i.e., 11.0.4.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/core-dependencies/quick-menu_check_for_updates.png" alt="" align="center" fullwidth="true" />

## LTM-2.7 Engine

LTM is PiecesOS’s core memory engine, capturing workflow context locally to enhance productivity.

You can toggle it on or off from the Quick Menu.

### Enabling, Pausing & Disabling LTM

You can toggle the LTM engine **On** or **Off** from the Quick Menu.

To do so, click the `Pieces` logo in your taskbar or toolbar, and click `Enable Long-Term Memory Engine` to enable it.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/core-dependencies/quick-menu_turn_off_ltm.png" alt="" align="center" fullwidth="true" />

Conversely, you can click the green `On` button to display a drop-down menu that lets you disable the LTM temporarily in minute increments or altogether.

### Long-Term Memory Access Control

This section allows you to manage which applications and sources LTM captures data from through two menus:

1. **Enabled Sources**

This view displays a list of apps from which LTM is actively gathering data (e.g., Google Chrome, ChatGPT).

Clicking on an enabled source opens a window where you can choose to disable it.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/new_pos_media/quick_menu_known_icons.png" alt="" align="center" fullwidth="true" />

## MCP Menu

Pieces is fully integrated with MCP functionality and now ships with an in-house MCP protocol that passes workflow context captured by Long-Term Memory to your favorite IDEs, such as Cursor, VS Code, and more.

You can find the SSE endpoint URL for creating your own Pieces MCP instances, as well as links to related documentation, in the `Model Context Protocol (MCP) Servers` menu.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/core-dependencies/quick-menu_mcp_options.png" alt="" align="center" fullwidth="true" />

## Settings

The `Settings` menu allows you to configure PiecesOS to best suit your workflow.

### Optimize Memory Usage

Adjusts memory allocation for PiecesOS to reduce resource consumption while maintaining performance.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/core-dependencies/quick-menu_ml_processing.png" alt="" align="center" fullwidth="true" />

### Launch on Login

You can enable or disable automatic startup for PiecesOS when your computer boots up.

### Enabled Apps

View a list of applications that have Pieces plugins and extensions installed.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/new_pos_media/enabled_apps.png" alt="" align="center" fullwidth="true" />

### Telemetry Sharing

Enable or disable telemetry data collection on an individual application, plugin, or extension basis.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/new_pos_media/telemetry_pos.png" alt="" align="center" fullwidth="true" />

### ML Processing

This menu controls how PiecesOS manages AI model inference. You can use `Blended Mode` or `Local Mode` to switch between using a combination of local and cloud-based LLMs for performance, or purely on-device processing with no cloud dependencies.

You can also make changes to the enrichment to level and type to individual applications for more fine-tuned control.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/new_pos_media/ml_blending.png" alt="" align="center" fullwidth="true" />

### Resources

The `Resources` provides quick access to documentation, support, and community links:

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

***

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/new_pos_media/resources.png" alt="" align="center" fullwidth="true" />

## Linux

The Pieces Quick Menu on Linux contains several helpful resources and links, such as:

* **Discoverer Integrations:** Opens the Pieces website, where you can find all <a target="_blank" href="https://pieces.app/plugins">Pieces browser and IDE extensions and plugins</a>.

* **About:** Launches the <a target="_blank" href="https://pieces.app/about">About</a> page for Pieces.

* **Documentation:** Brings you to the official <a target="_blank" href="/">Pieces documentation</a>, where you can browse through guides and troubleshooting information for the entire Pieces Suite.

* **Submit Feedback or Issues:** If you're experiencing an issue, click this button to open a webpage with a form for submitting bug reports or providing feedback. <a target="_blank" href="/products/support">You can also</a>[ visit our Support page here to do so.](/products/support)

* **Optimize Memory Usage:** Adjusts memory allocation for PiecesOS to reduce resource consumption while maintaining performance.

* **Quit:** Quits PiecesOS. To relaunch, open your terminal and type `pieces-os` and press `enter` or find the PiecesOS launcher from your application tray.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/pieces_os_main/quick_menu/linux_quick_menu.png" alt="" align="center" fullwidth="true" />

As a background resource task, there are currently fewer adjustable actions, but LTM Pieces Drive and Pieces Copilot can still be accessed and utilized within Pieces plugins and extensions on Linux.