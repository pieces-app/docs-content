---
title: Configuration
path: /extensions-plugins/visual-studio-code/configuration
visibility: PUBLIC
status: PUBLISHED
description: Refer to the guide below to effectively configure the Pieces for VS Code Extension to align with your workflow and personal preferences.
metaTitle: How to Configure the Pieces for VS Code Extension
metaDescription: Configure the Pieces for VS Code Extension to match your workflow and preferences with this step-by-step setup guide.
---

## Settings, Models, and More

Learn how to configure the Pieces for VS Code Extension—from choosing your preferred LLM to customizing settings, shortcuts, and snippet behaviors.

### Supported LLMs

We constantly update and configure our plugins and extensions to work with the latest LLMs.

The Pieces for VS Code Extension [currently supports over 54 different LLMs.](/products/large-language-models)

[Read documentation on how to switch your Pieces Copilot Runtime (LLM)](/products/extensions-plugins/visual-studio-code/copilot/llm-settings#how-to-configure-your-llm-runtime) utilized by the Pieces for VS Code Extension within your IDE.

## Connecting to a Remote PiecesOS Instance

You can configure the Pieces VS Code Extension to connect to a remote machine running PiecesOS.

<Embed src="https://www.youtube.com/watch?v=sbgIaK9kpu4" />

### Prerequisites

* One machine running [Pieces OS](/installation-getting-started/what-am-i-installing)

* One machine running the [Pieces VS Code extension](/extensions-plugins/vscode)

Before you begin, note that this *only applies* if VS Code and PiecesOS are running on different machines.

<Callout type="tip">
  If Pieces OS is running on the same machine as VS Code, there should be no requirement to use this feature. Please verify these steps are required for your set up before following this guide.
</Callout>

Remember:

* Do not use your Pieces Cloud URL, as this feature requires a direct connection.

* The default port for remote connection is `39300`.

### LAN Setup

If both machines are on the same LAN:

1. Make sure your firewall allows traffic between them.

2. Find the LAN IP of the machine running Pieces OS.

3. In VS Code, go to `Settings → Workspace → Pieces: Custom URL` and enter:\
   `http://<LAN_IP>:39300`

4. Reload your VS Code window via `Command Palette → Developer: Reload Window`.

### Remote Access (Ngrok or Tailscale)

If machines are **not** on the same LAN:

1. Install <a target="_blank" href="https://ngrok.com/download">ngrok</a> or <a target="_blank" href="https://tailscale.com/">Tailscale</a> on the machine with Pieces OS.

2. Run: `ngrok http 39300`

3. Copy the public forwarding URL.

4. In VS Code, set it as the `Pieces: Custom URL` (see steps above).

5. Reload the VS Code window.

<Callout type="alert">
  Exposing Pieces OS publicly via *ngrok* should only be used as a last resort.
</Callout>

## Troubleshooting

Read below to find answers and fixes to some common issues experienced when setting up remote instances of PiecesOS.

### PiecesOS is Not Connecting

If PiecesOS is not connecting even though you’ve properly set up the remote connection, there are two potential causes (and two fixes) depending on the connection method.

### via WSL

If PiecesOS doesn’t connect automatically in WSL, try one of the following:

<Steps>
  <Step title="Enable Mirrored Networking (Recommended)">
    Requires WSL version 2.0.0 or higher and Windows 11.

    To do this, create or edit a `.wslconfig` file at `C:\Users\<your-username>\.wslconfig` then add the following code:

    ```plaintext
    [wsl2]
    networkingMode=mirrored
    ```

    Then, restart WSL by running:

    ```plaintext
    wsl --shutdown
    wsl
    ```
  </Step>

  <Step title="Add a Windows Firewall Rule">
    You can also try to add a firewall rule to bypass this issue.

    1. Press Win + R, type `firewall.cpl`, and hit `Enter`

    2. Go to *Advanced Settings → Inbound Rules → New Rule*

    3. Configure the rule:

       * **Rule Type:** Port

       * **Protocol**: TCP

       * **Port**: `39300`

       * **Action**: Allow the connection

       * **Profile**: Public, Private, Domain

       * **Name**: Allow PiecesOS on Port `39300`
  </Step>
</Steps>

### via Dev Containers

If experiencing connectivity issues with PiecesOS inside of development containers, try this:

1. Make sure Pieces OS is running *before* launching VS Code

2. Reload your VS Code window using Command Palette → Developer: Reload Window

If it's still not connecting, set a firewall rule:

* On Windows or macOS, allow traffic on port `39300`

* On Linux, allow traffic on port `5323`

## Opening Pieces Settings

To open the **Pieces Settings** in the Pieces for VS Code Extension, select the `Pieces Settings` icon within your sidebar. This will open the new Pieces Settings bar.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/configuration/new_opening_settings.gif" alt="" align="center" fullwidth="true" />

You can also access **Pieces Settings** in the bottom-left corner of the screen, where it says `Pieces Settings`.

## Overriding Commands in VS Code

If you’d like to adjust the keyboard shortcuts for Pieces functionality in VS Code, such as [saving a snippet](/products/extensions-plugins/visual-studio-code/drive/save-snippets) or [previewing markdown](/products/extensions-plugins/visual-studio-code/drive/search-reuse#viewing-and-reusing-saved-snippets), follow these steps:

<Steps>
  <Step title="Open Keyboard Shortcuts">
    Open the **Keyboard Shortcuts** editor by pressing `⌘+k+s` (macOS) or `ctrl+k+s` (Windows/Linux)
  </Step>

  <Step title="Locate the Pieces Command">
    Use the **search bar at the top of the editor** to locate the Pieces command you want to modify, such as `Save Current Selection`
  </Step>

  <Step title="Edit the Keybind">
    Click the **pencil icon** next to the command and select `Add Keybinding`
  </Step>

  <Step title="Enter Preferred Shortcut">
    **Enter your preferred shortcut**—be sure it doesn’t conflict with an existing VS Code command—i.e., `⌘+shift+'` (macOS) or `ctrl+shift+'` on (Windows/Linux)

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/configuration/new_settings_overview.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

## Settings Overview

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/configuration/new_settings_overview.png" alt="" align="center" fullwidth="true" />

### Account & Cloud Integrations

* **Account Name:** Displays your chosen display name in the extension.

* **Account Email:** Displays the email address associated with your account.

* **Early Access Program:** Indicates whether you are enrolled in the beta program.

### Personal Cloud

* **Status:** Shows whether your cloud is connected or disconnected and displays the last-updated timestamp.

* **Personal Domain:** Displays your custom subdomain (for example, `<your-domain>.`[`pieces.cloud`](http://pieces.cloud)).

* **Backup & Restore Data:** Provides a button to back up or restore all of your personal cloud data.

### Saved Material Auto-Enrichment

* **Auto-Generated Context:** A dropdown menu allows you to select how much context is auto-generated (None, Low, Medium, High).

### ML Processing

* **Processing Mode:** You can choose between Local, Cloud, or Blended resource usage.

* **Long-Term Memory Engine:** Toggles the long-term memory engine on or off and displays its current version.

* **Long-Term Memory Source Control:** Provides a link to manage which memory sources are used for long-term storage.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/configuration/ml_proceess_vscode.png" alt="" align="center" fullwidth="true" />

### Utilities

* **Clear Long-Term Memory Engine Data…:** Provides a button to purge persisted memory for a specified date range.

### Model Context Protocol (MCP)

* **Server URLs:** Provides a text field where you can list all of your MCP endpoint URLs.

* **View Documentation:** Links to the official MCP usage documentation for guidance.

### CodeLens

* **Enable Pieces Code-Lens:** Toggles the code-lens features on or off in the editor.

* **Use Same Conversation For Code-Lens:** Shares a single Copilot conversation across all code-lens actions.

### Saved Materials

* **Close Snippet Editor on Save:** Automatically closes the snippet editor when you save a snippet.

* **Enable Automatic Link Copy:** Automatically copies the snippet’s shareable link to your clipboard upon saving.

### PiecesOS Configs

* **Launch on Startup:** Automatically launches the PiecesOS background service when VS Code starts.

* **Auto Launch on Interaction:** Automatically starts PiecesOS the first time you interact with the extension.

### Autocomplete

* **Enable AutoComplete:** It suggests saved snippets are inline as you type code in the editor.

### Git Integration

* **Pieces › Save › Git: Related Links:** Attaches related commit links when saving a snippet.

* **Pieces › Save › Git: Related People:** Attaches the commit authors as metadata when saving a snippet.

* **Pieces › Save › Git: Description:** Uses commit messages as the default description for the saved snippet.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/vs_code_extension_assets/configuration/git_integration.png" alt="" align="center" fullwidth="true" />

### Notifications

* **Show Update Extension Notification:** Prompts you on startup if a new extension version is available.

### Onboarding

* **Launch Onboarding:** Reopens the onboarding tutorial to help you learn how to use the extension.

### Telemetry & Analytics

* **Telemetry & Diagnostics:** Shares anonymous usage and crash data to help improve the extension.

* **Share Error Analytics:** Shares detailed error analytics to help diagnose and fix bugs.

* **Share Usage Analytics:** Shares anonymized usage patterns to inform future feature development.

### Support

* **Documentation:** Provides a link to the online Pieces documentation.

* **Submit Feedback/Issues:** Provides a link to the GitHub issues page or support form for reporting bugs or requesting features.

### PiecesOS Information

* **PiecesOS Version:** Displays the current version number of the PiecesOS service.

* **Check for PiecesOS Updates:** Provides a button to check for and install PiecesOS updates manually.

* **PiecesOS Port:** Displays the network port on which PiecesOS is listening.

### Settings Applet

* **Version:** Displays the current version number of the Settings Applet.

***

For additional support resources, check out our [troubleshooting guide.](/products/extensions-plugins/visual-studio-code/troubleshooting)