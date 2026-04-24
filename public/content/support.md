---
title: Support
path: /support
visibility: PUBLIC
status: PUBLISHED
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/support/pieces_support.png"
description: Get help with Pieces—book a call with our engineers, open a GitHub issue, join our Discord, or send feedback. This page also shows where to find your logs on macOS, Windows, and Linux.
metaTitle: Pieces Support & Help Center
metaDescription: Reach the Pieces team for live support, report bugs on GitHub, share feedback, or locate your PiecesOS logs on macOS, Windows, and Linux.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair/support/support_banner.png" alt="" align="center" fullwidth="true" />

***

## Getting Help
The fastest way to get a response depends on what you need—pick the option that matches your situation.

We read every report, reply to GitHub issues directly, and our founders regularly hop on calls with users to make sure Pieces fits your workflow.

<CardGroup cols={2}>
  <Card title="Book a Live Call" image="/assets/icons/platform_logos/pieces_logo.png" href="https://calendar.app.google/WVUDtUfNy5Vst3sH7" external="true">
    Talk directly with our Founders & Engineering Leaders—great for onboarding help, workflow feedback, or walking through an issue together.
  </Card>

  <Card title="Open a GitHub Issue" image="/assets/icons/github.svg" href="https://github.com/pieces-app/support/issues" external="true">
    Report bugs, request features, or track known issues for PiecesOS, the Desktop App, and any MCP integration.
  </Card>

  <Card title="Join our Discord" image="/assets/icons/discord.svg" href="https://discord.com/invite/getpieces" external="true">
    Chat with the team and other power users, catch release notes, and join weekly community events.
  </Card>

  <Card title="Send Feedback" image="/assets/icons/annotation.svg" href="https://getpieces.typeform.com/to/mCjBSIjF#page=docs-support" external="true">
    Prefer not to use GitHub? Drop us a note—bug reports and feature requests both welcome.
  </Card>
</CardGroup>

<Callout type="tip">
  If you're reporting a bug, please include your logs. See [Finding Your Logs](#finding-your-logs) below—attaching them to your GitHub issue helps us reproduce and fix the problem much faster.
</Callout>

## Finding Your Logs
Your PiecesOS logs live in a per-platform application folder. Share the whole `Support` folder when filing a bug to help us diagnose it quickly.

Zip the folder before attaching it to a GitHub issue or sending it to support—logs are plain text, but zipping keeps everything in order.

<Tabs>
  <TabItem title="macOS">
    ### macOS
    Open Finder, press `⌘+shift+g`, and paste the path below:

    ```plaintext
    ~/Library/com.pieces.os/production/support/
    ```

    <Callout type="tip">
      If the `Library` folder is hidden, press `⌘+shift+.` (period) in Finder to toggle hidden files.
    </Callout>

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/support/mac_support.png" alt="" align="center" fullwidth="true" />

    > Locating Pieces log files on macOS
  </TabItem>

  <TabItem title="Windows">
    ### Windows
    Press `Win+R` to open the Run dialog, then paste:

    ```powershell
    C:\Users\<username>\AppData\Local\Mesh Intelligent Technologies, Inc\Pieces OS\com.pieces.os\production\Support
    ```

    <Callout type="tip">
      Replace `<username>` with your system username. If `AppData` is hidden, enable `View → Show → Hidden items` in File Explorer.
    </Callout>

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/support/windows_support.png" alt="" align="center" fullwidth="true" />

    > Locating Pieces log files on Windows
  </TabItem>

  <TabItem title="Linux">
    ### Linux
    Open your file manager or a terminal and navigate to:

    ```bash
    ~/.local/share/com.pieces.os/
    ```

    <Callout type="tip">
      In most file managers, press `ctrl+h` to toggle hidden files so you can see the `.local` directory.
    </Callout>

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/support/linux_support.png" alt="" align="center" fullwidth="true" />

    > Locating Pieces log files on Linux
  </TabItem>
</Tabs>

## Joining the Community
If you're looking for longer-form conversations, feature brainstorms, or answers from other developers, our community spaces are the right place.

We use these channels to inform the roadmap—feature requests and discussions here genuinely shape what we build next.

* **<a target="_blank" href="https://discord.com/invite/getpieces">Discord</a>** — live chat, release announcements, and weekly community events.
* **<a target="_blank" href="https://github.com/pieces-app/support/discussions">GitHub Discussions</a>** — longer-form threads, Q&A, and roadmap input.

***

## Next Steps
Not finding what you need in the docs? Browse common setup and account questions, or jump back to the product overview.

[Troubleshooting PiecesOS →](/products/core-dependencies/pieces-os/troubleshooting)

[Privacy, Security & Your Data →](/privacy-security-your-data)
