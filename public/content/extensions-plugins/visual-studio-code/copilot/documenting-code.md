---
title: Documenting Code
path: /extensions-plugins/visual-studio-code/copilot/documenting-code
visibility: PUBLIC
status: PUBLISHED
description: With the Pieces Copilot inside the Pieces for VS Code Extension, you can quickly generate comments that capture the functionality and intent of your code—an often overlooked aspect of high-quality documentation.
metaTitle: Documenting Code Comments with Pieces Copilot in VS Code
metaDescription: With the Pieces Copilot inside the Pieces for VS Code Extension, you can quickly generate comments that capture the functionality and intent of your code.
---

## Adding Documentation with Pieces

Pieces Copilot can analyze and **comment on any selected portion of your code,** explaining its logic line by line to help ensure that it is not only readable but also easy to understand for others.

## How To Add Code Comments

There are two ways to add code comments to your selected

### via Right-Click Menu

To add comments to your code from the toolbar, select the desired lines, right-click, hover over `Pieces`, and choose `Comment Selection with Copilot`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/pieces_copilot/documenting_code/hover_over_comment.png" alt="" align="center" fullwidth="true" />

Pieces Copilot will generate clear, contextual comments for the selected code inside the chat window.

You can then click `Insert at Cursor` to insert the fix at the location of your cursor. You can also click `Accept Changes` to place the code comments directly between your lines of code at the precise location from which you selected the code.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/pieces_copilot/documenting_code/insert_at_cursor_code_comments.gif" alt="" align="center" fullwidth="true" />

### via Pieces: Comment

A quicker way of adding documentation to a function you may have previously overlooked is to click the `Pieces: Comment` tool, which appears above actionable tasks in your code that are visible on your screen.

This new [AI Quick Actions](/products/extensions-plugins/visual-studio-code#using-ai-quick-actions) feature—similar to CodeLens actions that sit above functions nearest your cursor—can generate quick, insertable comments to explain the purpose and logic of your code.

To get started, look for the **AI Quick Actions** buttons above individual functions in your code.

Once you’ve located the **AI Quick Actions**, left-click on `Pieces: Comment`, then click `Accept Changes` to insert the newly commented code in the original code’s location.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/pieces_copilot/documenting_code/add_comments_quick_action.gif" alt="" align="center" fullwidth="true" />

## Why Use Code Comments?

Code comments play a vital role in **maintaining a clean, well-documented codebase.**

They **provide context for reviewers** to focus on functionality and **make complex reasoning transparent,** ensuring easier code to follow and maintain.

Good documentation improves code readability and accelerates onboarding for people unfamiliar with the codebase. This is a twofold benefit—it supports **current and future development,** and creates a strong **foundation for upgrading and reiterating.**

Comments help you remember the purpose and function of the code, making it easier to revisit and understand after a long time away.

That’s why this specific feature is so powerful. Need a few hundred lines of code documented? No problem—just `Comment Selection with Copilot`.