---
title: Sharing Snippets
path: /cli/drive/sharing
visibility: PUBLIC
status: PUBLISHED
---

## How to Share a Saved Snippet

Sharing a saved snippet is easy with the Pieces CLI. It enables you to collaborate with other developers, coworkers, and members even if they are outside of your organization or don’t have a Pieces account.

### via Command

Read below for detailed steps on using the `share` command within the Pieces CLI.

<Steps>
  <Step title="Open a Terminal">
    To access a terminal on your device, the method depends on your platform: use the search bar of your OS to type in `terminal` for macOS/Linux or `CMD` for Windows.
  </Step>

  <Step title="Enter Share Command">
    To share a snippet, enter the `pieces share` command.

    If you’re within the Pieces CLI run mode, you can enter `share`.
  </Step>

  <Step title="Select a Snippet">
    In the new view, use your arrow keys to navigate your saved snippets. When you’ve located the snippet you’d like to share, press `return` (macOS) or `enter` (Windows/Linux).

    This will begin the process of sharing the snippet using the Pieces CLI.
  </Step>

  <Step title="Open in Browser or Copy Link">
    After the snippet has been shared, its URL will appear within the terminal, and the CLI will prompt you to open the snippet in a browser.

    Open it in a browser with `y` or deny it with `n`. After entering your option, press `return` (macOS) or `enter` (Windows/Linux).

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_drive/sharing/sharing_snippet.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

## Enriched Sharing Experience

When you `share` a snippet, it’s not just the code that’s included. The snippet comes with additional metadata to provide context—<a target="_blank" href="/products/cli/drive/sharing#what-information-gets-shared">you can read more about that here.</a>

* `Snippet Type`: Identify the language or framework, such as Python or React.

* `Tags`: Useful keywords for quick categorization.

* `Description`: A summary of what the snippet does.

* `Related Links`: Helpful resources or documentation tied to the snippet.

* `Author Information`: A record of who created the snippet.

## What Information Gets Shared

When you save a snippet to the Pieces Cloud, the code is [enriched with valuable information](/products/cli/drive/save-snippets#what-happens-when-you-save-a-snippet), such as related people, links, annotations, tags, and an automatically generated description.

This information appears to the right of the code block when the shared snippet is open in your browser:

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair/CLI/cli_drive_sharing_1.png" alt="" align="center" fullwidth="true" />

### Sensitive Information Watchdog

The share command does more than enable you to share snippets with your entire team and other communities effectively.

You'll see a section titled **Sensitive Information:**

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair/CLI/cli_drive_sharing_2.png" alt="" align="center" fullwidth="true" />

Our in-house ML model scans snippets for potentially sensitive information, such as API keys or passwords, and alerts you so you can make an informed decision before sharing the snippet.
