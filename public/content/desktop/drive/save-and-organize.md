---
title: Saving & Organizing Materials
path: /desktop/drive/save-and-organize
visibility: PUBLIC
status: PUBLISHED
description: Learn about bringing new code snippets into Pieces Drive, keeping them tidy, and maintaining context and clarity as your library expands.
metaTitle: Save & organize code snippets with Pieces Drive | Pieces Docs
metaDescription: Learn how to save, organize, and manage code snippets in Pieces Drive while maintaining context and clarity as your library grows.
---

## Overview

Saving materials—code snippets, text notes, or entire files—is the foundation of Pieces Drive.

Once saved, these materials are automatically enriched with valuable metadata such as tags, annotations, and suggested links, helping you find and reuse them easily.

## Saved Materials List

All of your saved materials are listed on the left-hand side of the view.

From this list, you can scroll down to see previous saved materials, or click the `Clock` icon to sort them in a few different ways:

* `Recent`**:** Sorts the list of materials by which were most recently used.

* `Suggested`**:** Presents saved materials that are likely to benefit your current workflow, eg., if you’ve been working on API calls in Python, you may see API boilerplate code snippets.

* `Alphabetical`**:** Sorts the list by *titles* in alphabetically-descending order.

* `Language`**:** Groups saved materials by language—Python, JavaScript, Kotlin, etc.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Interacting/sort_filters_drive.png" alt="" align="center" fullwidth="true" />

### Adding New Materials

The primary way to add materials to Pieces Drive is through the `Add Materials` button, located in the bottom-left corner of the Pieces Drive view.

Clicking it opens a modal that presents several distinct options for different workflows and preferences.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Drive/Transforming%20%26%20Translating%20Code/add_code_snippet.png" alt="" align="center" fullwidth="true" />

### Paste Code from Clipboard

Paste code from your clipboard to save as a new material.

<Steps>
  <Step title="Purpose">
    Quickly add snippets you’ve copied from somewhere else—an IDE, a website, or a note.
  </Step>

  <Step title="How It Works">
    Select `Paste Code from Clipboard`, then paste or drag and drop your code snippet into the provided text field. Pieces will instantly parse it and create a new snippet in your drive.
  </Step>
</Steps>

### Use a Plugin

Find materials in your Pieces Drive that you saved in other Pieces-enabled plugins and extensions.

<Steps>
  <Step title="Purpose">
    Seamlessly save snippets to Pieces Drive from within your favorite IDE or browser.
  </Step>

  <Step title="How It Works">
    Install a Pieces extension or plugin (e.g., for Visual Studio Code, JetBrains IDEs, Chrome, etc.).

    Whenever you highlight code and choose “Save to Pieces” (or similar), it syncs directly to your Pieces Drive.

    Then, the snippet appears in your Saved Materials List with an auto-generated title and immediate enrichment.
  </Step>
</Steps>

### Snippet Discovery

Scan local code repositories for useful snippets that are relevant to your workflow.

<Steps>
  <Step title="Purpose">
    Automate finding reusable code within a local folder or repository.
  </Step>

  <Step title="How It Works">
    Select **Snippet Discovery** in the modal, then choose a folder or repository on your device.

    Pieces scans these files for frequently repeated code patterns (snippets).

    You can decide which discovered snippets to add to Pieces Drive.
  </Step>
</Steps>

### Import GitHub Gists

Import GitHub Gists as individual saved materials in your Pieces Drive.

<Steps>
  <Step title="Purpose">
    Bring your Gists (public or private) into one centralized repository.
  </Step>

  <Step title="How It Works">
    Log in with your GitHub account if prompted. Select `Import GitHub Gists` and pick the Gist(s) you want to import.

    Each file in the selected Gist becomes a separate snippet in Pieces Drive.
  </Step>
</Steps>

### Create from Scratch

Create new saved materials from scratch.

<Steps>
  <Step title="Purpose">
    Quickly craft a new snippet or note that doesn’t yet exist anywhere else.
  </Step>

  <Step title="How It Works">
    Click `Create from Scratch`.

    Then, type or paste the content you’d like to save—this can be code or plain text.

    You can assign an initial title or let Pieces generate one automatically.
  </Step>
</Steps>

### Duplicate Current Material

Make a duplicate copy of a material to fork, revise, or modify.

<Steps>
  <Step title="Purpose">
    Make an immediate copy of the snippet you have open, often used for branching or revisions.
  </Step>

  <Step title="How It Works">
    Choose **Duplicate Current Material** in the modal.

    Decide whether you want an exact copy, or a transformed version (e.g., more readable, more performant, different language, or boilerplate template).

    The new snippet appears alongside the old one, preserving all context.
  </Step>
</Steps>

### Describe a Snippet to Generate

Use generative AI to generate new saved materials based on your exact requirements.

<Steps>
  <Step title="Purpose">
    Use natural language to generate brand-new code.
  </Step>

  <Step title="How It Works">
    Click `Describe a Snippet to Generate`.

    Type a short or detailed description, e.g., “A basic Node.js HTTP server with URL parsing.”

    Pieces produces the snippet automatically, complete with immediate enrichment and classification.
  </Step>
</Steps>

### Add Files

Import files from your device to use as a base for snippet discovery, or as context for future workflows.

<Steps>
  <Step title="Purpose">
    Import entire local files into Pieces Drive for safekeeping and snippet discovery.
  </Step>

  <Step title="How It Works:">
    Select `Add Files`.

    Browse and pick one or multiple files.

    Pieces scans their content, creating separate snippets if it detects multiple distinct code sections—or it may create a single snippet if the file is smaller.
  </Step>
</Steps>

## Best Practices & Tips

Find some additional information and quick tips for saving and organizing materials in the Pieces Drive below.

<AccordionGroup>
  <Accordion title="Name Snippets Wisely">
    While Pieces auto-generates titles, consider adding your own if you frequently revisit a snippet.
  </Accordion>

  <Accordion title="Use Tags for Faster Search">
    The more tags you add, the easier it becomes to filter your library when you’re deep into a project.
  </Accordion>

  <Accordion title="Annotate for Clarity">
    If you’re sharing your workspace with other developers, annotations can be invaluable for explaining snippet usage or constraints.
  </Accordion>

  <Accordion title="Enable Snippet Discovery (Early)">
    If you have large repositories, run Snippet Discovery to populate your drive with frequently used code.
  </Accordion>

  <Accordion title="Leverage Plugins">
    Don’t forget that saving snippets from an IDE plugin is often the fastest way to build up your Pieces Drive library without leaving your coding environment.
  </Accordion>
</AccordionGroup>