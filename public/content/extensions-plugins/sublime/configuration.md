---
title: Configuration
path: /extensions-plugins/sublime/configuration
visibility: PUBLIC
status: PUBLISHED
description: Read the guide below to configure the Pieces for Sublime Text Plugin to work efficiently in your workflow and adapt to your preferences.
metaTitle: How to Configure the Pieces for Sublime Extension
metaDescription: Configure Pieces for Sublime Text to match your coding preferences and workflow requirements.
---

## Supported LLMs

We constantly update and configure our plugins and extensions, like the Pieces for Sublime Text Plugin, to [work with the latest LLMs.](/products/large-language-models)

## Opening Pieces Settings

To open Pieces settings inside of the Pieces for Sublime Text Plugin, you can use `⌘+shift+p` (macOS) or `ctrl+shift+p` (Windows/Linux) to open the command palette.

Then, enter `Pieces: Open Pieces Settings`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/sublime_text_plugin_assets/configuration/open_pieces_settings.gif" alt="" align="center" fullwidth="true" />

## Login / Logout

Use the `Pieces: Login` or `Pieces: Logout` command in your command palette to log in and out of your Pieces account.

<Image src="https://cdn.hashnode.com/res/hashnode/image/upload/v1733970751972/4255a16f-7b9e-44fb-b912-810fbfc80d51.png" alt="" align="center" fullwidth="true" />

***

## Configurable Settings

The Pieces for Sublime Text Plugin offers customizable settings to tailor your experience. These options let you configure the connection, language model, startup behavior, and code autocompletion. Here's an overview of the key settings:

***

| `host`                 | Specifies the address where the plugin should connect to a local service or server.                |
| ---------------------- | -------------------------------------------------------------------------------------------------- |
| `model`                | Determines which large language model to use for all Pieces Pilot functionality.                   |
| `syntax`               | Let’s you adjust your language extension.                                                          |
| `auto_start_pieces_os` | Lets you decide whether or not to open PiecesOS automatically on startup.                          |
| `Copilot`              | Allows you to choose whether to open the Copilot in the browser or IDE.                            |
| `auto_check_updates`   | Gives you the ability to enable or disable PiecesOS from auto updating.                            |
| `snippet.autocomplete` | Decide whether or not to enable auto-completion of code via suggest snippets from your repository. |

***

To change settings, you need to copy and paste the contents of the default settings file into the empty window on the right side, which you can find below:

```json
{
	"model":"gpt-4o", // Deprecated use "Pieces: Change LLM" instead
	"auto_start_pieces_os":true, // Open PiecesOS automatically on startup
	"snippet.autocomplete":false, // auto complete via Pieces saved snippets or not
	"syntax" : {}, // Langauge extension : syntax path
	"copilot" : "IDE", // IDE, BROWSER 
					  // Opens the copilot either in browser or in the sublime IDE it self
	"auto_check_updates": true  // Check if Pieces for Sublime plugin has an update on startup
								// Turn this off if Package Control is working fine
}
```

### Pieces Auto-Launch on Startup

You can choose whether or not PiecesOS starts immediately on the launch of the Sublime text editor by setting the parameters to `true` or `false.`

### Snippet Auto-Complete

Similarly, adjust the parameters to `true` or `false` to enable auto-completion of code via snippets to speed up your coding progress.

If you have Pieces snippets saved that are relevant to the code you're writing, you'll get automatic completion for that specific language.

### Reloading the Plugin

To reload the plugin, enter the command palette with `⌘+shift+p` (macOS) or `ctrl+shift+p` (Windows/Linux) and type `Pieces: Reload Plugin`.

For additional support resources, [check out our troubleshooting guide.](/products/extensions-plugins/sublime/troubleshooting)

## Saving Your Settings

Once you've copied the contents of the .JSON object and edited them to your preferences, simply save the file, reload the plugin, and restart Sublime for your changes to take effect.

<Callout type="info">
  You can save the .JSON file with `⌘+s` (macOS) or `ctrl+s` (Windows / Linux). You do not need to use **Save As,** as the file is already existing and this is simply updating the settings file, which comes with the Pieces for Sublime Text package.
</Callout>