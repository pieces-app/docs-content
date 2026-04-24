---
title: Privacy, Security & Your Data
path: /privacy-security-your-data
visibility: PUBLIC
status: PUBLISHED
description: Pieces is built local-first and SOC 2 Type II certified—your code and context stay on your device by default. This page covers where your data lives, how security is designed, what runs offline, and the controls you have over telemetry and cloud features.
metaTitle: Pieces Privacy & Security | Your Data
metaDescription: How Pieces keeps your data private and secure—local-first architecture, SOC 2 Type II compliance, optional cloud features, on-device LTM processing, and full user control.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/pieces_more/privacy_security_your_data.png"
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/privacy_and_security/soc_secure_private.png" alt="" align="center" fullwidth="true" />

***

## Local-First by Design
Pieces runs on your device. Your code, chats, and long-term memory context never leave your machine unless you explicitly enable a cloud feature.

That means full offline functionality by default, opt-in cloud integrations, clearly marked telemetry, and granular controls over everything you share.

<Callout type="info">
  Pieces is **SOC 2 Type II certified** and enterprise-ready. We never use your data to train models, and you can delete everything at any time by removing the `com.pieces.os` folder.
</Callout>

## Where Your Data Lives
All Pieces data is stored in a single folder on your device—easy to back up, copy, move between machines, or delete entirely.

The `com.pieces.os` folder holds your long-term memory context, saved materials, and logs. You can copy it to OneDrive, a USB drive, or another machine without touching any cloud service.

<Tabs>
  <TabItem title="macOS">
    ```plaintext
    /Users/<username>/Library/com.pieces.os/
    ```
  </TabItem>

  <TabItem title="Windows">
    ```plaintext
    C:\Users\<username>\AppData\Local\Mesh Intelligent Technologies, Inc\Pieces OS\com.pieces.os\
    ```
  </TabItem>

  <TabItem title="Linux">
    ```plaintext
    /home/<username>/.local/share/com.pieces.os/
    ```
  </TabItem>
</Tabs>

<Callout type="tip">
  Replace `<username>` with your system username. For detailed backup and migration steps, see [On-Device Storage](/products/core-dependencies/on-device-storage).
</Callout>

## Security Architecture
Pieces is architected so your sensitive work stays isolated from external networks whenever possible.

The core design keeps processing local, makes cloud connectivity optional, and uses per-user data isolation when cloud features are enabled.

* **Offline-first processing** — code analysis, language detection, secret detection, and tag generation run on-device, minimizing exposure to external networks.
* **Opt-in cloud** — no data leaves your machine unless you enable a cloud feature.
* **Isolated user data** — each developer's data is stored in its own micro-database, preventing cross-contamination.
* **Decentralized by default** — no centralized server holds your data, so there's no single point of failure.

### What Runs Offline
These pillars of Pieces functionality work fully offline, with cloud as an optional enhancement rather than a requirement.

| **Feature**        | **Local** | **Cloud (Optional)** |
| ------------------ | :-------: | :------------------: |
| Code Analysis      |     ✅     |          ✅           |
| Language Detection |     ✅     |          ✅           |
| Secret Detection   |     ✅     |          ✅           |
| Tag Generation     |     ✅     |          ✅           |
| Long-Term Memory   |     ✅     |          ✅           |
| Conversational Chat (with local models) |     ✅     |          ✅           |

## Long-Term Memory Security
The Long-Term Memory (LTM-2.7) Engine is the most context-aware part of Pieces—and the most important to keep local.

By default, every LTM function runs on your device. You can pair it with a local LLM through PiecesOS for end-to-end on-device processing, so nothing about your work ever crosses the network.

* **On-device processing** — LTM runs locally by default, keeping sensitive context within your environment.
* **Built-in local models** — download and run local LLMs directly through PiecesOS for fully offline conversations.
* **You decide what's shared** — cloud features are opt-in per interaction, so you stay in control at every step.

<Callout type="alert">
  For the strongest privacy posture, pair LTM-2.7 with a local model. This keeps Long-Term Memory, Conversational Search, and Pieces Drive fully on-device.
</Callout>

## Privacy Controls
You have full control over what Pieces collects, stores, and sends—no dark patterns, no mandatory telemetry.

Every Pieces product exposes settings for data sharing, cloud connectivity, and telemetry so you can match the tool to your team's policies.

* **All cloud features are opt-in** — nothing is sent remotely unless you turn it on.
* **Telemetry is anonymous and opt-out** — clearly marked, never tied to your code.
* **Granular settings per product** — PiecesOS, the Desktop App, and each integration expose their own privacy controls.
* **No model training on your data** — ever.

## Cloud Integration (Optional)
When you do enable cloud features, each user gets their own isolated infrastructure rather than a shared pool.

This isolation makes Pieces cloud suitable for enterprise environments where tenancy and data segregation matter.

* **Per-user cloud instance** — your cloud environment is dedicated to your account, not shared.
* **Unique subdomain per user** — further isolates your data from other tenants.
* **Independent scaling** — performance scales with your usage without affecting other users.
* **Data isolation** — even in cloud mode, your data is segregated from every other user's.

## Compliance & Certifications
Pieces meets the standards required by enterprise security teams, with regular audits and enterprise-grade authentication.

<Steps>
  <Step title="SOC 2 Type II Certified">
    Our systems meet the stringent requirements of SOC 2 Type II—a critical benchmark for security, availability, and confidentiality in enterprise environments.
  </Step>

  <Step title="Regular Security Audits">
    We audit our infrastructure frequently to identify potential vulnerabilities and continuously improve our systems beyond the baseline that certifications require.
  </Step>

  <Step title="Enterprise Authentication with Auth0">
    Access is protected through Auth0, with support for multi-factor authentication and the advanced sign-in options enterprise teams expect.
  </Step>
</Steps>

## Privacy Policy & Questions
Our full privacy policy covers the details not addressed here. Reach out if you have specific concerns or need documentation for a security review.

* Read our <a target="_blank" href="https://pieces.app/legal/privacy-policy">Privacy Policy</a>
* <a target="_blank" href="https://calendar.app.google/WVUDtUfNy5Vst3sH7">Book a call</a> with our team
* Open a <a target="_blank" href="https://github.com/pieces-app/support/issues">GitHub issue</a> or join our <a target="_blank" href="https://pieces.app/discord">Discord</a>

***

## Next Steps
Dig deeper into how Pieces stores your data and what runs locally.

[On-Device Storage →](/products/core-dependencies/on-device-storage)

[Support →](/support)
