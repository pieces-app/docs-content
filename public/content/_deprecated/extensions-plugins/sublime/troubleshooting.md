---
title: Troubleshooting
path: /extensions-plugins/sublime/troubleshooting
visibility: PUBLIC
status: PUBLISHED
description: Find links to support resources, documentation and our Discord channel for any troubleshooting related to the Pieces for Sublime Text Plugin.
metaTitle: Troubleshooting Common Issues with the Pieces for Sublime Text Plugin
metaDescription: Resolve common issues with the Pieces for Sublime Text using our troubleshooting guide.
---

## Having Trouble with Pieces for Sublime Text?

If the Pieces for Sublime Text Plugin isn’t working as expected, try the following troubleshooting steps.

<on-device-storage />

### Ensure You Have the Latest Version(s)

First, confirm you’re using the latest version of the <a target="_blank" href="https://packagecontrol.io/packages/Pieces">Pieces for Sublime Text Plugin</a> from Package Control and the latest version of [PiecesOS](/products/core-dependencies/pieces-os).

The minimum functioning version permitted is currently **1.4.3.**

### Check PiecesOS Status

Check to make sure PiecesOS is running. PiecesOS must be running for the Pieces for Sublime Text Plugin to work.

### Restart Sublime Text After Updates

If you’ve recently installed or updated PiecesOS or the Pieces for Sublime Text Plugin, restart the IDE.

Contact the <a target="_blank" href="https://getpieces.typeform.com/to/mCjBSIjF#docs-sublime">Pieces support team</a> if the issue still persists.

### macOS-Specific Configuration

Make sure that the `host` object inside the Pieces Settings file is **empty,** not set to `localhost:1000` as this creates issues with Package Control trying to load the Pieces Package, and can disable the plugin.

### Reload the Plugin<a target="_blank" href="/extensions-plugins/sublime#reload-the-plugin">​</a>

If you're experiencing an issue or something isn't working properly, try reloading the plugin.

To do so, open the command palette using `⌘+shift+p` (macOS) or `ctrl+shift+p` (Windows / Linux) and typing `Pieces: Reload Plugin`, then press Enter.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/troubleshooting/reload_plugin_sublime.gif" alt="" align="center" fullwidth="true" />