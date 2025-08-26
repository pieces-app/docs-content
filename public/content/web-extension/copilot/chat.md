---
title: Generative AI Conversations
path: /web-extension/copilot/chat
visibility: PUBLIC
status: PUBLISHED
description: Enhance your development workflow with Copilot Chats in the Pieces Web Extension—an interactive AI assistant directly in your favorite browser.
metaTitle: Accessing Pieces Copilot Chat in Web Extension
metaDescription: Learn how to open the Pieces Copilot chat via right‑click menus, AI quick actions, or the sidebar, and add files, code snippets, or screenshots for context‑aware assistance.
---

## Accessing the Pieces Copilot Chat in the Web Extension

There are several ways to open up the Pieces Copilot chat window in your browser.

### via Right-Click Context Menu

The primary method of accessing Pieces Copilot, Pieces Drive, and other views is from the right-click menu.

<Steps>
  <Step title="Highlight Any Section of Text">
    When you find a code snippet or an important text block, highlight it.
  </Step>

  <Step title="Right-Click and Select Option">
    Right-click on your selection, hover over `Pieces For Developers`, and select `Ask Copilot About…`

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/web_extension/pieces_copilot/chat/ask_pieces_right_click.gif" alt="" align="center" fullwidth="true" />

    This initiates a Pieces Copilot chat using the active code snippet as pre-loaded context for the conversation.
  </Step>
</Steps>

### via AI Quick Actions

Under any code block, Pieces adds AI Quick Actions that let you quickly open the Copilot Chat window with the context of the code block.

Clicking the `Ask Copilot` Quick Action will start a Copilot Chat with the code within the code snippet as context.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/web_extension/pieces_copilot/chat/ask_copilot_QA.gif" alt="" align="center" fullwidth="true" />

### via the Sidebar

You can open up the dedicated Pieces Copilot view to locate previous chats or start new ones without context right from the sidebar.

<Steps>
  <Step title="Open the Pieces Web Extension">
    Select the `Pieces` icon in the extensions within your browser.
  </Step>

  <Step title="Switch to Pieces Copilot">
    If it's not enabled by default, click the dropdown in the top left and choose Pieces Copilot to access the Copilot Chats.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/web_extension/pieces_copilot/chat/hovering_pieces_copilot.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

## Starting Copilot Chats with Context

You can add context to a chat by adding `Files`**,** `Folders`**,** `Snippets`**,** `Websites`**,** and `Messages`**.**

This greatly boosts the number of generative AI responses you receive that will actually benefit you. It can provide *hyper-specific* responses because it’s contextually aware of your workspace.

To do this, you can select the `Circled Plus` Icon in the bottom-left corner of your Copilot Chat window, which is openable from the extensions section of your browser.

Click the `Circled Plus` icon**,** then add whatever context items you need.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/web_extension/pieces_copilot/chat/add_context_clicked.png" alt="" align="center" fullwidth="true" />

### Adding Code Snippets

You can paste code snippets as a code block in any Copilot Chat by clicking the `{ }` icon in the add context window and then pasting your code.

This helps add code that isn't currently in the active file as context, or for making comparisons and suggestions.

You can also locate a code snippet, i.e., on StackOverflow, and select the `Ask Copilot` that appears below it.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/web_extension/pieces_copilot/chat/add_context_snippet.png" alt="" align="center" fullwidth="true" />

### Extracting Code from Screenshots

You can extract code from screenshots directly in the Copilot chat menu by selecting `Extract Code from Screenshot`.

Choose the screenshot from your **Finder** (macOS) or **File Explorer** (Windows/Linux) menu, and confirm your selection.

Pieces Copilot will scan the screenshot and generate the code from the image into the chat. You can then copy it, save it as a snippet, and more.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/web_extension/pieces_copilot/chat/extract_code_screenshot.gif" alt="" align="center" fullwidth="true" />

## AI Quick Actions

Below code blocks on websites, you can find a clickable `Ask Copilot` option that will allow you to ask Pieces Copilot directly about the code.

Clicking `Ask Copilot` will open the Pieces Copilot sidebar. The code will be explained within that chat, along with its purpose and function.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/web_extension/pieces_copilot/chat/ask_copilot_QA.gif" alt="" align="center" fullwidth="true" />

## Improving Code Consistency & Standardization

The Pieces Copilot Chat helps you with coding and learning tasks to increase productivity and improve your workflow.

It achieves this by removing the need for **context-switching** (leaving your window to use generative AI).

### Naming Inconsistencies

Suppose functions across your workspace use inconsistent naming patterns (e.g., `authenticateUser` in `authHandler.go` vs. `retrieveUserProfile` in `userHandler.go`).

In that case, it is helpful to adopt a standardized naming convention for better readability and maintainability. You can find suggestions for such conventions in snippets available on the web, like this:

```c
// authHandler.go
func authenticateUser(ctx context.Context, credentials Credentials) (User, error) {
    if credentials.Username == "" || credentials.Password == "" {
        return User{}, errors.New("missing credentials")
    }
}
```

### Inconsistent Error Handling

If error-handling strategies differ across web sources (e.g., structured errors in `authService.go` vs. inconsistent handling in `userService.go`), Pieces Copilot can help unify the approach:

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