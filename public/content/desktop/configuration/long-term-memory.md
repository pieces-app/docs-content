---
title: Long-Term Memory
path: /desktop/configuration/long-term-memory
visibility: PUBLIC
status: PUBLISHED
description: Manage long-term memory preferences and data.
metaTitle: Long-Term Memory Settings in Pieces Desktop
metaDescription: Manage long-term memory preferences, app access control, system permissions, and stored data.
---

## Long-Term Memory Settings

Manage long-term memory preferences and data. Configure the Long-Term Memory Engine, control which applications Pieces can access, manage system permissions, optimize performance, and clear stored data.

To access Long-Term Memory settings, click your `User Profile` in the top left, then hover over `Settings` and select `Long-Term Memory`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/configuration/long-term-memory/long-term_memory_settings.png" alt="" align="center" fullwidth="true" />

> Long-Term Memory settings showing Memory Formation, Performance, and Stored Data sections

## Memory Formation

Configure how the Long-Term Memory Engine captures and processes your workflow context. The Long-Term Memory (LTM-2.7) Engine uses on-device machine learning to auto-generate Workstream Activities and provide temporal context for your Conversational Search.

### Long-Term Memory Engine

Toggle the Long-Term Memory Engine on or off to control whether Pieces captures and uses your workflow context.

<Steps>
  <Step title="Open Long-Term Memory Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Long-Term Memory`.
  </Step>

  <Step title="Locate Long-Term Memory Engine">
    In the *Memory Formation* section, find the "Long-Term Memory Engine" option showing your current status (e.g., "Long-Term Memory Engine: On" with a green indicator).
  </Step>

  <Step title="Toggle Long-Term Memory Engine">
    Click the toggle or button to enable or disable the Long-Term Memory Engine. When enabled, it uses on-device machine learning to auto-generate Workstream Activities and provide temporal context for your Conversational Search.
  </Step>
</Steps>

<Callout type="info">
  The Long-Term Memory Engine helps Pieces understand your workflow patterns and provide more contextual suggestions in Conversational Search. When disabled, Pieces won't capture or use workflow context.
</Callout>

### App Access Control

Manage which applications the Long-Term Memory Engine interacts with. This allows you to control what data sources Pieces uses when capturing workflow context.

<Steps>
  <Step title="Open Long-Term Memory Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Long-Term Memory`.
  </Step>

  <Step title="Locate App Access Control">
    In the *Memory Formation* section, find the "App Access Control" option with the description "Manage apps that Long-Term Memory interacts with".
  </Step>

  <Step title="Open App Access Control">
    Click the `Dropdown Arrow` or icon next to "App Access Control" to manage which applications the Long-Term Memory Engine interacts with.
  </Step>

  <Step title="Configure Applications">
    Enable or disable specific applications that you want Long-Term Memory to capture data from. Applications that are enabled will have their workflow context captured and indexed.
  </Step>
</Steps>

### System Permissions

Manage accessibility and screen permissions for the Long-Term Memory Engine. If permissions are not already enabled, you can provide the necessary permissions to Pieces.

<Steps>
  <Step title="Open Long-Term Memory Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Long-Term Memory`.
  </Step>

  <Step title="Locate System Permissions">
    In the *Memory Formation* section, find the "System Permissions" option with the description "Manage accessibility and screen permissions for LTM".
  </Step>

  <Step title="Click Permissions Icon">
    Click the `Permissions Icon` to open the permissions settings. If permissions are not already enabled, you'll be prompted to provide the necessary permissions to Pieces.
  </Step>

  <Step title="Grant Permissions">
    Follow the system prompts to grant the required accessibility and screen permissions that allow the Long-Term Memory Engine to capture workflow context.
  </Step>
</Steps>

## Performance

Optimize system resources and manage memory usage for the Long-Term Memory Engine.

### Optimize System RAM Usage

Unload local machine learning models and resources from memory to free up system resources. This is useful if you need to reduce memory usage or free up resources for other applications.

<Steps>
  <Step title="Open Long-Term Memory Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Long-Term Memory`.
  </Step>

  <Step title="Locate Performance Section">
    Scroll down to the *Performance* section.
  </Step>

  <Step title="Click Optimize System RAM Usage">
    Click the `Optimize System RAM Usage` button (CPU/Microchip Icon) to unload local machine learning models and resources from memory.
  </Step>
</Steps>

<Callout type="tip">
  Optimizing memory usage can help free up system resources, but you may need to reload models when you next use features that require them, which may take a moment.
</Callout>

## Stored Data

Manage and clear persisted data captured by the Long-Term Memory Engine.

### Clearing Long-Term Memory Data

Remove persisted data captured by the Long-Term Memory Engine for a specific time range. This allows you to clear workflow context while keeping the engine enabled.

<Steps>
  <Step title="Open Long-Term Memory Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Long-Term Memory`.
  </Step>

  <Step title="Locate Clear LTM Data">
    Scroll down to the *Stored Data* section, find the "Clear LTM Data..." option.
  </Step>

  <Step title="Click Trash Icon">
    Click the `Trash Icon` next to "Clear LTM Data..." to open the clearing options.
  </Step>

  <Step title="Select Time Range">
    Choose the time range for the data you want to clear (e.g., last 7 days, last 30 days, all time).
  </Step>

  <Step title="Confirm Clearing">
    Confirm the clearing action when prompted. The selected Long-Term Memory Engine data will be permanently removed.
  </Step>
</Steps>

<Callout type="alert">
  Clearing Long-Term Memory data is a permanent action that cannot be undone. This will remove workflow context captured during the selected time range.
</Callout>

***

## Next Steps

Now that you understand how to manage Long-Term Memory settings, learn about [Models](/products/desktop/configuration/models) to configure AI models and processing modes, or explore [Conversational Search](/products/desktop/conversational-search) to query your workflow memories and get AI-powered insights.
