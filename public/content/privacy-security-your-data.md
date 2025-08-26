---
title: Privacy, Security & Your Data
path: /privacy-security-your-data
visibility: PUBLIC
status: PUBLISHED
description: At Pieces for Developers, we believe that your trust is paramount—that’s why we’ve built our platform with a local-first approach that keeps your code and data safely on your device by default.
metaTitle: Pieces Privacy & Security | Your Data
metaDescription: Understand how Pieces handles privacy, security, and data protection to keep your AI-assisted development experience secure.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/pieces_more/privacy_security_your_data.png"
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/privacy_and_security/soc_secure_private.png" alt="" align="center" fullwidth="true" />

***

## Private and Secure

Your privacy and security are our **top priorities.**

Pieces for Developers is built with a local-first architecture, so your code stays on-device by default, with complete offline functionality and cloud capabilities *only if enabled.*

Designed for complete user control, all cloud features are opt-in only, telemetry is clearly marked and opt-out of, and you have full control over all privacy settings.

***

🛡️ *We are SOC 2 Certified & Enterprise-Ready!*

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/privacy_and_security/soc_compliance.png" alt="" align="center" fullwidth="true" />

***

## Data Storage & Control

All of your data is stored locally. When interacting with cloud-based LLMs, Pieces for Developers defaults to the model provider’s Privacy Policy—like OpenAI—since we use their API to provide the model.

### Where Your Data Lives

All Pieces for Developers data is stored on your device and can be deleted, copied, compressed, or moved between devices without relying on cloud services. This allows easy transfer, simple backup, and no cloud dependency.

At any time, you can find your up-to-date log files can find your log files in the following locations, depending on your platform:

* macOS: `/Users/<username>/Library/com.pieces.os/`

* Windows: `C:/Users/<username>/Documents/com.pieces.os/`

* Linux: `/Users/<username>/Documents/com.pieces.os/`

<Callout type="tip">
  Replace \<username> with your system username.
</Callout>

## Security Architecture

Our system is built to run entirely on your device, ensuring your data never leaves your machine unless you choose to use cloud features.

* **All Core Features Work Offline:** Our platform runs on-device, processing your *code and sensitive data locally.* This minimizes exposure to external networks and reduces unauthorized access risks.

* **No Mandatory Cloud Connectivity:** You control your data. Cloud services are optional, and *no data is sent or stored remotely* unless you enable it.

* **Private By Default:** Your development environment is *isolated from external servers* by default, enhancing security and reducing data breach risks.

### Enterprise Security Features

We provide robust, isolated data storage and a scalable architecture designed to meet the high security demands of enterprise environments.

* **Individual User Repositories:** Each developer's data is stored separately in isolated micro-databases to prevent cross-contamination.

* **No Centralized Servers:** Our decentralized approach avoids a single point of failure, reducing the risk of large-scale breaches.

* **Dedicated Cloud Instances (If Enabled):** For those using cloud connectivity, we provide dedicated instances with high isolation, security, and enterprise-grade scalability.

### Compliance & Certifications

Our platform meets stringent industry standards—with SOC-2 compliance and regular security audits—ensuring you can trust our secure infrastructure.

<Steps>
  <Step title="SOC-2 Compliant Infrastructure">
    Our systems meet the *stringent requirements* of SOC-2 compliance, a critical benchmark for security in enterprise environments. 
  </Step>

  <Step title="Regular Security Audits">
    We conduct frequent audits of our infrastructure to ensure that our security practices not only meet but exceed industry standards.

    These audits help us identify potential vulnerabilities and *continuously improve* our systems.
  </Step>

  <Step title="Enterprise-Ready Authentication with Auth0">
    Secure access is key to our security. Using Auth0, we ensure only *authorized* users access sensitive data, with advanced and multi-factor authentication options for extra protection.
  </Step>
</Steps>

## Privacy Controls

We ensure users have full control over their privacy settings, data collection, and telemetry. **All data collection is opt-out**, telemetry is anonymous, and there are *clear opt-out options* in all our products.

Each Pieces product offers detailed settings for *data sharing, Cloud connectivity, and telemetry controls.*

<Callout type="tip">
  Our tools keep your data safe by processing it on your device. Tasks run locally, and we *never* use your data to train models. You can disable cloud processing anytime to keep data on your device.
</Callout>

### Available Offline Features

Many of the core pillars of Pieces for Developers functionality have been designed to be offline-flexible.

***

| **Feature**        | **Local Available** | **Cloud Optional** |
| ------------------ | ------------------- | ------------------ |
| Code Analysis      | ✅                   | ✅                  |
| Language Detection | ✅                   | ✅                  |
| Secret Detection   | ✅                   | ✅                  |
| Tag Generation     | ✅                   | ✅                  |

***

### Cloud Integration (Optional)

For users who choose to leverage cloud-based features, our platform offers secure, scalable cloud integration while keeping you in full control.

* **Individual Cloud Infrastructure:** Each user gets their own dedicated cloud setup so your data remains isolated and secure.

* **Unique Subdomain Per User:** Your cloud instance is accessed via a unique subdomain, further isolating your data from others.

* **Independent Scaling:** Our cloud services automatically scale based on *your* usage so you get consistent performance without compromising security.

* **Data Isolation:** Even when using cloud functionalities, we make sure your data remains segregated from other users’ data.

### Long-Term Memory (LTM-2.5) Security

Our Long-Term Memory (LTM-2.5) Engine is designed to protect your work through on-device processing and advanced local integration options.

* **On-device Processing:** All LTM functions run locally by default, keeping your sensitive data within your own environment.

* **Local LLM Options via** <a target="_blank" href="https://ollama.com/">Ollama</a>: You can integrate with local LLMs through the Pieces client’s usage of Ollama as a local model wrapper for added security.

* **Complete Control Over Data Sharing:** Decide when and if your data is shared, so you can be confident that you maintain full ownership and control over your information.

<Callout type="alert">
  For users concerned about privacy, we strongly recommend using a local LLM with Pieces for Developers products, so LTM-2.5, Pieces Copilot and Pieces Drive never send data through the cloud.
</Callout>

## Privacy Policy Updates

We maintain transparency about <a target="_blank" href="https://pieces.app/legal/privacy-policy">our privacy practices</a>.

For the latest updates or specific concerns, please <a target="_blank" href="https://calendar.google.com/calendar/u/0/appointments/schedules/AcZssZ22WJ2Htd2wRMJhueCNYc0xbFBFCAN-khijcuoXACd_Uux3wIhgZeGkzDRcqD3teamAI-CwCHpr">contact our support team.</a>

***

### Support & Documentation

Need help or have questions about privacy?

* Visit our [Support Page](/products/support)

* Join our <a target="_blank" href="https://pieces.app/discord">Discord community</a>

* Open a <a target="_blank" href="https://github.com/pieces-app/support/issues">GitHub issue</a>