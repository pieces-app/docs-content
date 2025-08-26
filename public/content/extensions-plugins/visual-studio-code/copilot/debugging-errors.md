---
title: Debugging Errors
path: /extensions-plugins/visual-studio-code/copilot/debugging-errors
visibility: PUBLIC
status: PUBLISHED
description: Intelligently debug tricky issues and correctly center that <div> with Pieces Copilot.
metaTitle: Debugging Code with AI in VS Code using Pieces Copilot
metaDescription: Use Pieces Copilot in VS Code for AI-driven debugging – quickly find, fix issues, and learn from intelligent AI-generated solutions.
---

## Fixing Bugs with Pieces Copilot

The Pieces Copilot in the <a target="_blank" href="https://marketplace.visualstudio.com/items?itemName=MeshIntelligentTechnologiesInc.pieces-vscode">Pieces for VS Code Extension</a> offers AI-driven debugging that **simplifies finding and fixing code issues in VS Code.** This feature not only speeds up troubleshooting but also provides an opportunity to learn from the fixes suggested by the AI.

## Using the Debugging Tool

To start debugging, locate your project's error or problematic code segment.

<Callout type="tip">
  Errors are usually indicated by **red underscoring** surrounding the error or problematic lines of code.
</Callout>

Then, right-click on the error, open the quick fix menu, and select `Pieces: Fix`. You will also see a **Yellow Lightbulb**. Clicking the **Yellow Lightbulb** will show `Pieces: Fix`, allowing you to debug the error on that line quickly.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/pieces_copilot/debugging_errors/pieces_fix_quick_action.gif" alt="" align="center" fullwidth="true" />

Pieces Copilot will utilize whichever LLM you have currently active and analyze the issue. Then, it will open a Copilot chat with suggestions, regenerate the code, and provide the option `Insert at Cursor` with fresh code comments.

You can then choose to `Accept` or `Insert at Cursor`. `Insert at Cursor` will place the fixed code at the pointer’s position. `Accept` will replace the broken code with the fixed version.

## Why Debug with Pieces Copilot?

Debugging with Pieces Copilot smoothens error resolution and provides AI-driven insights in an experience that doesn’t detract from your workflow in VS Code.

This saves time by reducing the need to search for solutions online or navigate extensive documentation, keeping your workflow efficient and reducing distractions.

Additionally, each suggested fix includes an explanation, helping you understand and improve your coding practices as you debug.

<Callout type="tip">
  The Pieces Copilot proactively identifies code issues—highlight your code, click the **Yellow Lightbulb,** and let it analyze the problem(s).
</Callout>