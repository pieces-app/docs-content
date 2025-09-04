---
title: LLM Settings
path: /cli/copilot/llms-settings
visibility: PUBLIC
status: PUBLISHED
---

## Switching LLMs

The Pieces CLI currently supports 19 different cloud-hosted LLM models.

## How To Configure Your LLM Runtime

Switching your LLM model in the Pieces CLI is easy. You can select the model that best fits your needs.

Follow the steps below to change the cloud LLM utilized by the Pieces MCP:

<Steps>
  <Step title="Open a Terminal">
    Opening a terminal on your device depends on your platform: Open your OS’ search bar and enter `terminal`(macOS/Linux) or `CMD`(Windows).
  </Step>

  <Step title="Start Pieces CLI">
    In your terminal, enter `pieces run` to launch into Pieces.
  </Step>

  <Step title="Open Models and Change">
    While in the Pieces CLI, type `list models`. This will display a list of available models within the Pieces CLI.

    Use your `scroll wheel` or `arrow keys` to navigate to your desired LLM and press `return` (macOS) or `enter` (Windows/Linux) to set the LLM runtime.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/pieces_copilot/llms_settings/available_models.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

Once you’ve chosen a new model, the switch is instant. You can continue your work seamlessly with the selected model's capabilities—*no need to restart or refresh anything.*

### Available LLMs

Pieces CLI supports 26 cloud-hosted LLM models, allowing you to choose from a variety of options to meet your needs.

| Supported LLMs                | Supported LLMs   |
| ----------------------------- | ---------------- |
| Gemini-2.7 Flash Preview      | GPT-4o Mini      |
| o4 Mini                       | Gemini-1.5 Pro   |
| o3                            | Gemini-1.5 Flash |
| GPT-4.1                       | GPT-4o           |
| Gemini-2.0 Flash Lite         | Claude 3 Haiku   |
| Gemini-2.7 Pro Experimental   | Claude 3 Sonnet  |
| Gemini-2.7 Pro Preview        | Claude 3 Opus    |
| Claude 3.7 Sonnet             | GPT-4 Turbo      |
| o3 Mini                       | (Gemini)         |
| o1                            | GPT-3.5-turbo    |
| Gemini-2.0 Flash Experimental | GPT-4            |
| Claude 3.5 Sonnet             | Codey (PaLM2)    |
| Claude 3.5 Haiku              | (PaLM2)          |
