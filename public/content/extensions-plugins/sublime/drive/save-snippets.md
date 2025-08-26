---
title: Saving
path: /extensions-plugins/sublime/drive/save-snippets
visibility: PUBLIC
status: PUBLISHED
description: The Pieces for Sublime Text Plugin lets users save code snippets directly from the editor, so that their snippets are securely stored and ready to be reused at a later date.
metaTitle: How to Save Code Snippets in Sublime with Pieces Drive
metaDescription: Save and organize important code snippets in Sublime Text using Pieces Drive for easy access.
---

## Saving Materials to Pieces Drive

There are two ways to save code with the Pieces for Sublime Text Plugin—through the right-click menu, or by saving with hotkeys.

You can use this feature to save all kinds of useful code materials, like:

* API endpoint definitions

* Utility functions or commonly used helper methods

* Code templates for starting new modules

* Reusable logic for error handling or authentication

## How to Save Materials

There is one way to save code within the Pieces for Sublime Text Plugin—through the right click menu.

### via Right-Click Menu

To capture useful code snippets, simply:

<Steps>
  <Step title="Select a Portion of Code">
    Highlight the code within your editor
  </Step>

  <Step title="Right Click">
    Right click the selection of code you chose
  </Step>

  <Step title="Select Save to Pieces">
    Hover on `Pieces` and then select `Save to Pieces`

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/using_snippets/using_snippets_PARENT_PAGE/saving_to_pieces.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

## What’s Stored When You Save a Snippet

When you save a snippet to your Pieces Cloud, it’s more than just the code that gets stored.

The Pieces Copilot captures:

* `Type`: Categorizes the snippet (e.g., API call, function, class) with it’s code language.

* `Associated Tags`: Keywords associated with the snippet for easier searching.

* `Custom Description`: Specifies precisely which *lines* (in numerical form) the snippet is from, as well as the file from which it originated—very useful for mind-mapping.

* `Smart Description`: AI-generated descriptions that summarize the snippet’s purpose and function.

* `Suggested Searches`: Related searches that help you discover similar snippets.

* `Related Links`: References to documentation, code repositories, or other relevant resources.

* `Related People`: Associated collaborators or contributors.

<Image src="https://cdn.hashnode.com/res/hashnode/image/upload/v1733969003991/b9f128cb-abed-4994-a43a-c6a2fdcde437.png" alt="" align="center" fullwidth="true" />

Additionally, the Pieces Copilot **scans saved snippets for sensitive information**, such as API keys, passwords, or authentication tokens, to ensure no confidential data is accidentally stored.

## Where Saved Snippets Live

Saved snippets are stored locally on your device, ensuring accessibility even when offline. This also means that any Pieces for Developers extension or plugin—or even the Pieces Desktop App—has constant, up-to-date access to your saved materials.

You can search your saved snippets with the `Pieces: Search` feature.

[Read more about how to find your saved snippets here.](/products/extensions-plugins/sublime/drive/search-reuse#finding-saved-snippets)