---
title: Machine Learning
path: /desktop/configuration/copilot-and-machine-learning
visibility: PUBLIC
status: PUBLISHED
description: Configure auto-enrichment, processing modes, Long-Term Memory Engine settings, and device resource management.
metaTitle: Machine Learning Settings in Pieces Desktop
metaDescription: Configure auto-enrichment levels, processing modes, Long-Term Memory Engine settings, and device resource management.
---

***

## Machine Learning Settings

Configure how Pieces enriches your saved materials, controls local vs. cloud-based machine learning resources, and manages the Long-Term Memory Engine. Adjust auto-enrichment levels, processing modes, and device resources to match your workflow and privacy preferences.

To access Machine Learning settings, click your `User Profile` in the top left, then hover over `Settings` and select `Machine Learning`.

<Image src="https://www.jacksonsquareshopping.co.uk/wp-content/uploads/2016/12/placeholder-1920x1080-copy.png" alt="" align="center" fullwidth="true" />

> Machine Learning settings showing auto-enrichment, processing mode, and Long-Term Memory Engine options

## Saved Material Auto-Enrichment

Control how much enriched metadata is automatically attached to your saved materials. Auto-enrichment adds tags, related websites, hints, and references to help you organize and discover your materials more effectively.

### Auto-Generated Context

Set the level of enriched metadata that Pieces automatically generates for your saved materials. Higher levels provide more detailed metadata but may take longer to process.

<Steps>
  <Step title="Open Machine Learning Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Machine Learning`.
  </Step>

  <Step title="Locate Auto-Generated Context">
    In the *Saved Material Auto-Enrichment* section, find the "Auto-Generated Context" option showing your current level (e.g., "Auto-Generated Context: Medium").
  </Step>

  <Step title="Open Level Selector">
    Click the `Dropdown Arrow` next to the current level to open the enrichment level options.
  </Step>

  <Step title="Select Enrichment Level">
    Choose from the following levels:
    * **None**: No enriched metadata (0)
    * **Low**: Lower levels of enriched metadata (2-3)
    * **Medium**: Medium levels of enriched metadata (3-5)
    * **High**: Higher levels of enriched metadata (7-9)
  </Step>
</Steps>

<Image src="https://www.jacksonsquareshopping.co.uk/wp-content/uploads/2016/12/placeholder-1920x1080-copy.png" alt="" align="center" fullwidth="true" />

> Auto-Generated Context dropdown showing None, Low, Medium, and High enrichment levels with descriptions

<Callout type="info">
  By default, auto-generated context is set to *Medium*. Lower levels may be beneficial if you prefer minimal automatic annotations or need to limit processing time.
</Callout>

## ML Processing

Configure how Pieces uses local and cloud machine learning resources to process your materials and power various functions within the Pieces software experience.

### Processing Mode

Choose how Pieces processes your materials using machine learning resources. You can select Cloud, Local, or Blended processing modes based on your performance and privacy preferences.

<Steps>
  <Step title="Open Machine Learning Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Machine Learning`.
  </Step>

  <Step title="Locate Processing Mode">
    In the *ML Processing* section, find the "Processing Mode" option showing your current mode (e.g., "Processing Mode: Blended").
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

<Image src="https://www.jacksonsquareshopping.co.uk/wp-content/uploads/2016/12/placeholder-1920x1080-copy.png" alt="" align="center" fullwidth="true" />

> Processing Mode dropdown showing Cloud, Blended, and Local options with icons

<Callout type="tip">
  Selecting the processing mode that best fits your security and performance needs ensures that Pieces processes your materials in the most efficient or privacy-conscious way possible.
</Callout>

## Long-Term Memory Engine

Configure the Long-Term Memory (LTM-2.7) Engine, which uses on-device machine learning to auto-generate Workstream Activities and provide temporal context for your Conversational Search.

### Enabling Long-Term Memory Engine

Toggle the Long-Term Memory Engine on or off to control whether Pieces captures and uses your workflow context.

<Steps>
  <Step title="Open Machine Learning Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Machine Learning`.
  </Step>

  <Step title="Locate Long-Term Memory Engine">
    In the *ML Processing* section, find the "Long-Term Memory Engine" option showing your current status (e.g., "Long-Term Memory Engine: On" with a green indicator).
  </Step>

  <Step title="Toggle Long-Term Memory Engine">
    Click the toggle to enable or disable the Long-Term Memory Engine. When enabled, it uses on-device machine learning to auto-generate Workstream Activities and provide temporal context for your Conversational Search.
  </Step>
