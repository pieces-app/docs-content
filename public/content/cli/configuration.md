---
title: Configuration
path: /cli/configuration
visibility: PUBLIC
status: PUBLISHED
---

## Configuring the Pieces CLI

Pick which cloud model powers `ask`, set the editor that opens your config file, and manage your Pieces Cloud session. For the full command list, see the [commands reference](/products/cli/commands).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/configuration/available_models.png" alt="" align="center" fullwidth="true" />

> Switching between available models inside the Pieces CLI.

## Available Cloud Models

The Pieces CLI uses the same catalog of cloud LLMs as the rest of the Pieces Suite, with both *Free* and *Pro* tiers noted on each model.

<pieces-cloud-models />

For deeper guidance on picking the right model—and on configuring local LLMs—see [LLM Settings](/products/cli/copilot/llms-settings) and the full [Cloud Models](/products/large-language-models/cloud-models) reference.

## Switch the Active Model

Use `pieces list models` to view every model configured for the `ask` command. The active model is highlighted, and you can pick a new one interactively from the list.

```bash
pieces list models
```

The next `pieces ask "..."` you run will use the newly selected model.

## Set Your Code Editor

The CLI opens its config file in whichever editor you specify—`vim`, `code`, `nano`, or anything else on your `PATH`. Run `pieces config` to print the current configuration, or `pieces config --editor <editor>` to open the file for editing.

```bash
pieces config
pieces config --editor code
```

Edit values like `timeout: 10`, save the file, and changes take effect on your next CLI invocation.

## Account & Sync

`pieces login` signs you in to your Pieces Cloud account, enabling sync and access to private materials in your [Pieces Drive](/products/cli/drive). `pieces logout` clears your session—useful when switching accounts or working on a shared machine.

```bash
pieces login
pieces logout
```

***

## Next Steps

Hit a snag? Check the [troubleshooting guide](/products/cli/troubleshooting). For a complete reference of every CLI command and flag, see [Commands](/products/cli/commands).
