---
title: Code Comments
path: /extensions-plugins/visual-studio/copilot/documenting-code
visibility: PUBLIC
status: PUBLISHED
description: With the Pieces Copilot in the Pieces for Visual Studio Extension, you can quickly generate comments that clearly capture your code's functionality and intent.
metaTitle: Documenting code with Pieces Copilot for Visual Studio
metaDescription: Automatically generate code comments inside Visual Studio with Pieces Copilot to improve documentation and readability.
---

## Commenting Code Selections with Pieces Copilot

Pieces Copilot **analyzes** and **comments on selected code**, generating precise, line-by-line explanations. This enhances readability and makes your code easier to understand.

### via Pieces > Comment

A quick way to add documentation to a function is by using the [AI Quick Actions](/products/extensions-plugins/visual-studio#using-ai-quick-actions) feature, visible above actionable tasks in your code. This feature allows you to generate comments to explain the logic and purpose of your functions directly within your editor.

To get started:

<Steps>
  <Step title="Locate the Pieces Quick Actions">
    Look for the `Pieces` button above individual functions in your code.
  </Step>

  <Step title="Open the Pieces Menu">
    Click the Pieces `Quick Action` button to open the available options.
  </Step>

  <Step title="Select the Comment Option">
    Choose `Comment` from the menu to let the Copilot generate meaningful documentation for the function.
  </Step>

  <Step title="Accept Changes">
    Review the generated comments and click `Accept Changes` to insert them into your code.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/documenting_code/adding_comments_quick_action.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

You can also right-click a selected portion of code, hover over `Pieces`, and choose `Comment Selection with Copilot`. Pieces Copilot will suggest changes that contain comments on new sections.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/documenting_code/hover_over_comment.png" alt="" align="center" fullwidth="true" />

## Why Use Code Comments?

Code comments are essential for maintaining a clean and well-documented codebase. They **provide context for reviewers**, allowing them to focus on functionality and **understand complex reasoning**, making the code easier to follow and maintain.

Good documentation improves code readability and accelerates onboarding for people unfamiliar with the codebase. This dual benefit supports **current and** **future development** by creating a strong **foundation for upgrades and iterations**.

Comments also serve as a memory aid, helping you remember the purpose and function of the code when revisiting it after a long time away.

That’s what makes the Pieces Copilot’s commenting feature so powerful. Whether you’re documenting a single function or hundreds of lines of code, simply highlight the desired code, click the `Pieces` CodeLens button, select **Comment**, and let Copilot take care of the rest.