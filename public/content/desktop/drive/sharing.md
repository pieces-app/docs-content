---
title: Sharing Saved Materials
path: /desktop/drive/sharing
visibility: PUBLIC
status: PUBLISHED
description: Share your saved materials through the cloud to developers & colleagues, even if they don't have a Pieces account.
metaTitle: Share saved code snippets in Pieces Drive | Pieces Docs
metaDescription: Easily generate and copy unique shareable links for your saved materials in Pieces Drive, enabling seamless collaboration and code sharing with your team.
---

## Collaborating with Saved Materials

You can generate and copy unique shareable links for saved materials in the Pieces Drive, letting you showcase your code and easily collaborate other developers on your team.

## Sharing

One of the most convenient ways to collaborate or showcase work is by sending a code snippet to your team, friends, or the broader developer community.

Pieces Drive makes this process dirt-simple using *shareable links*, which allow others to view your snippet and its related metadata in a consistent, Pieces-branded web interface—even if they don’t have Pieces installed. 

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/pieces_drive/sharing/shared_snippet_demo_1.png" alt="" align="center" fullwidth="true" />

These links preserve the snippet’s code, syntax highlighting, tags, annotations, and other contextual data—this way, recipients see not just lines of text, but the snippet’s *entire backstory and classification.*

## Generating Shareable Links

There are two ways to generate shareable links for saved materials in your Pieces Drive.

### via Quick Menu

Start by opening the material you want in the main *Detail View* of Pieces Drive.

Find and click the **three-dot Quick Menu** (usually in the top-right corner of the snippet's section).

Then, choose `Generate Shareable Link` or `Shareable Link`—if it's your first time creating a link for that snippet, Pieces will make a new unique URL.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Navigation/Snippet%20Discovery/sharing_a_snippet.gif" alt="" align="center" fullwidth="true" />

<Callout type="tip">
  If you’ve already generated a link for this material before, it exists in the cloud—so you can just copy the shareable link to your clipboard.
</Callout>

### via Keyboard Shortcut

You can toggle a different shareable link modal that provides you with the previously-generated link or generates a new one by using keyboard shortcuts—`cmd+L` (macOS) or `ctrl+L` (Windows/Linux).

If you want to see how the snippet appears, simply paste the link into a web browser.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/pieces_drive/sharing/material_in_browser_demo_2.png" alt="" align="center" fullwidth="true" />

You’ll find a code view, syntax highlighting, any relevant tags, annotations, and a snippet description—just like in Pieces Drive.

## Security & Sensitive Data

<mark>Pieces Drive takes security seriously.</mark>

When you begin generating a shareable link, Pieces is designed to initiate and allow specific behaviors pertaining to privacy and security:

* **Automatic Detection of Secrets**: If the code snippet contains credentials or tokens that Pieces recognizes (API keys, client secrets, etc.), you’ll *receive a warning* before proceeding.

* **Sensitive Info Management**: You can explicitly mark or unmark certain strings as sensitive within the material’s context panel.

* **User Confirmation**: Pieces prompts you to confirm that you’re okay sharing the snippet as-is or suggests that you *remove or redact sensitive* *portions* first.

### Best Practices

Pieces may not catch everything, so you should *always be careful* of what code materials you generate links for, and *with whom you share them.*

<Steps>
  <Step title="Review for Secrets">
    Even if Pieces doesn’t automatically flag something, it’s good practice to check for any private tokens, database credentials, or other sensitive data.
  </Step>

  <Step title="Create ‘Safe’ Versions">
    If you need to show code logic without actual credentials, consider duplicating your snippet, removing the secrets, and then sharing that sanitized version.
  </Step>

  <Step title="Boilerplate or Readability Transformation">
    If you just want to demonstrate a concept, consider using the [Transforming Code](/products/desktop/drive/transforming-code) features to create a boilerplate or more readable version for sharing.
  </Step>
</Steps>

## Managing Existing Links

Once a snippet has a shareable link, Pieces Drive helps you track and modify it.

Revisit the **Quick Menu** for the saved material, then look under the first section titled *Shareable Link* and click `Manage`.

This will give you access to the shareable link in an input field, the option to generate a GitHub Gist based on that code, and then 3 further options:

1. `Open in Browser`**:** Automatically opens the code snippet’s shareable link in your default browser.

2. `Refresh Link`**:** Refreshes the link if you’ve made changes to the saved material itself, so you can always share an up-to-date version.

3. `Revoke Link`**:** Similar to *deleting a material,* this button essentially ‘deletes’ the shared link, taking the saved material off of the cloud so that it cannot be accessed outside of your Pieces Drive.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Drive/Transforming%20%26%20Translating%20Code/screenshot_of_share_tab.png" alt="" align="center" fullwidth="true" />

## Use Cases & Workflows

Check out the workflow use cases below for ideas or inspiration on how to share code using the Pieces system.

***

<AccordionGroup>
  <Accordion title="Team Collaboration">
    Shareable links are excellent for quick internal reviews. Instead of copying raw code into a Slack channel, send a link so your teammates get the snippet’s annotations, tags, and formatting intact.
  </Accordion>

  <Accordion title="Open-Source Contributions">
    If you maintain an open-source library, shareable links can demonstrate bug fixes or new features without requiring others to install Pieces. They’ll see a snippet rendered in a neat web interface.
  </Accordion>

  <Accordion title="Code Reviews & Documentation">
    Use shareable links to document specific sections of a codebase. Project managers or QA engineers can open the link, comment on the snippet, and refer back to it without rummaging through version control logs.
  </Accordion>

  <Accordion title="Demo or Client Presentations">
    For freelancers or consultants, a shareable link offers a tidy way to showcase code examples to clients. They see professional formatting and can test the snippet themselves if they have access to a browser-based environment.
  </Accordion>
</AccordionGroup>