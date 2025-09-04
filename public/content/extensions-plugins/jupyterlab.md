---
title: JupyterLab Extension
path: /extensions-plugins/jupyterlab
visibility: PUBLIC
status: PUBLISHED
description: Learn more about the Pieces for JupyterLab Extension.
metaTitle: Using Pieces for JupyterLab Extension | Pieces Docs
metaDescription: Learn how to integrate and use Pieces for JupyterLab to save, manage, and enhance code snippets while leveraging AI-powered features.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/plugins_extensions/jupyterlabs.png"
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/plugins_extensions/jupyterlabs.png" alt="" align="center" fullwidth="true" />

***

<Callout type="alert">
  V2 Documentation for the Pieces JupyterLabs Extension is under construction.

  In the meantime, you can look at the V1 documentation for the Pieces for JupyterLab Extension below.
</Callout>

***

## Pieces for JupyterLab

Learn how to install the Pieces for JupyterLab Extension via the **PYPI Manager, Pip,** and **Conda**.

This extension is compatible with *JupyterLab 4.0.0* and higher, and is currently in **beta**.

<Callout type="tip">
  Pieces captures *no identifiable user data.* Our local-only architecture means your data never has to leave your device.
</Callout>

### Sign in Required

Pieces requires all users to sign in before using any plugins or extensions. You'll be prompted to authenticate if you haven't already. For help, see our [sign-in guide](/products/meet-pieces/sign-into-pieces).

### Installing PiecesOS

[PiecesOS](/products/core-dependencies/pieces-os) must be downloaded and installed separately from the JupyterLab Extension to work correctly.

<get-started-install />

## Installation Instructions

To install the Pieces for JupyterLab extension, run this `pip` command in your terminal:

```bash
pip install jupyter-pieces
```

Make sure extensions are enabled. If you don’t know how to do this, <a target="_blank" href="https://tljh.jupyter.org/en/latest/howto/admin/enable-extensions.html">click here for official Jupyter documentation</a> on how to do so.

<Callout type="alert">
  Be sure to accept the disclaimer before moving forward in this process.
</Callout>

## Features

Read some of the latest features you can find with in the Pieces for JupyterLab Extension below.

## Pieces Copilot

**Pieces Copilot** inside JupyterLab is your context-aware AI assistant, designed to help you work smarter with your notebooks.

Powered by qGPT and deeply integrated into the Pieces ecosystem, Copilot can answer questions specific to your code, suggest improvements, and provide real-time assistance—all based on the content of your notebook.

Whether you’re debugging, exploring new concepts, or documenting your workflow, Copilot helps you stay focused by delivering relevant insights without leaving your development environment.

Here’s how to use it:

<Steps>
  <Step title="Open PiecesOS">
    Ensure PiecesOS is open and up to date.
  </Step>

  <Step title="Open the View">
    Click the bot icon in the top slider of the JupyterLab Extension to open Pieces Copilot.
  </Step>

  <Step title="Start Prompting">
    Interact with the Pieces Copilot to get answers related to your notebook.
  </Step>

  <Step title="“Ask Copilot”">
    Highlight code, right-click, and select `Ask Copilot` for context-aware help based on your selected code.
  </Step>
</Steps>

### Enrich Selected Code

`Enrich Selected Code` allows you to instantly add helpful context to any piece of code within your Jupyter notebook.

Simply highlight a section of code, right-click, and choose the “Enrich with Description” option.

Pieces will generate a clear, concise explanation of what the code does—perfect for improving readability, onboarding collaborators, or creating better documentation. It’s a fast, easy way to make your notebooks more understandable and maintainable.

### Realtime Streaming

Changes in other Pieces tools (Desktop App, VS Code, etc.) reflect in JupyterLab *automatically*.

Any snippet you save, edit, or enrich in JupyterLab is instantly reflected in other Pieces integrations—like the Desktop App, VS Code, or JetBrains plugins—without any extra steps.

<Callout type="info">
  This seamless, bidirectional sync keeps your context up to date in real time, so you can move between environments without losing track of your work.
</Callout>

## Pieces Drive

**Pieces Drive** is a local, privacy-first storage system that powers the Pieces ecosystem.

It securely stores your code snippets, enrichments, and contextual data directly on your device—enabling lightning-fast access, offline functionality, and complete control over your development artifacts without relying on the cloud.

To save a snippet:

1. Highlight text, right-click, and choose “Save to Pieces.”

2. Use the Pieces button in a code block.

3. Use a dedicated keyboard shortcut.

<Image src="https://storage.googleapis.com/pieces_multimedia/PROMOTIONAL/PIECES_FOR_DEVELOPERS/JUPYTER/MACOS/RIGHT_CLICK_SAVE_SELECTION/16X9/PIECES_FOR_DEVELOPERS-JUPYTER-RIGHT_CLICK_SAVE_SELECTION-16X9-MACOS-6_22_2023.gif" alt="" align="center" fullwidth="true" />

### Find your Snippets

Quickly access all of your saved snippets by opening the Pieces View from the Ribbon Menu in JupyterLab.

You can sort snippets by **recency** or **language**, and use the search bar to instantly locate the code you need—no more digging through old files.

