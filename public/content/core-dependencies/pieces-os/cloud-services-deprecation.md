---
title: "Update Required for Cloud Services"
path: /core-dependencies/pieces-os/cloud-services-deprecation
visibility: PUBLIC
status: PUBLISHED
description: "Action required by Friday, June 5th 2026: cloud services for PiecesOS versions prior to 12.4.0 will be deprecated. Update before that date to continue using Chat, Work Summaries, and Single Click Summaries."
metaTitle: "Update Required for Cloud Services | PiecesOS"
metaDescription: Cloud services for PiecesOS versions prior to 12.4.0 will be deprecated on Friday, June 5th 2026. Update to 12.4.0 or later to continue using Chat, Work Summaries, and Single Click Summaries.
---

## Summary

On Friday, June 5th 2026, we will be deprecating cloud services for all PiecesOS versions prior to 12.4.0. If you are running an older version of PiecesOS, you will need to update to 12.4.0 or later before that date to continue using cloud-backed features.

## Who is Affected

You are affected if your PiecesOS version is lower than 12.4.0.

To check your version:

* **Desktop App**: `Settings` → `About` → *PiecesOS Version*

## What Will Stop Working After June 6th, 2025

On deprecated versions, the following features will no longer function and will return an error:

* **Chat** — conversations, follow-ups, and any model-backed responses will fail
* **Work Summaries** — will fail to generate
* **Single Click Summaries** — will fail to generate

All other functionality (local features, account access, etc.) will continue to work as expected.

## What You Need to Do

Update PiecesOS to 12.4.0 or later before Friday, June 5th 2026. This is the only required action.

### Recommended: Update from the Pieces Tray Icon

On all operating systems, the easiest way to update is directly from the Pieces icon in your system tray / toolbar. Click the Pieces icon, and PiecesOS will check for updates automatically — if a new version is available, you can install it from there.

### Alternative: Update from Inside the Desktop App

You can also trigger the update from within the Pieces Desktop App by opening the user menu in the top-left and selecting `Check for Updates`.

### Other Install Methods

* **Homebrew (macOS/Linux)**: `brew upgrade pieces-os`
* **Manual installs**: follow the [manual installation guide](/products/core-dependencies/pieces-os/manual-installation)

After updating, restart PiecesOS and verify your version is 12.4.0 or higher.

## Why We Are Making This Change

Older PiecesOS versions were built against legacy cloud infrastructure that we are retiring in favor of our new agentic engine and updated backend. Maintaining backward compatibility with the old infrastructure was holding back security, reliability, and the ability to ship improvements to Chat and the broader product.

## Need Help?

If you run into trouble updating, or if updating doesn't resolve your issue:

* Open a new issue in this repository with your PiecesOS version, OS, and a description of what you're seeing
* Or email us directly at [support@pieces.app](mailto:support@pieces.app)
* Or book a quick [support call](https://calendar.google.com/calendar/u/0/appointments/schedules/AcZssZ3bJHPPSJJHom2WwsPf5KcNlu-vRZsVa3DO1gJ7q4VIwExD1NUFBXlc7w8JGnEoSd2TLxP3eFbh)

Thanks for being part of the Pieces community.
