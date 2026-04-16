---
title: Managing Your Account
path: /meet-pieces/managing-your-account
visibility: PUBLIC
status: PUBLISHED
description: Sign in, sign out, and understand how your Pieces account status affects PiecesOS—with links to full account settings in the Desktop App.
metaTitle: Managing Your Account | Get Started
metaDescription: Learn how to sign in and out through PiecesOS, understand what your account and subscription unlock, and access full account settings in the Pieces Desktop App.
---

## Your Account and PiecesOS

Your Pieces account is managed by **PiecesOS**—the background service that powers every Pieces tool and integration. Signing in authenticates PiecesOS directly, not just the Desktop App. This means your session, subscription entitlements, and LTM access are all tied to PiecesOS, regardless of which Pieces product you use.

A sign-in is required to use Pieces. Anonymous usage is not available.

***

## Signing In

When you launch PiecesOS for the first time (or after signing out), it will prompt you to sign in. You can also initiate sign-in from the **[PiecesOS Quick Menu](/products/core-dependencies/pieces-os/quick-menu)**—the Pieces icon in your menu bar (macOS/Linux) or system tray (Windows).

<Steps>
  <Step title="Open the Quick Menu">
    Click the Pieces icon in your menu bar or system tray.
  </Step>

  <Step title="Click Sign In">
    If you're not signed in, a `Sign In` option appears. Click it to open the authentication flow in your browser.
  </Step>

  <Step title="Choose your sign-in method">
    Sign in with GitHub, Google, Microsoft, or email. If using email, check your inbox for a verification code.
  </Step>

  <Step title="Return to Pieces">
    After authenticating in the browser, PiecesOS recognizes your session automatically. If the browser doesn't switch back, return to the app manually—PiecesOS will already be signed in.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/core-dependencies/quick-menu_sign_in.png" alt="" align="center" fullwidth="true" />

> The PiecesOS Quick Menu sign-in prompt on macOS

<Callout type="info">
  Once signed in, you stay signed in automatically across restarts. If you sign out from another device, you'll need to sign in again.
</Callout>

For troubleshooting sign-in issues, see [Sign In to Pieces](/products/meet-pieces/sign-into-pieces).

***

## Signing Out

Sign out from the **PiecesOS Quick Menu** at any time.

<Steps>
  <Step title="Open the Quick Menu">
    Click the Pieces icon in your menu bar or system tray.
  </Step>

  <Step title="Click your name">
    Click your account name at the top of the Quick Menu.
  </Step>

  <Step title="Click Log Out">
    Select `Log Out`. PiecesOS will end your session immediately.
  </Step>
</Steps>

You can also sign out from inside the Pieces Desktop App—click your `User Profile` in the top left and select `Log Out`.

***

## What Your Account Unlocks

Your account and subscription tier determine what PiecesOS can do across all integrations and tools:

| Feature | Free | Pieces Pro |
| --- | --- | --- |
| *Local LLMs* | ✓ | ✓ |
| *Cloud LLMs* (GPT-4o, Claude, Gemini) | Limited | Unlimited |
| *Long-Term Memory (LTM)* | ✓ | ✓ |
| *Pieces Cloud sync & backup* | ✓ | ✓ |
| *MCP Server* | ✓ | ✓ |

<Callout type="tip">
  Your subscription is tied to your account, not to a specific device. Sign in on any machine and your plan applies everywhere.
</Callout>

***

## Full Account Settings

Detailed account management—linked accounts, organizations, subscriptions, personal cloud, backup & restore, and privacy settings—is available in the Pieces Desktop App.

<FancyCard title="Account Settings (Desktop App)" href="/products/desktop/configuration/account" colored={false}>
  Manage linked accounts, organizations, subscriptions, personal cloud sync, backup & restore, and telemetry settings.
</FancyCard>

<FancyCard title="Sign In to Pieces" href="/products/meet-pieces/sign-into-pieces" colored={false}>
  Step-by-step sign-in instructions, update requirements, and troubleshooting for authentication issues.
</FancyCard>