<Image src="https://storage.googleapis.com/pieces_multimedia/PROMOTIONAL/PIECES_FOR_DEVELOPERS/JUPYTER/MACOS/SEARCH_AND_INSERT/16X9/PIECES_FOR_DEVELOPERS-JUPYTER-SEARCH_AND_INSERT-16X9-MACOS-6_22_2023.gif" alt="" align="center" fullwidth="true" />

### Use your Snippets

Once you’ve saved a snippet, you can copy it directly from the Pieces View and paste it anywhere in your notebook.

You’ll also see rich metadata and syntax highlighting, making it easy to understand and reuse your code at a glance.

<Image src="https://storage.googleapis.com/pieces_multimedia/PROMOTIONAL/PIECES_FOR_DEVELOPERS/JUPYTER/MACOS/EXPANDED_VIEW/16X9/PIECES_FOR_DEVELOPERS-JUPYTER-EXPANDED_VIEW-16X9-MACOS-6_22_2023.gif" alt="" align="center" fullwidth="true" />

### Share your Snippets

Sharing is simple with Pieces. Right-click any snippet or use the dedicated share button to generate a secure, shareable link.

Whether you’re collaborating with teammates or showing off a solution, you can distribute your code in just a click.

To share:

1. Highlight code, right-click, and select “Share via Pieces Link.”

2. Click the Share button within a code block or the Pieces View.

3. Or use a keyboard shortcut.

<Image src="https://storage.googleapis.com/pieces_multimedia/PROMOTIONAL/PIECES_FOR_DEVELOPERS/JUPYTER/MACOS/SNIPPET_BUTTON_SHARE/16X9/PIECES_FOR_DEVELOPERS-JUPYTER-SNIPPET_BUTTON_SHARE-16X9-MACOS-6_22_2023.gif" alt="" align="center" fullwidth="true" />

<Callout type="tip">
  Pieces stores all your snippets for seamless sharing.
</Callout>

### Discover Snippets

The `Discover` tab in the Pieces View automatically surfaces snippets Pieces has found in your project.

It’s a great way to jumpstart your library of reusable code without manually saving each snippet.

<Image src="https://old.docs.pieces.app/assets/images/PIECES_FOR_DEVELOPERS-JUPYTER-MACOS-SNIPPET_DISCOVERY-jupyterlab-snippet-discovery-3b1f1151ae918dc902fd310335ebbc01.gif" alt="" align="center" fullwidth="true" />

### Embedded Button

The Pieces JupyterLab Extension adds an embedded `Save` button directly inside your code cells, making it effortless to capture key snippets as you work.

With one click, you can save the contents of a cell to Pieces without interrupting your flow—perfect for preserving important functions, code patterns, or in-progress ideas for later use.

<Image src="https://storage.googleapis.com/pieces_multimedia/PROMOTIONAL/PIECES_FOR_DEVELOPERS/JUPYTER/MACOS/EMBEDDED_BUTTON_SAVE_ACTIVE_CELL/16X9/PIECES_FOR_DEVELOPERS-JUPYTER-EMBEDDED_BUTTON_SAVE_ACTIVE_CELL-16X9-MACOS-6_22_2023.gif" alt="" align="center" fullwidth="true" />

## **Data Privacy, Security, and Offline-First Approach**

We prioritize your privacy and offline usability in the same spirit as JupyterLab.

* **Privacy and Security**—All data is stored locally, on your device.

* **On-Device ML**—80%+ of ML runs locally, reducing server exposure.

* **Offline-First**—Works fully offline, with strong functionality.

* **Opt-In Cloud**: Optional cloud features—<mark>your data, your control.</mark>

<Image src="https://old.docs.pieces.app/assets/images/finder_window_privacy-1b7ed7f34f7bd8480ed5cdab215c1e36.png" alt="" align="center" fullwidth="true" />

## Configuration

You can personalize your experience with the Pieces JupyterLab Extension through the **Pieces Settings** menu.

This allows you to tailor how Pieces behaves to best fit your workflow:

* **Auto-open Snippet List View**: Choose whether the Pieces View should automatically open when you save a new snippet—perfect for keeping your saved work front and center.

* **Cloud Capabilities**: Toggle opt-in cloud features on or off. By default, Pieces is local-only, but you can enable cloud sync or sharing on a per-resource basis when needed.

* **Pieces Server Port**: Manually configure the server port used by Pieces if you’re running a custom setup or need to resolve port conflicts.

* **Login/Logout of Pieces Cloud**: Seamlessly sign in or out of your Pieces Cloud account to access synced snippets across devices or keep everything stored locally, depending on your preference.

## Troubleshooting

If the Pieces JupyterLab Extension isn’t working as expected, first check that **Pieces OS** is running—you should see the Pieces logo in your toolbar (macOS) or taskbar (Windows).

Make sure you have the latest versions of both the **Pieces JupyterLab Extension** and **Pieces OS (v8.0.0 or higher)**, and that your **JupyterLab version is 4.0.0 or above**.

After updating, always restart JupyterLab to apply changes.

If problems persist, [submit this support form](https://getpieces.typeform.com/jupyterlab).

<on-device-storage />