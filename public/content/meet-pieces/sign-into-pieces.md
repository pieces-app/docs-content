---
title: Getting Started with Sign-In
path: /meet-pieces/sign-into-pieces
visibility: PUBLIC
status: PUBLISHED
description: Everything you need to know about signing in to Pieces, including step-by-step instructions, troubleshooting common issues, and understanding our new security requirements.
metaTitle: "Sign In to Pieces: Authentication Guide & Troubleshooting"
metaDescription: Learn how to sign in to Pieces Desktop App. Step-by-step guide for new and existing users, platform instructions, and troubleshooting common sign-in issues.
---

## Signing In to Pieces

Whether you're new to Pieces or have used it for years, you'll need to sign in to use Pieces—anonymous usage is no longer available. We've upgraded our sign-in system with more sign-in options, better security, and the ability to combine accounts easily. Your existing account works exactly the same; just sign in like you normally would.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/sign-in/sign-in.png" alt="" align="center" fullwidth="true" />

> The Pieces sign-in screen

## Sign-In Process

When you open Pieces, you'll see a sign-in screen. Both new and existing users follow the same sign-in flow.

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
    Once you're signed in, you'll continue with the setup process or return to your workspace.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/sign-in/sign-in-page.png" alt="" align="center" fullwidth="true" />

> The sign-in screen you'll see when opening Pieces

### Accessing Sign-In

If the sign-in prompt doesn't appear automatically, you can access it from your system tray or menu bar:

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/sign-in/must-sign-up.png" alt="" align="center" fullwidth="true" />

> If you're not signed in, you'll see a prompt to sign in

<Tabs>
  <Tab title="macOS">
<Steps>
  <Step title="Open the Pieces App">
        Click the Pieces icon in your menu bar (top of screen).
  </Step>
      <Step title="Sign In">
    Click `Sign In` when the Pieces app opens.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/paid_plan/update-to-pieces-pro.png" alt="" align="center" fullwidth="true" />

        > Pieces menu bar dropdown showing Sign In option
      </Step>
    </Steps>
  </Tab>

  <Tab title="Windows">
    <Steps>
      <Step title="Open the Pieces App">
        Click the Pieces icon in your system tray (near the clock).
      </Step>
      <Step title="Sign In">
        Click `Sign In` when the Pieces app opens.
      </Step>
    </Steps>
  </Tab>

  <Tab title="Linux">
    <Steps>
      <Step title="Open the Pieces App">
        Click the Pieces icon in your system tray.
      </Step>
      <Step title="Sign In">
        Click `Sign In` when the Pieces app opens.
  </Step>
</Steps>
  </Tab>
</Tabs>

### Staying Signed In

Once you sign in, you should stay signed in automatically. However, if you sign out from another device or location, you'll need to sign in again. This keeps your account secure across all your devices.

## Requirements and Updates

To use the new sign-in features, you must update both PiecesOS and the Pieces Desktop app to version 15.0.0 or later. Older versions of Pieces Desktop and PiecesOS will be deprecated and will not work anymore.

<Callout type="alert">
  You must update to version 15.0.0 or later to use the Pieces Suite. Both PiecesOS and the Desktop App must be updated for sign-in to work properly.
</Callout>

### Update PiecesOS

PiecesOS runs in the background and powers all Pieces features.

<Steps>
  <Step title="Find PiecesOS">
    Check your menu bar (Mac) or system tray (Windows/Linux) for the PiecesOS icon.
  </Step>

  <Step title="Open Update Options">
    Right-click the icon and select `You're up to date`—this will trigger an automatic check for updates.
  </Step>

  <Step title="Install Update">
    If an update is available, click `Update Now`.
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

## Troubleshooting

If you encounter issues while signing in, try these solutions:

### Opening Pieces via Command Line

If the Pieces app doesn't open automatically, you can launch it directly from your terminal or command line:

<Tabs>
  <Tab title="macOS">
    Open Terminal and run:

    ```bash
    open "pieces-for-developers://open"
    ```
  </Tab>

  <Tab title="Windows">
    Open PowerShell or Command Prompt and run:

    ```powershell
    start "pieces-for-developers://open"
    ```
  </Tab>

  <Tab title="Linux">
    Open your terminal and run:

    ```bash
    xdg-open "pieces-for-developers://open"
    ```
  </Tab>
</Tabs>

### Stuck at Startup

If Pieces gets stuck at "Sign In to use Pieces" during startup, simply click the `Sign In` button that appears and complete the process in your browser. This is intentional, as we now require every Pieces user to be logged in to use our platform.

### Authentication Failed

Getting an "authentication failed" error? Make sure you're using the same account you used before with Pieces.

### Browser Doesn't Return

After signing in, your browser might not automatically switch back to Pieces. That's okay—just manually switch back to the Pieces app. It should recognize that you've signed in successfully. If it hasn't, restart your Pieces and follow the sign-in steps again.

### Repeatedly Signed Out

If you keep getting signed out, check that your computer's date and time are set correctly. Authentication relies on accurate time settings to keep your account secure.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/sign-in/flowchart2.png" alt="" align="center" fullwidth="true" />

> Troubleshooting flowchart for sign-in issues

## Keeping Your Account Safe

Here are simple ways to protect your Pieces account:

* Use a strong password if signing in with email
* Turn on two-factor authentication with your sign-in provider
* Sign out when using shared computers
* Let us know immediately if you see anything suspicious

## Getting Help

Having trouble signing in or have questions? We're here to help:

* **[Live Support](https://calendar.app.google/WVUDtUfNy5Vst3sH7)**: Book a call with our Founders & Engineering Leaders
* **[GitHub Issues](https://github.com/pieces-app/support/issues)**: Report bugs, request features, and track known issues
* **[Discord Community](https://discord.com/invite/getpieces)**: Join our community for support, discussions, and direct interaction with the Pieces team
* **[Community Discussions](https://github.com/pieces-app/support/discussions)**: Create or read through existing discussions to inform our product roadmap
* **[Feedback Form](https://getpieces.typeform.com/to/mCjBSIjF#page=docs-support)**: Leave feedback or report bugs without using GitHub

***

## Next Steps

Now that you're signed in, explore what Pieces can do for you.

[Getting Started with Pieces →](/products/meet-pieces)
