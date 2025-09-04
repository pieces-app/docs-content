---
title: Issues | Linux
path: /desktop/troubleshooting/linux
visibility: PUBLIC
status: PUBLISHED
description: Find out what troubleshooting steps to take if the Pieces Desktop App isn't working properly on your Linux device.
metaTitle: Troubleshooting Issues on Linux | Pieces Desktop App
metaDescription: Learn about what troubleshooting steps to take if the Pieces Desktop App isn’t working as expected on your Linux device.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/desktop/troubleshooting_linux.png"
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/linux/troubleshooting_linux.png" alt="" align="center" fullwidth="true" />

## Installation & Updating Fixes

You can find detailed instructions on how to update PiecesOS and the Pieces Desktop App on your Linux device using the terminal.

Additionally, you can check your system's OS and hardware specifications to ensure they meet the minimum recommended requirements.

<on-device-storage />

## Versions & Updates

Many issues can stem from running outdated versions of the Pieces Desktop App on Linux.

### Updating Pieces Desktop

On Linux, the Pieces Desktop App is distributed via snaps (for Ubuntu-based systems).

To update the Pieces Desktop App on Linux:

<Steps>
  <Step title="Check the Current Version">
    Running `snap info pieces-for-developers` to check the current version
  </Step>

  <Step title="Check for Updates">
    Running `sudo snap refresh` to apply any available updates

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/linux/snap_refresh_PFD.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

## Common Installation Issues

Official support is for **Ubuntu 22.04+ and Ubuntu-based distributions.** Other distributions might work, but *aren’t guaranteed.*

## Checking Distribution Compatibility

Ensure you’re running a supported **Ubuntu-based distribution.**

If not, consider switching to a supported environment, as installation on non-Ubuntu distributions isn’t guaranteed.

### Updating Snapd

Snap-based installations require an up-to-date snap `daemon`:

* Run `sudo snap refresh` to ensure `snapd` and its packages are current

### Adjusting Graphics & Display Settings

If installation or UI issues persist, consider the following:

* **Switch Between X11 and Wayland:** Some applications may work better on one display protocol than the other. Try switching to X11 for compatibility or Wayland for newer features. You can usually select this at the login screen.

<Callout type="alert">
  The LTM-2.7 Engine is designed to work with the X11 Window Manager. Other Window Managers, such as Wayland, are *not compatible.* This means that long-term memory functionality with certain Linux Virtual Machines (VMs) is not possible at this time.
</Callout>

* **Update your GPU Drivers:** Ensure they are up to date. For NVIDIA, check for proprietary driver updates. AMD and Intel users should verify that their open-source drivers are up to date.

* **Optimize Graphics Configurations:** Use tools like `nvidia-settings`, `radeon-profile`, or similar utilities to adjust your GPU settings for better performance and stability.

These adjustments can resolve many graphical and display-related issues you may experience while using Pieces.

## Checking System Information

Verify your system's hardware configuration and ensure it meets the recommended specifications by running specific commands in your terminal.

### Checking CPU Information

To determine your CPU type and find other important information, type `lscpu` in your terminal and press `Enter`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/linux/lscpu_UBUNTU.png" alt="" align="center" fullwidth="true" />

### Checking GPU Information

To determine your GPU type and find other important information, `lspci | grep -i vga` in your terminal and press `Enter`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/linux/lscpi_UBUNTU.png" alt="" align="center" fullwidth="true" />

Confirm that your CPU, GPU, and memory resources are sufficient for running PiecesOS and local AI models, if applicable.

### Checking Ubuntu Version

If the Pieces Installer is not working as intended, you could have an outdated version of Ubuntu. The minimum Ubuntu version that Pieces will run on is **Ubuntu 22.04 or later**.

To check what version of Ubuntu you’re running:

<Steps>
  <Step title="Open Settings">
    Open the **Settings** on Ubuntu by clicking the *options bar* in the top right
  </Step>

  <Step title="Find the System Section">
    Locate the **System** section at the bottom of the left-hand side menu and click it
  </Step>

  <Step title="Open the About Section">
    Open the **About** section and locate the **Operating System** label
  </Step>
</Steps>

This section will display your Ubuntu version information.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/linux/settings_about_system.gif" alt="" align="center" fullwidth="true" />

### Consulting Online Resources

If you encounter persistent installation issues, consult online forums or community guides related to snap and Ubuntu-specific troubleshooting steps.

## Restart & Retry

If you've updated components, checked the hardware, and adjusted configurations without success, try restarting your machine and then try again.

If the problem persists, please open a <a target="_blank" href="https://github.com/pieces-app/support/issues">**GitHub issue**</a> for further assistance or book a call with our engineers.