---
title: LTM-2.7 Engine
path: /core-dependencies/pieces-os/long-term-memory
visibility: PUBLIC
status: PUBLISHED
description: Enable, pause, and control the Long-Term Memory (LTM-2.7) Engine directly from PiecesOS—including Audio ingestion and per-app Access Control.
metaTitle: LTM-2.7 Engine | PiecesOS
metaDescription: Learn how to enable, pause, disable, and configure the Long-Term Memory (LTM-2.7) Engine from the PiecesOS Quick Menu, including Audio and Access Control.
---

## What is the LTM-2.7 Engine?

The **Long-Term Memory (LTM-2.7) Engine** is PiecesOS's core memory system. It runs entirely on your device and continuously captures workflow context—code you copy, screens you view, audio you hear—so Pieces can power [Timeline](/products/desktop/timeline), [Conversational Search](/products/desktop/conversational-search), and [MCP integrations](/products/mcp) with real context from your day.

All captured data is processed and stored **locally**. Nothing leaves your machine unless you explicitly choose to share it. See [Privacy & On-Device Storage](/products/core-dependencies/on-device-storage).

The primary control point for LTM is the **[PiecesOS Quick Menu](/products/core-dependencies/pieces-os/quick-menu)**—the Pieces icon in your menu bar (macOS, Linux) or system tray (Windows).

***

## Enabling, Pausing & Disabling LTM

### Enabling LTM

<Steps>
  <Step title="Open the Quick Menu">
    Click the `Pieces` icon in your taskbar (Windows) or menu bar (macOS, Linux).
  </Step>

  <Step title="Enable LTM">
    Click `Enable Long-Term Memory Engine`.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/core-dependencies/quick-menu_turn_off_ltm.png" alt="Toggling the LTM engine on or off in the PiecesOS Quick Menu" align="center" fullwidth="true" />

> LTM toggle in the PiecesOS Quick Menu

### Pausing or Disabling LTM

When LTM is active, the Quick Menu shows a green `On` button. Click it to open a dropdown with timed pause options or a full disable:

| Option | Effect |
| --- | --- |
| *Pause for 15 minutes* | Temporarily stops capture; resumes automatically |
| *Pause for 1 hour* | Temporarily stops capture; resumes automatically |
| *Pause for 6 hours* | Temporarily stops capture; resumes automatically |
| *Pause for 24 hours* | Temporarily stops capture; resumes automatically |
| *Turn Off* | Fully disables LTM until you re-enable it manually |

<Callout type="tip">
  Use timed pauses when you want a temporary break—for example, during a private call or a personal browsing session—without losing your LTM context history.
</Callout>

You can also toggle LTM from within the Pieces Desktop App:

<Steps>
  <Step title="Open your profile">
    Click your `User Profile` in the top left.
  </Step>

  <Step title="Navigate to LTM settings">
    Hover over `Settings` and select `Long-Term Memory`.
  </Step>
</Steps>

For a full breakdown of every toggle and option in that settings panel, see [LTM Settings](/products/desktop/configuration/long-term-memory).

***

## LTM Audio

**LTM Audio** extends capture to system audio and microphone input—meeting recordings, video calls, podcasts, or your own voice during a call.

<Steps>
  <Step title="Open the Quick Menu">
    Click the `Pieces` icon in your taskbar or menu bar.
  </Step>

  <Step title="Enable Audio capture">
    Scroll to *LTM Audio* and toggle it on.
  </Step>
</Steps>

<Callout type="info">
  On macOS, LTM Audio requires **System Audio Capture** and **Microphone Access** permissions before it can be enabled. First-time users may see a yellow warning indicator on their User Profile inside the Desktop App—click it to grant the required permissions. See [LTM Audio setup](/products/desktop/configuration/long-term-memory#ltm-audio) for full per-platform instructions.
</Callout>

***

## Long-Term Memory Access Control

Access Control lets you decide exactly which applications LTM captures data from.

<Steps>
  <Step title="Open the Quick Menu">
    Click the `Pieces` icon in your taskbar or menu bar.
  </Step>

  <Step title="Open Access Control">
    Navigate to *Long-Term Memory Access Control*.
  </Step>
</Steps>

You'll see two views:

### Enabled Sources

A live list of all apps currently feeding data into LTM (for example, Google Chrome, VS Code, Slack).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/new_pos_media/quick_menu_known_icons.png" alt="LTM enabled sources showing application icons in the PiecesOS Quick Menu" align="center" fullwidth="true" />

> Enabled sources view showing apps currently monitored by LTM

Click any listed source to open a window where you can **disable** it for that app individually. Disabled sources stop contributing new events to LTM but previously captured context is retained.

<Callout type="tip">
  Disable sources like password managers, banking apps, or private browser profiles to keep sensitive activity out of LTM entirely.
</Callout>

***

## Next Steps

<FancyCard title="LTM Settings (Desktop App)" href="/products/desktop/configuration/long-term-memory" colored={false}>
  Configure app access control, system permissions, LTM Audio, performance options, and clear stored data from the full settings panel.
</FancyCard>

<FancyCard title="Privacy & On-Device Storage" href="/products/core-dependencies/on-device-storage" colored={false}>
  Understand exactly what LTM stores on your device and how to manage or delete it.
</FancyCard>

<FancyCard title="PiecesOS Quick Menu" href="/products/core-dependencies/pieces-os/quick-menu" colored={false}>
  Everything else you can do from the Quick Menu—updates, MCP settings, ML processing, and more.
</FancyCard>
