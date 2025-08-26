---
title: Generative AI Conversations
path: /extensions-plugins/jetbrains/copilot/chat
visibility: PUBLIC
status: PUBLISHED
description: Enhance your development workflow with Copilot Chats inside the Pieces for JetBrains Plugin—an interactive AI assistant integrated directly into your JetBrains IDE.
metaTitle: Chat with Pieces Copilot in JetBrains | Pieces Docs
metaDescription: Quickly search and reuse your saved code snippets in Pieces for JetBrains, ensuring seamless productivity without breaking your workflow.
---

## Accessing the Pieces Copilot Chat in JetBrains IDEs

There are several ways to open up the Pieces Copilot chat window in any JetBrains IDEs.

### via Right-Click Context Menu

<Steps>
  <Step title="Highlight Any Code Segment">
    Select some code in your active file
  </Step>

  <Step title="Select a Management Option">
    Select `Ask Copilot About Selection` or `Ask Copilot About File` from the tool menu to open a chat with the selected context.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/chat/ask_about_selection.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

### via the Sidebar

<Steps>
  <Step title="Select Copilot Tab in the Sidebar">
    Select the `Copilot Chat` tab within the JetBrains sidebar to open the chat interface.
  </Step>

  <Step title="Select the Starred Icon">
    Select the **Starred Icon** to add context to the Copilot chat

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/chat/add_context_and_ask.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

### via Keyboard Shortcuts

<Steps>
  <Step title="Open Search Everywhere">
    Press `ctrl+shift+a` (Windows/Linux) or `⌘+shift+a` (macOS) to open the `Search Everywhere` window
  </Step>

  <Step title="Query Pieces Copilot">
    Type **"Pieces Copilot"** and select it from the search results to open the chat

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/chat/searching_for_snippet.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

### via AI Quick Actions

Use the AI Quick Actions feature in the Pieces for JetBrains Plugin to quickly get an explanation for a confusing or forgotten function's logic.

Try using the `Pieces: Explain` tool above your code to start a conversation about a particular function.

This triggers the Copilot Chat window, which outputs an explanation and summary of the code function.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/chat/pieces_explain_quick_action.gif" alt="" align="center" fullwidth="true" />

In addition, there is also `Pieces: Comment`, which you can read more about <a target="_blank" href="/products/extensions-plugins/jetbrains/copilot/documenting-code#via-pieces-comment">here</a>.

## Contextualized Chats

You can utilize **2 different levels of contextual awareness** when initiating a Copilot chat (or adding code to an existing chat) with the Pieces Copilot.

### Ask Copilot About Selection

The `Ask Copilot About Selection` command lets you interact with Copilot regarding specific code snippets, functions, or classes.

To use this feature:

<Steps>
  <Step title="Choose a Portion of Code">
    Select a portion of code you want to ask about.
  </Step>

  <Step title="Open the Command Palette">
    Open the command palette with `⌘+shift+p` on macOS or `ctrl+shift+p` on Windows/Linux. Type and execute the `Ask Copilot About Selection` command.
  </Step>

  <Step title="Enter Your Prompt">
    Type your prompt in the text input field and press `return` (macOS) or `enter` (Windows/Linux).

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/chat/ask_about_selection_command_pallete.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

This approach is ideal for localized queries requiring **quick insights** or **guidance** **on specific code functionality**.

### Ask Copilot About Active File

The `Pieces Ask About Active File` feature focuses on the current file, offering tailored insights and assistance with debugging.

There are two ways to access this command:

1. Right-click inside your file and select `Ask Copilot about File`, then type your query into the dropdown text input field.

2. Open the command palette using `⌘+shift+p` (macOS) or `ctrl+shift+p` (Windows/Linux) and enter `Ask About File`.

Once you've entered your question, the Pieces Copilot will analyze the file's context to deliver precise responses.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/chat/ask_about_active_file.gif" alt="" align="center" fullwidth="true" />

This feature helps you understand file dependencies, methods, and structure. It also detects potential issues, suggests improvements, and more.

<Callout type="tip">
  The `Pieces: Ask About Active File` feature can also be applied during onboarding purposes to get helpful explanations for unfamiliar code.
</Callout>

## Adding Context to Copilot Chats

You can add context to a chat by adding `Files`**,** `Folders`**,** `Snippets`**,** `Websites`**,** and `Messages`**.**

This greatly boosts the number of generative AI responses you receive that will actually benefit you. It can provide **hyper-specific** responses because it’s contextually aware of your code.

To do this, select the **Starred Message Icon** in the bottom-left corner of your Copilot Chat window, which is openable from the JetBrains IDE sidebar.

Click the **Starred Message Icon,** then add whatever context items you need.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/chat/add_context_copilot.png" alt="" align="center" fullwidth="true" />

You can also right-click a file from your project or active file tree and add that file as context to the conversation.

This can be done without opening the Pieces Copilot window. Right-click on a file in your open project and select `Add to Copilot Chat Context`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/chat/add_to_copilot_context_file.png" alt="" align="center" fullwidth="true" />

### Adding Code Snippets

You can paste snippets of code as a code block inside of any Copilot Chat by clicking the `{ }` icon inside the chat window, then pasting in your code.

This is useful for bringing in code that isn’t present immediately in the active file as context, or for comparisons and suggestions.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/chat/adding_code_to_chat.png" alt="" align="center" fullwidth="true" />

### Extracting Code from Screenshots

You can also extract code from screenshots directly from the Copilot chat menu by selecting `Extract Code from Screenshot`, selecting the desired screenshot from your **Finder** (macOS) or **File Explorer** (Windows/Linux) menu, and confirming.

Pieces Copilot will then scan the screenshot and generate the code captured from the image into the chat. You can copy, insert it at your cursor, save it as a snippet, and more.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/chat/extract_from_screenshots.gif" alt="" align="center" fullwidth="true" />

## AI Quick Actions

Above the functions in your code, you can find the clickable `Pieces: Comment` and `Pieces: Explain` buttons.

Click `Pieces: Explain` to open up the Pieces Copilot in the side window. The Pieces Copilot will automatically explain the purpose and function of that code within the chat.

Similarly, you can click `Pieces: Comment` above a function to have your preferred LLM generate documentation for that piece of code—you can then insert that code directly at the cursor by clicking `Insert at Cursor` or save it as a snippet using the built-in `Save to Pieces` button.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/pieces_copilot/chat/pieces_explain_quick_action.gif" alt="" align="center" fullwidth="true" />

## Improving Code Consistency & Standardization

The Pieces Copilot Chat is designed to assist you with various coding tasks to boost productivity and enhance your workflow. This is done primarily by eliminating **context-switching** (needing to leave your IDE to access generative AI).

### Naming Inconsistencies

Suppose functions across your workspace use inconsistent naming patterns (e.g., `authenticateUser` in `authHandler.go` vs. `retrieveUserProfile` in `userHandler.go`). In that case, Pieces Copilot can suggest adopting a standardized naming convention for better readability and maintainability, like this:

```c
// authHandler.go
func authenticateUser(ctx context.Context, credentials Credentials) (User, error) {
    if credentials.Username == "" || credentials.Password == "" {
        return User{}, errors.New("missing credentials")
    }
}
```

### Inconsistent Error Handling

If error-handling strategies differ across files (e.g., structured errors in `authService.go` vs. inconsistent handling in `userService.go`), Pieces Copilot can help unify the approach:

```c
// authService.go
func LoginUser(credentials Credentials) (string, error) {
    token, err := authenticate(credentials)
    if err != nil {
        return "", fmt.Errorf("login failed: %w", err)
    }
    return token, nil
}
```