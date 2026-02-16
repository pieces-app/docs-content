---
title: Get Started with the Pieces Desktop App
path: /desktop/onboarding
visibility: PUBLIC
status: PUBLISHED
description: The Onboarding feature guides you through the initial stages of the Pieces Desktop App and sets you on your way to using the Long-Term Memory (LTM-2.7) Engine.
metaTitle: Pieces Onboarding
metaDescription: Get up and running with the Pieces Desktop App with this guided LTM + Conversational Search onboarding experience.
---

## Signing In

When you first launch the Pieces Desktop App, you'll be prompted to sign in with GitHub, Google, or other authentication providers. Signing in enables you to store snippets and backups in *Pieces Cloud* and import code Gists. Pieces stores materials locally by default, and you can share them with anyone you'd like.

<Steps>
  <Step title="Launch Pieces Desktop App">
    Open the Pieces Desktop App on your device.
  </Step>
  <Step title="Choose Sign-In Method">
    Select your preferred sign-in method from the available options (GitHub, Google, Microsoft, or other providers).
  </Step>
  <Step title="Complete Authentication">
    Follow the prompts to complete authentication with your chosen provider.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/onboarding/second_rv_pfd_onboarding/revised_login_page.png" alt="" align="center" fullwidth="true" />

> Login page showing sign-in options including GitHub, Google, and other authentication providers

## Setting Up Preferences

After signing in, configure your initial preferences including theme mode and data sharing settings. These settings help personalize your Pieces experience.

<Steps>
  <Step title="Choose Theme Mode">
    Select `Light` or `Dark` theme mode to suit your preferences, or choose `System` to match your operating system's theme. This mode can be changed later in [Appearance settings](/products/desktop/configuration/appearance).
  </Step>
  <Step title="Configure Data Sharing (Optional)">
    Decide if you want to share *anonymous crash data* to help improve the product. This setting can be changed later in [Troubleshooting settings](/products/desktop/configuration/troubleshooting).
  </Step>
  <Step title="Start Onboarding">
    Click `Get Started` to begin the onboarding process and start using Pieces.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/onboarding/second_rv_pfd_onboarding/revised_step_1.png" alt="" align="center" fullwidth="true" />

> Theme selection screen showing Light and Dark theme options, anonymous crash data toggle, and Get Started button

## Initial Memory Formation

After clicking `Get Started`, you'll land on the homepage of the Pieces Desktop App. The [Long-Term Memory (LTM-2.7)](/products/core-dependencies/pieces-os#ltm-27) Engine needs to capture workflow context before you can use all features. You'll see the *Single-Click Summaries* section with six cards that are locked until memory formation completes.

The homepage displays the *Single-Click Summaries* section with six cards: `What's Top of Mind`, `Standup Update`, `Time Breakdown`, `Custom Summary`, `Day Recap`, and `Discover`. These cards are grayed out and locked until memory formation completes. Below this section, you'll see the *Forming Initial Memories* progress tracker showing how many of the 30 required memories have been captured.

### Understanding the LTM Welcome Screen

When you first arrive at the homepage, you'll see the LTM welcome screen that explains Long-Term Memory and its benefits. This screen introduces you to how Pieces captures and uses your workflow context to provide personalized AI assistance.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/Onboarding/ltm_welcome.png" alt="" align="center" fullwidth="true" />

> LTM welcome screen explaining Long-Term Memory and its benefits

### Creating Initial Memories

After clicking `Got It` on the LTM welcome screen, you'll see the initial memory formation interface. This screen shows the progress of memory formation and introduces you to Single-Click Summaries that will become available once memories are captured.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/Onboarding/creating_initial_memories.png" alt="" align="center" fullwidth="true" />

> Initial memory formation screen showing progress tracker, memory formation status, and Single-Click Summary cards

### Capturing Workflow Context

