---
title: Models
path: /desktop/configuration/models
visibility: PUBLIC
status: PUBLISHED
description: Manage AI models and model preferences.
metaTitle: Models Settings in Pieces Desktop
metaDescription: Manage AI models, configure processing modes, set up local model runtime, and enable or disable specific models.
---

## Models Settings

Manage AI models and model preferences. Configure processing modes, set up local model runtime with Ollama, and control which AI models are available for use in Pieces.

To access Models settings, click your `User Profile` in the top left, then hover over `Settings` and select `Models`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/configuration/models/models_settings_overview.png" alt="" align="center" fullwidth="true" />

> Models settings showing Model Capabilities, Local Model Runtime, and Model Management sections

## Model Capabilities

Configure how Pieces processes your materials using machine learning resources. Choose between Cloud, Local, or Blended processing modes based on your performance and privacy preferences.

### Processing Mode

Choose how Pieces processes your materials using machine learning resources. You can select Cloud, Local, or Blended processing modes based on your performance and privacy preferences.

<Steps>
  <Step title="Open Models Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Models`.
  </Step>

  <Step title="Locate Processing Mode">
    In the *Model Capabilities* section, find the "Processing Mode" option showing your current mode (e.g., "Processing Mode: Blended").
  </Step>

  <Step title="Open Processing Mode Selector">
    Click the `Dropdown Arrow` next to the current processing mode to open the mode options.
  </Step>

  <Step title="Select Processing Mode">
    Choose from the following options:
    * **Cloud**: Optimized for speed, but all data gets sent to the cloud for processing
    * **Local**: Most processing happens locally before reaching out to the selected model, providing better privacy
    * **Blended**: Uses a combination of local and cloud resources, balancing speed and privacy
  </Step>
</Steps>

<Callout type="tip">
  Selecting the processing mode that best fits your security and performance needs ensures that Pieces processes your materials in the most efficient or privacy-conscious way possible.
</Callout>

## Local Model Runtime

Set up and manage Ollama for local model processing. Ollama allows you to run AI models locally on your device without sending data to the cloud.

### Ollama Status

Check if Ollama is installed, activated, and ready to use. Ollama must be installed and running for local model processing to work.

<Steps>
  <Step title="Open Models Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Models`.
  </Step>

  <Step title="Locate Local Model Runtime">
    Scroll down to the *Local Model Runtime* section.
  </Step>

  <Step title="Check Ollama Status">
    View the Ollama status:
    * **Activated and Ready**: Shows "Ollama is Activated and Ready" with a green checkmark and version number (e.g., "Version: 0.5.5")
    * **Not Installed**: Shows options to install Ollama
    * **Not Running**: Shows options to start Ollama
  </Step>
</Steps>

### Installing Ollama

If Ollama is not installed, you can install it directly from the Models settings page.

<Steps>
  <Step title="Open Models Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Models`.
  </Step>

  <Step title="Locate Local Model Runtime">
    Scroll down to the *Local Model Runtime* section.
  </Step>

  <Step title="Click Install Ollama">
    If Ollama is not installed, click the `Install` button or link to download and install Ollama.
  </Step>

  <Step title="Follow Installation Steps">
    Follow the installation prompts to complete the Ollama installation. Once installed, Ollama will automatically activate and be ready to use.
  </Step>
</Steps>

## Model Management

Enable or disable models to control which AI models are available for use in Pieces. Disabled models will not appear in chat or other features. Models disabled by an organization will not appear here.

### Understanding Model Management

Pieces supports a wide variety of AI models from different providers. By default, the most popular models are enabled, but you can customize which models are available based on your needs and preferences.

### Viewing Enabled Models

See how many models are currently enabled and which providers they belong to.

<Steps>
  <Step title="Open Models Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Models`.
  </Step>

  <Step title="Locate Model Management">
    Scroll down to the *Model Management* section.
  </Step>

  <Step title="View Model Count">
    At the top of the *Model Management* section, you'll see a count showing how many models are enabled out of the total available (e.g., "3 of 68 models enabled").
  </Step>
</Steps>

### Searching Models

Search for specific models or providers to quickly find what you're looking for.

<Steps>
  <Step title="Open Models Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Models`.
  </Step>

  <Step title="Locate Search Bar">
    In the *Model Management* section, find the search bar with the placeholder "Search models...".
  </Step>

  <Step title="Enter Search Term">
    Type the name of a model or provider in the search bar to filter the list of available models.
  </Step>
</Steps>

### Enabling or Disabling Models

Control which models are available by enabling or disabling them individually or by provider.

<Steps>
  <Step title="Open Models Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Models`.
  </Step>

  <Step title="Locate Model Provider">
    In the *Model Management* section, find the model provider you want to configure (e.g., OpenAI, Anthropic, Google, Microsoft, Meta, IBM).
  </Step>

  <Step title="Expand Provider">
    Click the arrow next to the provider name to expand and see all available models from that provider.
  </Step>

  <Step title="Toggle Model">
    Use the toggle switch on the right side of each model or provider to enable or disable it. Green indicates enabled, gray indicates disabled.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/configuration/models/enabling_a_model.png" alt="" align="center" fullwidth="true" />

> Models settings showing how to enable a model using the toggle switch

### Deleting Local Models

Remove local models that you no longer need. This frees up storage space on your device.

<Steps>
  <Step title="Open Models Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Models`.
  </Step>

  <Step title="Locate Local Model">
    In the *Model Management* section, find the local model you want to delete. Local models are typically from providers like Ollama or other local runtime environments.
  </Step>

  <Step title="Delete Model">
    Click the delete icon or option next to the local model to remove it from your device.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/configuration/models/delete_local_model.png" alt="" align="center" fullwidth="true" />

> Models settings showing how to delete a local model

### Enabling All Models

Quickly enable all available models at once.

<Steps>
  <Step title="Open Models Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Models`.
  </Step>

  <Step title="Locate Enable All">
    In the *Model Management* section, find the "Enable All" option with a checkmark icon.
  </Step>

  <Step title="Click Enable All">
    Click `Enable All` to enable all available models. This will make all models from all providers available for use.
  </Step>
</Steps>

### Model Providers

Pieces supports models from multiple providers. Each provider shows how many of its models are enabled:

* **OpenAI**: GPT models and other OpenAI models
* **Anthropic**: Claude models
* **Google**: Gemini and other Google models
* **Microsoft**: Azure OpenAI and other Microsoft models
* **Meta**: Llama and other Meta models
* **IBM**: Watson and other IBM models

Each provider can be expanded to see individual models, and you can enable or disable models individually or toggle the entire provider on or off.

### Compatible Models

For a complete list of all compatible models and their capabilities, see the [Compatible LLMs](/products/large-language-models) documentation. This page provides detailed information about cloud models, local models, and which models work best for different use cases.

***

## Next Steps

Now that you understand how to manage models, learn about [Long-Term Memory](/products/desktop/configuration/long-term-memory) to configure memory preferences, or explore [Model Context Protocol (MCP)](/products/desktop/configuration/mcp) to integrate Pieces with other tools. For a complete list of available models, see [Compatible LLMs](/products/large-language-models).
