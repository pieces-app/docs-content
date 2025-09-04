---
title: Getting Started with Sign-In
path: /meet-pieces/sign-into-pieces
visibility: PUBLIC
status: PUBLISHED
description: Everything you need to know about signing in to Pieces, including step-by-step instructions for new and existing users, troubleshooting common issues, and understanding our new security requirements.
metaTitle: "Sign In to Pieces: Authentication Guide & Troubleshooting"
metaDescription: Learn how to sign in to Pieces Desktop App. Step-by-step guide for new and existing users, platform instructions, and troubleshooting common sign-in issues.
---

# Sign-In to the Pieces Suite

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/sign-in/sign-in.png" alt="" align="center" fullwidth="true" />

<Callout type="alert">
  **Important Security Update**

  Starting with version 12.0.0, all users must sign in to use Pieces. This change helps us prevent misuse and discourage bad actors from abusing our infrastructure. Previous versions will no longer work after this update.
</Callout>

## What's Changing

You'll need to sign in to use Pieces - no more anonymous usage. <mark>This applies to everyone</mark>, whether you're new to Pieces or have been using it for years.

## For New Users

When you open Pieces for the first time, you'll see a sign-in screen right away. The option to skip sign-in has been removed.

Here's what to do:

<Steps>
  <Step title="Choose Your Sign-In Method">
    Choose how you want to sign in; we offer a wide range of platforms to suit your needs.
  </Step>

  <Step title="Complete Authentication">
    Complete the sign-in process in your web browser.
  </Step>

  <Step title="Verify Your Email">
    If you choose email, check your inbox for a verification code.
  </Step>

  <Step title="Continue Setup">
    Once you're signed in, you'll continue with the setup process.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/sign-in/sign-in-page.png" align="center" fullwidth="false" />

## For Existing Users

When you update and open Pieces, it will check if you're signed in during startup.

### What You'll See

1. Pieces will start up normally

2. You'll see a "Sign In to use Pieces" step

3. If you're not signed in, you'll see a prompt to sign in

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/sign-in/sign_in_request.png" alt="" align="center" fullwidth="true" />

<Callout type="tip">
  We're requiring sign-in to use Pieces as of the PiecesOS 12.0.0 release to enhance security and enable new features
</Callout>

## How to Sign In

### On Mac

If the sign in prompt doesn't appear automatically:

<Steps>
  <Step title="Open the Pieces App">
    Click the **Pieces** icon in your menu bar (top of screen).
  </Step>

  <Step title="Sign in to Pieces">
    Click `Sign In` when the Pieces app opens.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/sign-in/pieces_new_os_dropdown.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

Or open Pieces directly by typing this in Terminal:

```bash
open "pieces-for-developers://open"
```

### On Windows

If the sign in prompt doesn't appear automatically:

<Steps>
  <Step title="Open the Pieces App">
    Click the **Pieces** icon in your system tray (near the clock).
  </Step>

  <Step title="Sign in to Pieces">
    Click `Sign In` when the Pieces app opens.
  </Step>
</Steps>

Or open Pieces directly by typing this in PowerShell or Command Prompt:

```powershell
start "pieces-for-developers://open"
```

### On Linux

If the sign in prompt doesn't appear automatically:

<Steps>
  <Step title="Open the Pieces App">
    Click the Pieces icon in your system tray.
  </Step>

  <Step title="Sign in to Pieces">
    Click `Sign In` when the Pieces app opens.
  </Step>
</Steps>

Or open Pieces directly by typing this in your terminal:

```bash
xdg-open "pieces-for-developers://open"
```

### Staying Signed In

Once you sign in, you should stay signed in automatically. *However*, if you sign out from another device or location, you'll need to sign in again. This keeps your account secure across all your devices.

## Troubleshooting

***

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/sign-in/flowchart2.png" alt="" align="center" fullwidth="true" />

***

### Stuck at Startup

If Pieces gets stuck at "Sign In to use Pieces" during startup, simply click the `Sign In` button that appears and complete the process in your browser.

This is intentional, as we now require every Pieces user to be logged in to use our platform.

### Authentication Failed

Getting an "authentication failed" error? Make sure you're using the same account you used before with Pieces.

### Browser Doesn't Return

After signing in, your browser might not automatically switch back to Pieces. That's okay - just manually switch back to the Pieces app. It should recognize that you've signed in successfully.

If it hasn’t, restart your Pieces and follow the sign in steps again.

### Repeatedly Signed Out

