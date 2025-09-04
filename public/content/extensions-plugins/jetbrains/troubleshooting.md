---
title: Troubleshooting
path: /extensions-plugins/jetbrains/troubleshooting
visibility: PUBLIC
status: PUBLISHED
description: Support resources, documentation, and our Discord channel for troubleshooting the Pieces for JetBrains Plugin, along with troubleshooting steps for JCEF-related issues.
metaTitle: Troubleshooting Pieces for JetBrains | Pieces Docs
metaDescription: Resolve common issues with the Pieces for JetBrains Plugin using our troubleshooting guide for smooth and uninterrupted development.
---

## Troubleshooting Pieces for JetBrains

Here are links to support resources, documentation, and our Discord channel for troubleshooting related to the <a target="_blank" href="https://plugins.jetbrains.com/plugin/17328-pieces">Pieces for JetBrains Plugin.</a>

You can also find some specific troubleshooting steps for JCEF-related issues below.

<on-device-storage />

[​](/extensions-plugins/jetbrains#troubleshooting)

## Pieces Copilot: Enabling JCEF Runtime and Downgrade[​](/extensions-plugins/jetbrains#pieces-copilot-enabling-jcef-runtime-and-downgrade)

The Pieces Copilot relies on the **JCEF (Java Chromium Embedded Framework)** runtime to function appropriately within JetBrains IDEs.

However, not all JetBrains IDEs, including specific versions of **Android Studio**, come pre-configured with a JCEF-compatible runtime, which can cause compatibility issues.

### Switching to a JCEF-Enabled Runtime

You must switch your Java runtime to a **JCEF-enabled runtime** inside your global IDE settings.

<Callout type="alert">
  This operation will require restarting your IDE, so make sure to save your work before doing so.
</Callout>

Follow these steps to switch your runtime:

<Steps>
  <Step title="Open Action Search">
    Open the Action Search Dialog using `⌘+shift+a` (macOS) or `ctrl+shift+a` (Windows/Linux).
  </Step>

  <Step title="Search for Boot Runtime">
    Search for `Choose Boot Java Runtime for the IDE`.
  </Step>

  <Step title="Choose the Latest JCEF Runtime">
    Select the **latest version** from the available JCEF-enabled runtimes.
  </Step>

  <Step title="Restart IDE" />
</Steps>

### Android Studio Hedgehog Compatibility Issues

If you’re using **Android Studio Hedgehog (2023.1.1)**, switching to a JCEF runtime may still result in GPU process errors, which can cause performance instability.

This is a <a target="_blank" href="https://github.com/gitbito/bitoai/issues/174">known issue with this release,</a> affecting Pieces Copilot and other plugins relying on JCEF (such as the <a target="_blank" href="https://github.com/flutter/flutter-intellij/issues/7119">Flutter inspector</a>).

### Recommended Workaround for Hedgehog Users

If you encounter GPU-related errors after switching to a JCEF runtime, consider **downgrading to Android Studio Giraffe (2022.3.1 Patch 4)**. This version offers better compatibility until a permanent fix is released for Hedgehog.

To downgrade Android Studio, follow these steps:

1. **Uninstall Hedgehog (2023.1.1)** from your device.

2. **Download Giraffe (2022.3.1 Patch 4)** from the Android Studio archives, which you can find here.

3. **Reinstall Android Studio** using the Giraffe version and switch the runtime to JCEF-enabled using the instructions above.

## Unable to Find the JetBrains Plugin in the JetBrains Marketplace[​](/extensions-plugins/jetbrains#i-cant-find-the-pieces-jetbrains-plugin-in-the-jetbrains-marketplace)

If you can't find the Pieces JetBrains Plugin in the JetBrains Marketplace, you can navigate directly to it using <a target="_blank" href="https://plugins.jetbrains.com/plugin/17328-pieces--save-search-share--reuse-code-snippets">this link</a>.

## Updating[​](/extensions-plugins/jetbrains#updating)

The Pieces for JetBrains Plugin will automatically update when a new version is available.

You can manually update the plugin by going to your Plugins window using `⌘+shift+x` (macOS) or `ctrl+shift+x` (Windows/Linux).

Next, locate the Pieces for JetBrains Plugin (titled ‘Pieces’) and click the **update button.**

### Check PiecesOS Status

Check to make sure PiecesOS is running. PiecesOS must be running for the Pieces for JetBrains Plugin to work.

### Restart JetBrains After Updates

If you’ve recently installed or updated PiecesOS or the Pieces for JetBrains Plugin, restart the IDE.

## Reloading the Pieces Copilot Chat Window

You may need to restart or refresh the Pieces Copilot chat, especially if you’re using a cloud LLM and disconnect from WiFi.

These scenarios can occasionally cause the LLM to ‘hang’—to appear as if generating a response but eventually timing out, entering an infinite response loop, or experiencing other issues.

To do so, click the small `Reload Copilot` symbol above the Pieces Copilot chat once it is open.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/troubleshooting/reload_copilot.png" alt="" align="center" fullwidth="true" />