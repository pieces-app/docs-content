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

### LTM Audio

LTM Audio, also known as Audio Ingestion, enables the Long-Term Memory Engine to capture system audio and microphone input to enhance your workflow context. This feature is currently in *Preview* and requires platform-specific permissions.

<Embed
  src="https://youtu.be/vg4Mg8Xasn8"
  title="How to enable LTM Audio in Pieces Desktop"
/>

<Tabs>
  <TabItem title="macOS">
    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/audio_ingestion/v1/audio_ingestion_mac.gif" alt="" align="center" fullwidth="true" />

    > LTM Audio setup on macOS

    First-time users will see a yellow warning indicator on the `Enable LTM Audio` option when they open their `User Profile` in the top left. Click the `warning indicator` to open the permissions dialog and grant the required access.

    <Steps>
      <Step title="Open Permissions Dialog">
        Click your `User Profile` in the top left. If you see a yellow warning indicator, click it to open the "Some Permissions Are Missing" dialog. Otherwise, go to *Settings* → *Long-Term Memory* → *Long-Term Memory Permissions*.
      </Step>

      <Step title="Grant System Audio Capture">
        In the permissions dialog, locate "System Audio Capture" and click the `Allow` button. This opens the macOS *Privacy & Security* → *Screen & System Audio Recording* settings.
      </Step>

      <Step title="Add Pieces OS to System Audio Recording">
        In the *System Audio Recording Only* section at the bottom, click the `+` button. Navigate to *Applications* in Finder and select `Pieces OS`. The system will prompt you to restart Pieces OS—choose `Quit & Reopen`.
      </Step>

      <Step title="Grant Microphone Access">
        After restarting, the permissions dialog will prompt you to grant Microphone Access. Click the `Allow` button for "Microphone Access" to open the macOS *Privacy & Security* → *Microphone* settings.
      </Step>

      <Step title="Enable Microphone for Pieces OS">
        In the Microphone settings, find `Pieces OS` and turn the toggle on. Choose `Quit & Reopen` when prompted to restart Pieces OS.
      </Step>

      <Step title="Enable LTM Audio">
        Once permissions are granted, click your `User Profile` in the top left and click `Enable LTM Audio` to turn the feature on. Alternatively, click the `PiecesOS` icon in your menu bar to open the dropdown, scroll to *LTM Audio*, and enable it there.
      </Step>
    </Steps>

    <Callout type="info">
      LTM Audio is a *Preview* feature. You must grant both System Audio Capture and Microphone Access, then restart Pieces OS after each permission change, before the feature can be enabled.
    </Callout>
  </TabItem>

  <TabItem title="Windows">
    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/audio_ingestion/v1/audio_ingestion_windows.png" alt="" align="center" fullwidth="true" />

    > LTM Audio setup on Windows

    On Windows, LTM Audio prompts for microphone permission only. Accept the prompt and the feature is enabled—no system audio capture or restart required.

    Enable LTM Audio from your `User Profile` in the top left, or from the PiecesOS icon in your system tray—click it to open the dropdown, scroll to *LTM Audio*, and toggle it on.

    **If you skipped the initial permission prompt**

    You can grant microphone access through Windows Settings:

    <Steps>
      <Step title="Open Settings">
        Press `Win + I` or click the `Start` button and select `Settings`.
      </Step>

      <Step title="Navigate to Microphone settings">
        Go to `Privacy & Security` (Windows 11) or `Privacy` (Windows 10), then select `Microphone`.
      </Step>

      <Step title="Enable microphone for Pieces OS">
        Turn on *Microphone access* if it is off. Find `Pieces OS` in the list of apps and enable the toggle next to it.
      </Step>

      <Step title="Enable LTM Audio">
        Restart Pieces if it was open, then enable *LTM Audio* from your `User Profile` or the `PiecesOS` system tray dropdown.
      </Step>
    </Steps>

    <Callout type="info">
      LTM Audio is a *Preview* feature. Accept the microphone permission when prompted to enable the feature.
    </Callout>
  </TabItem>

  <TabItem title="Linux">
    On Linux (Snap installation), run `pieces-os.doctor` after installation. The script outputs a command you can copy and paste into your terminal to connect all interfaces with the system.

    Once the interfaces are connected, enable LTM Audio from your `User Profile` in the top left, or from the PiecesOS icon in your application tray—click it to open the dropdown, scroll to *LTM Audio*, and toggle it on.

    <Callout type="info">
      LTM Audio is a *Preview* feature. Run `pieces-os.doctor` to connect system interfaces before enabling the feature.
    </Callout>
  </TabItem>
</Tabs>

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