If you keep getting signed out, check that your computer's date and time are set correctly. Authentication relies on accurate time settings to keep your account secure.

***

## What's New with Sign-In

We've upgraded our sign-in system to make it better for you:

* **Combine accounts easily**: If you've signed in different ways before, you can now merge those accounts

* **More sign-in options**: Choose from more providers than ever before

* **Better security**: Enhanced protection against threats and abuse

<Callout type="tip">
  Your existing account works exactly the same - just sign in like you normally would
</Callout>

## How This Affects Your Daily Work

### Right Now

* You <mark>must update</mark> to the latest version to keep using Pieces

* You need to sign in before you can access your snippets and tools

<Callout type="alert">
  Older versions of Pieces Desktop and PiecesOS will be depreciated and will not work anymore. You must update to version 12.0.0 to use the Pieces Suite.
</Callout>

## Keeping Your Account Safe

Here are simple ways to protect your Pieces account:

1. Use a strong password if signing in with email.

2. Turn on two-factor authentication with your sign-in provider.

3. Sign out when using shared computers.

4. Let us know immediately if you see anything suspicious.

## Updating to the Latest Version

To use the new sign-in features, you'll need to update both PiecesOS and the Pieces Desktop app.

### Update PiecesOS

PiecesOS runs in the background and powers all Pieces features.

To update:

<Steps>
  <Step title="Find PiecesOS">
    Check your menu bar (Mac) or system tray (Windows/Linux) for the PiecesOS icon.
  </Step>

  <Step title="Open Update Options">
    Right-click the icon and select `You’re up to date`—this will trigger an automatic check for updates.
  </Step>

  <Step title="Install Update">
    If an update is available, click "Update Now".
  </Step>

  <Step title="Wait for Restart">
    PiecesOS will restart automatically when complete.
  </Step>
</Steps>

### Update Pieces Desktop App

After updating PiecesOS, update the desktop app:

<Steps>
  <Step title="Open Pieces">
    Launch the Pieces Desktop App.
  </Step>

  <Step title="Check for Updates">
    Click your profile icon (right side of the search bar) and select `Check for Desktop App Updates`.
  </Step>

  <Step title="Install Update">
    Click `Update` when prompted to download and install the latest version.
  </Step>

  <Step title="Restart App">
    Restart the app when the update completes.

    <Callout type="info">
      You may also see an update notification automatically when you open either of the apps.
    </Callout>
  </Step>
</Steps>

<Callout type="alert">
  Both components must be updated to version 12.0.0 or later for sign-in to work properly. If you're having issues, make sure both PiecesOS and the Desktop App are fully updated.
</Callout>

***

## Need Help?

Having trouble signing in or have questions? We're here to help:

## Live Support with Pieces

We want to ensure that your experience with PiecesOS, the Pieces Desktop App, and any of our IDE or browser integrations is as smooth and seamless as possible—and part of that is speaking with as many users as possible so we can continue iterating and improving on Pieces products.

If you need help getting everything up and running, feel free to book a call with our Founders & Engineering Leaders via <a target="_blank" href="https://calendar.google.com/calendar/u/0/appointments/schedules/AcZssZ22WJ2Htd2wRMJhueCNYc0xbFBFCAN-khijcuoXACd_Uux3wIhgZeGkzDRcqD3teamAI-CwCHpr">our support calendar.</a>

## Open a GitHub Issue<a target="_blank" href="/extensions-plugins/sublime#get-support-or-share-feedback">**​**</a>

You can open GitHub issues for PiecesOS, the Pieces Desktop App, or any other Pieces plugin or extension by <a target="_blank" href="https://github.com/pieces-app/support/issues">opening an issue in our GitHub repository.</a>

If you would prefer not to use GitHub, you can still <a target="_blank" href="https://getpieces.typeform.com/to/mCjBSIjF#page=docs-support">leave feedback or report a bug here.</a>

## Join our Discord Community

We have a strong community presence on <a target="_blank" href="https://discord.com/invite/getpieces">our Discord channel,</a> so feel free to reach out to other users or members of the Pieces team.

You can also catch up on product updates, speak with our power users, or participate in weekly Community Events.

## Join Community Discussions

We’re active within our community and are always looking for feedback and suggestions from our power users.

If this is you, feel free to <a target="_blank" href="https://github.com/pieces-app/support/discussions">create or read through existing discussions on our GitHub</a>—that way you can inform our product roadmap and contribute feature requests.
