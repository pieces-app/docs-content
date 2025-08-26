---
title: Generative AI Conversations
path: /extensions-plugins/visual-studio/copilot/chat
visibility: PUBLIC
status: PUBLISHED
description: The Pieces for Visual Studio Extension offers flexible options for using generative AI to gain insights, debug, and optimize your code within your editor.
metaTitle: Chat with Pieces Copilot for Visual Studio | Pieces Docs
metaDescription: Chat with Pieces Copilot inside Visual Studio for AI-driven code insights, debugging help, and automated coding assistance.
---

## Accessing Copilot Chat in Visual Studio

There are four primary ways to access generative AI conversations with the Pieces Copilot.

If the Pieces Copilot window isn't open, you can open it using the methods below, or by opening the command palette with `ctrl+shift+p`, searching for `Pieces Copilot`, and selecting it or pressing enter, or by using the keybind `alt+m,c`.

### via Right-Click Menu

<Steps>
  <Step title="Highlight Code and Right-Click">
    Highlight any code segment and right-click to open the tool menu.
  </Step>

  <Step title="Choose 'Ask Copilot'">

    Choose an option from the list that best fits your use case:

    * `Ask Copilot About Selection`

    * `Ask Copilot About Active File`

    * `Add Active File to Copilot Context`

    * `Explain Selection with Copilot`
  </Step>

  <Step title="Enter Question">
    A new menu will appear, prompting you to enter your question. Type your query and press `Enter`.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/chat/ask_about_file.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

### via Keyboard Shortcuts

You can also open up a dialogue with the Pieces Copilot chat—specifically the `Ask Copilot` option—by using the shortcut `alt+m` and then pressing `a`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/chat/asking_question_input_modal_for_asking_about_selection.png" alt="" align="center" fullwidth="true" />

### via Command Palette

Open the command palette with `ctrl+shift+p`, and enter commands, such as:

`Pieces > Ask Copilot about Selection`: Generates suggestions or improvements for the selected code snippet.

`Pieces > Ask Copilot About Active File`: Provides insights for the current file open in your Visual Studio editor.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/chat/command_pallette.png" alt="" align="center" fullwidth="true" />

Read more about [what commands are available in the Pieces for Visual Studio Extension](/products/extensions-plugins/visual-studio/commands).

### via AI Quick Actions

