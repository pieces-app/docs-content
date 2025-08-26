---
title: Download | Pieces for Developers
path: /desktop/download
visibility: PUBLIC
status: PUBLISHED
description: Find download links for the Pieces Desktop App and links to OS-specific and method-specific installation guides.
metaTitle: Download Pieces
metaDescription: Download the Pieces Desktop Application for AI-powered workflow assistance, code management, and enhanced developer productivity.
---

## Installing the Pieces Desktop App

Installation for the Pieces Desktop App and its core dependencies—[PiecesOS](/products/core-dependencies/pieces-os) and [Ollama](/products/core-dependencies/ollama)—is straightforward.

Select the appropriate download file for your platform (macOS/Windows) or follow the CLI installation instructions for Linux.

<Callout type="info">
  macOS users will be prompted to select the proper download file based on their device’s architecture—ARM or Intel.
</Callout>

## Downloads

Find the download files for the Pieces Desktop App for your macOS or Windows device below.

### macOS

If you know your macOS device’s CPU architecture, you can select either the ARM or Intel buttons to download the Pieces Desktop App using the *recommended* installation method.

Read this [guide on determining your CPU architecture](/products/desktop/troubleshooting/macos#checking-cpu-type) if you need help.

For detailed instructions, refer to our comprehensive [macOS installation and quick-start guide.](/products/meet-pieces/macos-installation-guide)

<CardGroup cols={2}>
  <Card title="Apple Silicon / ARM" image="https://cdn.hashnode.com/res/hashnode/image/upload/v1740593663020/d271a302-cec3-466c-9d9d-085f762d95bc.png" href="https://builds.pieces.app/stages/production/macos_packaging/pkg-arm64/download?download=true&product=DOCUMENTATION_WEBSITE&ga_visitor=286281413.1724689222&_gl=1*soqacc*_gcl_au*MTgwNDcwNzY1OC4xNzQwNDA5MjEz*_ga*Mjg2MjgxNDEzLjE3MjQ2ODkyMjI.*_ga_BVYEFRWCYX*MTc0MDU3NzUzMS42My4xLjE3NDA1OTM3MjEuNTIuMC4w">
    *macOS 12.0 (Monterey) or higher*
  </Card>

  <Card title="Intel" image="https://cdn.hashnode.com/res/hashnode/image/upload/v1740593657157/c79ed786-39f3-4fca-a596-451ce98307b1.png" href="https://builds.pieces.app/stages/production/macos_packaging/pkg/download?download=true&product=DOCUMENTATION_WEBSITE&ga_visitor=108380292.1740593596&_gl=1*1vo6txu*_gcl_au*MTE0NTE1OTUyLjE3NDA1OTM1OTY.*_ga*MTA4MzgwMjkyLjE3NDA1OTM1OTY.*_ga_BVYEFRWCYX*MTc0MDU5MzU5NS4xLjEuMTc0MDU5MzYxMS40NC4wLjA.">
    *macOS 12.0 (Monterey) or higher*
  </Card>
</CardGroup>

Otherwise, you can download Pieces software using [alternative installation methods](/products/meet-pieces/macos-installation-guide) (.DMG, Homebrew).

### Windows

Click the download button to install the Pieces Desktop App using the *Recommended* (`.appinstaller`) installation method.

For detailed instructions, refer to our comprehensive [Windows installation and quick-start guide.](/products/meet-pieces/windows-installation-guide)

<Card title="Windows" image="https://cdn.hashnode.com/res/hashnode/image/upload/v1740593810761/7014560e-d011-438c-aa0d-1509abcf313d.png" href="https://builds.pieces.app/stages/production/appinstaller/pieces_for_x.appinstaller?_gl=1*o2haep*_gcl_au*MTA2NTQ0NTg3OC4xNzM4NjI2MzMx*_ga*MTkzMTk3NjkzNy4xNzM4NjI2MzMx*_ga_BVYEFRWCYX*MTc0NjIwNTI5OS45LjEuMTc0NjIxMzY2MC41NC4wLjA.">
  *Windows 10 (1809) or higher*
</Card>

If you want alternative installation methods (`.exe`, WinGet), [click here.](/products/desktop/troubleshooting/windows#alternative-installation-methods)

### Linux

Installation of Pieces software is done using the Command-Line Interface (CLI).

For a step-by-step terminal process using the CLI, refer to our [comprehensive Linux installation and quick-start guide.](/products/meet-pieces/linux-installation-guide)

<Card title="Download — Linux" image="https://cdn.hashnode.com/res/hashnode/image/upload/v1741278390901/a6fcd0e6-4c6a-47e8-93ac-01981b74f8b6.webp">
  *Ubuntu 22+ required.*

  ***

  Run these commands **in order** to install and properly set up PiecesOS.

  1. **Open Terminal:** Open the Command-Line Interface (CLI) using `ctrl+alt+t`.

  2. Run `sudo snap install pieces-os` to install PiecesOS. You will be prompted to enter your local account’s password.

  3. Enter and run `sudo snap connect pieces-os:process-control :process-control` to enable offline and on-device machine learning and LLM functionality.

  4. Then, type `sudo snap install pieces-for-developers` to download the Pieces Desktop App.

  5. Type `pieces-for-developers` to launch the application directly from your terminal.
</Card>