Continue with your normal workflow for 10-15 minutes while LTM-2.7 captures workflow context in the background. The progress tracker shows memory formation status, and you can see which memories have been formed as you work. Each memory appears with a checkmark and description once it's been captured.

<Steps>
  <Step title="Continue Your Workflow">
    Use your computer normally—browse documentation, write code, use your IDE, or work in other applications. LTM-2.7 captures workflow context automatically in the background.
  </Step>
  <Step title="Monitor Progress">
    Watch the progress tracker to see memory formation status. The tracker shows "X/30" memories captured, and you can see which memories have been formed as you work.
  </Step>
  <Step title="Wait for Completion">
    Once 30 memories are captured, the *Single-Click Summaries* cards unlock and become clickable.
  </Step>
</Steps>

### Unlocking Features

Once you've successfully captured 30 memories, the six *Single-Click Summaries* cards become clickable and unlock. You can now generate summaries like `Standup Update`, `Day Recap`, `What's Top of Mind`, and more. Each card provides one-click access to contextual summaries based on your captured workflow data, giving you instant insights into your productivity and work patterns.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/timeline/exploring_pieces_timeline.gif" alt="" align="center" fullwidth="true" />

> Pieces Timeline showing unlocked Single-Click Summary cards and workflow events

## Using Conversational Search

[LTM](/products/core-dependencies/pieces-os#ltm-27) captures and stores workflow context, enabling you to use [Conversational Search](/products/desktop/conversational-search) as an AI assistant trained on your personal workflow data. All data is kept on-device for privacy, so your conversations and memories stay secure.

### Understanding Conversational Search

Conversational Search lets you ask questions about your workflow and get context-aware responses powered by LTM-2.7. You can visit sites like Stack Overflow, read code explanations, and later query Conversational Search about what you read. By enabling LTM, you can use Conversational Search as an AI assistant trained on your personal workflow data, making it uniquely helpful for your specific work patterns and projects.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/using-conversational-search/model_selection_in_desktop_app.png" alt="" align="center" fullwidth="true" />

> Conversational Search interface showing model selection dropdown and available models

<Callout type="info">
  Read more about [data collection and storage](/products/core-dependencies/on-device-storage).
</Callout>

### Accessing Conversational Search

Access Conversational Search directly from the homepage to ask questions about your workflow, with LTM providing context from your captured memories. You can switch between cloud-hosted and local models using the model selector in the chat interface.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/conversational-search/using-conversational-search/conversational_chat_with_sample_question.png" alt="" align="center" fullwidth="true" />

> Typing a prompt into Conversational Search input field

***

## Next Steps

You've completed the Pieces onboarding and are ready to start exploring the app. Learn more about key features and how to utilize the Pieces ecosystem in your daily workflow.

### Explore Key Features

* **[Conversational Search](/products/desktop/conversational-search)** - Ask questions about your workflow, get context-aware responses, and receive insights powered by LTM-2.7—all in a chat format you know.

* **[Pieces Timeline](/products/desktop/timeline)** - View incremental workflow summaries, saved context, and related information gathered by the Long-Term Memory (LTM-2.7) Engine.

* **[Single-Click Summaries](/products/desktop/single-click-summaries)** - Generate instant, contextual summaries from your workflow using preset summary types.

### Customize Your Experience

* **[Configuration](/products/desktop/configuration)** - Customize everything from visuals and aesthetics to Conversational Search models to fit your preferences and workflow.

* **[Navigation](/products/desktop/navigation)** - Learn the different views and layouts in the Pieces Desktop App.

* **[Actions & Keyboard Shortcuts](/products/desktop/actions)** - Use *Power Menu* Actions and Keyboard Shortcuts to perform tasks or navigate from view to view quickly.

### Get Help

* **[Troubleshooting](/products/desktop/troubleshooting)** - If the Pieces Desktop App isn't working as expected, start here. This page explains our troubleshooting documentation and guides you to the solution that best addresses your issue.