One quick way to get an explanation for a confusing or unclear function is by using the new [AI Quick Actions](/products/extensions-plugins/visual-studio#using-ai-quick-actions) feature in the Pieces for Visual Studio Extension.

Click the `Pieces` tool above a code function, then select `Explain`. This will start a conversation about the selected function.

You can also right-click a selected portion of code, hover over `Pieces`, and select `Explain Selection with Copilot`.

This action triggers the Copilot Chat window, which provides a detailed explanation and summary of the code's logic.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/chat/pieces_explain_quick_action.gif" alt="" align="center" fullwidth="true" />

There is also `Pieces > Comment`, which you can read more about [here](/products/extensions-plugins/visual-studio/copilot/documenting-code).

## Contextualized Chats

You can use two levels of contextual awareness in Visual Studio to start a conversation or add code to an existing Copilot Chat with the Pieces Copilot.

### Pieces > Ask Copilot About Selection

Use the `Pieces > Ask Copilot About Selection` button to interact with Copilot about specific code snippets, functions, or classes.

To use this feature:

<Steps>
  <Step title="Select a Portion/Piece of Code">
    Select a portion of code or select a class in the solution explorer.
  </Step>

  <Step title="Right-Click">
    Open the tool menu by right-clicking your selection.
  </Step>

  <Step title="Locate “Ask Copilot About Selection”">
    Locate the `Pieces` tool menu section, hover over it, and select `Ask Copilot About Selection`.
  </Step>

  <Step title="Ask your Question">
    Type your prompt in the text input field and press `enter`.
  </Step>
</Steps>

This approach is perfect for **quick insights** or **guidance** on specific code functionality.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/chat/asking_question_input_modal_for_asking_about_selection.png" alt="" align="center" fullwidth="true" />

### Pieces > Ask Copilot About Active File

The `Pieces > Ask About Active File` feature targets the current file, providing specific insights and help with debugging.

There are two ways to access this command:

1. Right-click inside your file, hover over `Pieces`, and select the `Ask Copilot about Active File`. Then enter your query into the drop-down text input field.

2. Open the command palette using `ctrl+shift+p` and enter `Pieces > Ask Copilot About Active File`. Then enter your query into the drop-down text input field.

<Callout type="tip">
  You can also use the default keybind to ask Pieces Copilot about the active file by pressing `alt+m,a`
</Callout>

After you enter your question, Pieces Copilot will analyze the file's context to provide precise responses that you can accept and insert at the cursor, directly placing them into your code environment.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/chat/ask_about_file.gif" alt="" align="center" fullwidth="true" />

This feature helps you understand file dependencies, methods, and structure. It also detects potential issues, suggests improvements, and more.

<Callout type="tip">
  The `Pieces > Ask About Active File` feature can also be applied during onboarding purposes to get helpful explanations for unfamiliar code.
</Callout>

## Adding Context to Copilot Chats

You can add context to a chat by adding `Files`**,** `Folders`**,** `Snippets`**,** `Websites`**,** and `Messages`**.**

This flexibility is especially useful when reference materials are not directly accessible from Visual Studio or when you want to compartmentalize context, minimizing overlap by keeping files or folders from other projects separate from your active workflow.

To do this, you can select the **Starred Message Icon** in the bottom-left corner of your Copilot Chat window, which you can open from the Visual Studio sidebar.\`

Click the **Starred Message Icon**, then add whatever context items you need.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/chat/adding_context.gif" alt="" align="center" fullwidth="true" />

### Adding Code Snippets

You can insert code snippets as a code block in any Copilot Chat by clicking the `{ }` icon in the chat window and pasting your code.

This feature is particularly helpful for referencing code that isn't in the active file, making comparisons, and receiving tailored suggestions.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/chat/snippet_in_chat.png" alt="" align="center" fullwidth="true" />

### Extracting Code from Screenshots

You can extract code directly from screenshots through the Copilot Chat menu. Select `Extract Code from Screenshot`, choose the desired screenshot from your File Explorer, and confirm.

Pieces Copilot will scan the screenshot, generate the code from the image, and display it in the chat. You can copy the code, insert it at your cursor, save it as a snippet, and more.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/chat/extracting_code.gif" alt="" align="center" fullwidth="true" />

### Adding Folders from File Explorer

To add folders to your Copilot Chat context, click the **Starred Message Icon** in the bottom-left corner of the Copilot Chat window, accessible from the Visual Studio sidebar.

You can then choose which type of context you’d like to add, but in our case, we’ll choose a `folder`.

This will open a new prompt to guide you through adding folders to the context.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/pieces_copilot/chat/add_folder_to_context.png" alt="" align="center" fullwidth="true" />

## Improving Code Consistency & Standardization

The Pieces Copilot helps improve code quality by identifying inconsistencies and providing actionable suggestions for standardization.

### Naming Inconsistencies

Suppose functions across your workspace use inconsistent naming patterns (e.g., `authenticateUser` in `authHandler.go` vs. `retrieveUserProfile` in `userHandler.go`). In that case, can suggest adopting a standardized naming convention for better readability and maintainability, like this:

```go
// authHandler.go
func authenticateUser(ctx context.Context, credentials Credentials) (User, error) {
    if credentials.Username == "" || credentials.Password == "" {
        return User{}, errors.New("missing credentials")
    }
}
```

### Inconsistent Error Handling

If error-handling strategies vary across files (e.g., structured errors in `authService.go` vs. inconsistent handling in `userService.go`), Pieces Copilot can standardize the approach. For example:

```go
// authService.go
func LoginUser(credentials Credentials) (string, error) {
    token, err := authenticate(credentials)
    if err != nil {
        return "", fmt.Errorf("login failed: %w", err)
    }
    return token, nil
}
```