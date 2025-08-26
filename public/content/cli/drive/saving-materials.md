---
title: Saving Materials
path: /cli/drive/saving-materials
visibility: PUBLIC
status: PUBLISHED
---

## Saving Code Snippets to Pieces Drive

Storing developer materials, such as snippets of boilerplate code, is an excellent way to build a helpful code collection in your Pieces Drive.

This helps you save time when writing generic code in various forms. The Pieces CLI offers a *create* feature designed to assist you with this.

You can use this feature to save all kinds of functional code materials, like:

* API endpoint definitions

* Utility functions or commonly used helper methods

* Code templates for starting new modules

* Reusable logic for error handling or authentication

## How to Save Materials

For Pieces CLI, you can save a snippet to your Pieces Drive with one command.

<Steps>
  <Step title="Open a Terminal">
    Opening a terminal on your device depends on your platform: Open your OS’ search bar and enter `terminal`(macOS/Linux) or `CMD`(Windows).
  </Step>

  <Step title="Find a Snippet">
    Select a section of code or text you want to save and copy it to your clipboard.

    The pieces will use what you have copied to the clipboard as the snippet.
  </Step>

  <Step title="Enter Pieces Create">
    In your terminal, you can now enter `pieces create`, which will automatically save your clipboard as a new snippet.

    If you’re within the Pieces CLI `pieces run` mode, you can enter `create`.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_drive/saving_snippet/pieces_create.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

## What’s Stored When You Save a Snippet

When you save a snippet to your Pieces Drive, more than just the code is stored.

The Pieces Copilot captures several different kinds of metadata:

* `Type`: Categorizes the snippet (e.g., API call, function, class) and its programming language.

* `Associated Tags`: Keywords linked to the snippet for easier searching.

* `Custom Description`: Specifies exactly which *lines* (by number) the snippet is from and the file it came from—handy for mind-mapping.

* `Smart Description`: AI-generated summaries that explain the snippet’s purpose and function.

* `Suggested Searches`: Related searches that help you find similar snippets.

* `Related Links`: References to documentation, code repositories, or other relevant resources.

* `Related People`: Associated collaborators or contributors.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_drive/saving_snippet/saved_snippet_displayed.png" alt="" align="center" fullwidth="true" />

Furthermore, the Pieces Copilot reviews stored snippets for sensitive data, including API keys, passwords, and authentication tokens, ensuring that **no confidential information** is unintentionally saved.

## Where Saved Snippets Live

Saved snippets are stored locally on your device, ensuring offline accessibility. This also means that any Pieces for Developers extension, plugin, or even the Pieces Desktop App, has constant, up-to-date access to your saved materials with Pieces Drive.

You can find your saved snippets via the `pieces list` command or the `pieces search` feature.

[Read more about how to find your saved snippets here.](/products/cli/drive/search-reuse#viewing-and-reusing-saved-snippets)