</Steps>

<Callout type="info">
  The Long-Term Memory Engine helps Pieces understand your workflow patterns and provide more contextual suggestions in Conversational Search. When disabled, Pieces won't capture or use workflow context.
</Callout>

### Long-Term Memory Source Control

Manage which sources the Long-Term Memory Engine interacts with. This allows you to control what data sources Pieces uses when capturing workflow context.

<Steps>
  <Step title="Open Machine Learning Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Machine Learning`.
  </Step>

  <Step title="Locate Long-Term Memory Source Control">
    In the *ML Processing* section, find the "Long-Term Memory Source Control" option.
  </Step>

  <Step title="Open Source Control">
    Click the `Dropdown Arrow` next to "Long-Term Memory Source Control" to manage which sources the Long-Term Memory Engine interacts with.
  </Step>
</Steps>

### Long-Term Memory Permissions

Manage accessibility and screen permissions for the Long-Term Memory Engine. If permissions are not already enabled, you can provide the necessary permissions to Pieces.

<Steps>
  <Step title="Open Machine Learning Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Machine Learning`.
  </Step>

  <Step title="Locate Long-Term Memory Permissions">
    In the *ML Processing* section, find the "Long-Term Memory Permissions" option.
  </Step>

  <Step title="Click Permissions Icon">
    Click the `Permissions Icon` to open the permissions settings. If permissions are not already enabled, you'll be prompted to provide the necessary permissions to Pieces.
  </Step>

  <Step title="Grant Permissions">
    Follow the system prompts to grant the required accessibility and screen permissions that allow the Long-Term Memory Engine to capture workflow context.
  </Step>
</Steps>

### Clearing Long-Term Memory Engine Data

Remove persisted data captured by the Long-Term Memory Engine for a specific time range. This allows you to clear workflow context while keeping the engine enabled.

<Steps>
  <Step title="Open Machine Learning Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Machine Learning`.
  </Step>

  <Step title="Locate Clear Long-Term Memory Engine Data">
    In the *ML Processing* section, find the "Clear Long-Term Memory Engine Data..." option.
  </Step>

  <Step title="Click Trash Icon">
    Click the `Trash Icon` next to "Clear Long-Term Memory Engine Data..." to open the clearing options.
  </Step>

  <Step title="Select Time Range">
    Choose the time range for the data you want to clear (e.g., last 7 days, last 30 days, all time).
  </Step>

  <Step title="Confirm Clearing">
    Confirm the clearing action when prompted. The selected Long-Term Memory Engine data will be permanently removed.
  </Step>
</Steps>

<Callout type="alert">
  Clearing Long-Term Memory Engine data is a permanent action that cannot be undone. This will remove workflow context captured during the selected time range.
</Callout>

## Device Resources

Manage device resources and optimize memory usage by unloading local machine learning models and resources from memory when not in use.

### Optimize Memory Usage

Unload local machine learning models and resources from memory to free up system resources. This is useful if you need to reduce memory usage or free up resources for other applications.

<Steps>
  <Step title="Open Machine Learning Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Machine Learning`.
  </Step>

  <Step title="Locate Device Resources Section">
    Scroll down to the *Device Resources* section at the bottom of the Machine Learning settings.
  </Step>

  <Step title="Click Optimize Memory Usage">
    Click the `Optimize Memory Usage` button (CPU/Microchip Icon) to unload local machine learning models and resources from memory.
  </Step>
</Steps>

<Image src="https://www.jacksonsquareshopping.co.uk/wp-content/uploads/2016/12/placeholder-1920x1080-copy.png" alt="" align="center" fullwidth="true" />

> Device Resources section showing Optimize Memory Usage option

<Callout type="tip">
  Optimizing memory usage can help free up system resources, but you may need to reload models when you next use features that require them, which may take a moment.
</Callout>

***

## Next Steps

Now that you understand how to configure Machine Learning settings, learn about [Conversational Search](/products/desktop/conversational-search) to query your workflow memories and get AI-powered insights, or explore [Model Context Protocol (MCP)](/products/desktop/configuration/mcp) to integrate Pieces with other tools.
