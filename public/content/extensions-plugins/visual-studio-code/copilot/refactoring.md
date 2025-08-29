---
title: Refactoring
path: /extensions-plugins/visual-studio-code/copilot/refactoring
visibility: PUBLIC
status: PUBLISHED
description: Modify your code to add error handling, remove outdated documentation, and much more with Pieces Copilot.
metaTitle: Refactoring Code with AI in VS Code using Pieces Copilot
metaDescription: Switch between LLMs in the Pieces for VS Code Extension, including cloud-based and local models, for flexible AI-powered coding.
---

## Refactoring Code

Refactoring is vital for improving your code's structure and maintainability without changing its behavior. The <a target="_blank" href="https://marketplace.visualstudio.com/items?itemName=MeshIntelligentTechnologiesInc.pieces-vscode">Pieces for VS Code Extension</a> simplifies this process with its `Modify Selection with Copilot` feature.

## Modifying your Code with Pieces Copilot

You can modify your code to include changes to error handling, changing function names, and adding functionality in two different ways.

### via Right-Click Menu

Right-click a highlighted piece of code you’d like to modify, then hover over `Pieces` and click on `Modify Selection with Copilot`.

Once you click `Modify Selection with Copilot`, Pieces Copilot will open the Copilot chat window in the VS Code sidebar, generating and showcasing the proposed changes.

You can review the modifications and decide whether to accept them, automatically integrating the updates into your codebase from the point the code was selected—i.e, at your cursor.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/pieces_copilot/refactoring/modify_selection.gif" alt="" align="center" fullwidth="true" />

### via Command Palette

You can also access the `Modify Selection with Copilot` feature quickly using shortcut commands in VS Code.

Press `⌘+shift+p` (macOS) or `ctrl+shift+p` (Windows/Linux) to open the command palette, then type `Pieces: Modify Selection with Copilot`.

Once the input modal is visible at the top of your IDE, enter in your prompt—i.e, whatever changes you’d like made to the code—then press `return` (macOS) or `enter` (Windows/Linux).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair_2/visual_studio_code/refactoring.gif" alt="" align="center" fullwidth="true" />

This method offers a fast, efficient way to refactor and improve your code without interrupting your workflow.

<Callout type="tip">
  You can use `Modify Selection with Copilot` to add detailed logging to critical functions for improved debugging and restructure long methods into smaller, more modular functions.
</Callout>