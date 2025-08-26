---
title: Generative AI Conversations
path: /extensions-plugins/sublime/copilot/chat
visibility: PUBLIC
status: PUBLISHED
description: The Pieces for Sublime Text Plugin provides versatile tools for leveraging generative AI to gain insights, debug, and optimize code seamlessly within your editor.
metaTitle: Chatting with AI in Sublime using Pieces Copilot | Pieces Docs
metaDescription: Interact with Pieces Copilot in Sublime Text for AI-driven coding insights and automated development assistance.
---

## Accessing Copilot Chats in Sublime Text

There are two primary ways to access Generative AI Conversations with the Pieces Copilot.

### via Right-Click Menu

<Steps>
  <Step title="Select Code and Right-Click in the Editor">
    Highlight any code segment and right-click to open the Tool Menu.
  </Step>

  <Step title="Select a Relevant Action">
    Choose `Start Conversation About The Current Selection` to open a new conversation.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/pieces_ai_copilot/chat/about_current_selection.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

### via Command Palette

Open the command palette with `⌘+shift+p` (macOS) or `ctrl+shift+p` (Windows/Linux), and enter commands such as:

* `Pieces: Copilot`: Opens a clean-slate chat with Pieces Copilot.

* `Pieces: Ask Copilot About Active File`: Provides insights for the current file open in your Sublime Text editor.

- `Pieces: Ask About The Current Project`: Offers context-aware assistance across your entire project.

<Image src="https://cdn.hashnode.com/res/hashnode/image/upload/v1733965846464/9d871fcd-c401-4235-bdb2-e971e0809335.png" alt="" align="center" fullwidth="true" />

Read more about [what commands are available in the Pieces for Sublime Text Plugin.](/products/extensions-plugins/sublime/commands)

## Contextualized Chats

There are 3 levels of contextual awareness you can use when starting a conversation or adding code to an existing Copilot Chat with the Pieces Copilot.

### Pieces: Start Conversation About The Current Selection

One of the easiest ways to ask the Pieces Copilot a question about a specific class, method, function, or script is to open the right-click menu, hover over the Ask Copilot section, and select the `About Current Selection` option.

To use this feature:

<Steps>
  <Step title="Open the Right Click Menu">
    Right click on a selected portion of code.
  </Step>

  <Step title="Locate Ask Copilot">
    Hover over the `Ask Copilot` section.
  </Step>

  <Step title="About the Current Selection">
    Select the `About Current Selection` option.
  </Step>

  <Step title="Enter Query">
    Once selected, you can enter your prompt in the text input field at the bottom of the Sublime Text's view and press enter.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/pieces_ai_copilot/chat/chatting_with_selection.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

This feature makes it incredibly convenient for users to get quick insights or answers to specific questions about their code.

### Pieces: Ask About The Current File

The `Pieces: Ask About The Current File` feature focuses on providing insights and assistance with the specific file you're working on.

To use this feature:

<Steps>
  <Step title="Open the Command Palette">
    Open up the command palette using `⌘+shift+p` (macOS) or `ctrl+shift+p` (Windows/Linux).
  </Step>

  <Step title="Execute Command and Enter Query">
    Enter `Pieces: Ask About The Current File`, then enter your question into the input field.

    <Image src="https://cdn.hashnode.com/res/hashnode/image/upload/v1733965582024/558aef1b-5c14-4613-a7b2-76686c5fa823.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

After running the initial command, you can then query the LLM, which will use the file as context to generate accurate and useful responses.

<Callout type="tip">
  This is ideal for developers who need a comprehensive understanding of a file, such as its dependencies, functions, and classes
</Callout>

### Pieces: Ask About The Current Project

Similar to the file-level command, the `Pieces: Ask About The Current Project` command lets developers understand every corner of an entire project.

To ask about the current project:

<Steps>
  <Step title="Open the Command Palette">
    Open the command palette with `⌘+shift+p` (macOS) or `ctrl+shift+p` (Windows/Linux).
  </Step>

  <Step title="Execute Command and Enter Query">
    Enter `Pieces: Ask About The Current Project`, then type in your question.

    <Image src="https://cdn.hashnode.com/res/hashnode/image/upload/v1733965827869/24c0facf-d574-4b57-99e6-c5a48f2eb8ab.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

This feature highlights errors and suggests improvements on a larger scale. Its main benefit is helping developers navigate their codebase by using the Pieces context-awareness engine to provide accurate information, even for specific prompts.

## Adding Context to Copilot Chats

There are a number of individual items you can add as context to a chat, namely **Files, Folders,** and **Snippets**.

This flexibility is useful when reference materials aren't directly accessible from Sublime Text or when you want to **compartmentalize context** by keeping files or folders from other projects separate from your active workflow.

To do this:

<Steps>
  <Step title="Select the Message Icon">
    You can select the **Message Icon** on the left side of any of your chats in the Copilot Chat window.
  </Step>

  <Step title="Select your Context Type">
    A new menu will appear. Choose the type of context you want to add, then select the item you wish to include in the Copilot chat.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/pieces_ai_copilot/chat/adding_context_to_copilot_chats.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

## Improving Code Consistency & Standardization

The Pieces Copilot helps improve code quality by identifying inconsistencies and providing actionable suggestions for standardization.

### Naming Inconsistencies

If functions across your workspace use inconsistent naming patterns (e.g., `authenticateUser` in `authHandler.go` vs. `retrieveUserProfile` in `userHandler.go`), Pieces Copilot can suggest adopting a standardized naming convention for better readability and maintainability, like this:

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