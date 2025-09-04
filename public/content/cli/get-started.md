---
title: Get Started
path: /cli/get-started
visibility: PUBLIC
status: PUBLISHED
description: The Pieces CLI is a flexible command-line interface for Pieces that integrates smoothly with your development environment.
metaTitle: Get Started with Pieces CLI
metaDescription: Get Started with Pieces CLI, a flexible command-line interface for Pieces.
---

<pieces-pro-cta />

## Pieces CLI Prerequisites

Before installation, you’ll need:

* **PiecesOS:** The power engine behind the Pieces CLI and the rest of the Pieces Suite. [Learn more about PiecesOS](/products/core-dependencies/pieces-os).

* **Python 3.xx:** <a target="_blank" href="https://www.python.org/downloads/">Python</a> is required to be installed on your development machine.

<Callout type="alert">
  PiecesOS must be installed to use the Pieces CLI and ensure it works properly. 

  We also suggest using the Pieces for Developers Desktop App for better functionality.
</Callout>

### Sign in Required

Pieces requires all users to sign in before using any plugins or extensions. You'll be prompted to authenticate if you haven't already. For help, see our [sign-in guide](/products/meet-pieces/sign-into-pieces).

## Installing the Pieces CLI

Follow the instructions below to install the Pieces CLI and any required dependencies.

<Steps>
  <Step title="Install Python">
    Head to [Python’s website](https://www.python.org/downloads/) and download the version that best suits your environment.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/get_started/python_download.png" alt="" align="center" fullwidth="true" />

    After downloading the Python version 3.xx, you will be guided through the installation process. Follow their steps until Python is installed.

    <Callout type="tip">
      Make sure to allow Python to be added to your environment variables, so it’s executable via terminal.
    </Callout>
  </Step>

  <Step title="Install Pieces CLI">
    Once Python is installed, its dependency `pip` is automatically installed. Choose your OS:

    <Tabs>
      <Tab label="Windows">
        Install the Pieces CLI on Windows using Python’s launcher:

        ```bash
        py -m pip install pieces-cli
        ```
      </Tab>
      <Tab label="macOS">
        Install with Homebrew on macOS:

        ```bash
        brew install pieces-cli
        ```
      </Tab>
      <Tab label="Linux">
        Install with pip3 on Linux:

        ```bash
        pip3 install pieces-cli
        ```
      </Tab>
    </Tabs>
  </Step>

  <Step title="Verify Installation">
    To verify a successful installation of the Pieces CLI, you can type `pieces version` within your terminal. This will display your Pieces OS and Pieces CLI versions.

    <Callout type="alert">
      If you receive **'pieces' is not recognized as an internal or external command,** you can run pieces with `py -m pieces $command`.
    </Callout>
  </Step>

  <Step title="Run Pieces CLI">
    To run Pieces CLI, you can enter the command `pieces run`. This will launch you into the Pieces CLI and make it so you don’t have to prefix with `pieces`.
  </Step>
</Steps>

### Setting Up PiecesOS

To use the Pieces CLI, you must install [PiecesOS](/products/core-dependencies/pieces-os) on your working environment.

Click the download buttons or follow the set-up instructions below for your operating system:

<get-started-install />

<Callout type="alert">
  For enhanced security and better system integration, we recommend installing the `.appinstaller` package over the `.exe` installer. The `.appinstaller` package operates in a containerized environment, providing additional security benefits.
</Callout>

## Updating

Follow the steps below to update the Pieces CLI.

<Steps>
  <Step title="Open a Terminal">
    Opening a terminal on your device depends on your platform: Open your OS’ search bar and enter `terminal` (macOS/Linux) or `CMD` (Windows).
  </Step>

  <Step title="Update Pieces CLI">
    Choose your OS:

    <Tabs>
      <Tab label="Windows">
        Update to the latest Pieces CLI on Windows:

        ```bash
        py -m pip install pieces-cli -U
        ```
      </Tab>
      <Tab label="macOS">
        Upgrade with Homebrew on macOS:

        ```bash
        brew upgrade pieces-cli
        ```
      </Tab>
      <Tab label="Linux">
        Update with pip3 on Linux:

        ```bash
        pip3 install pieces-cli -U
        ```
      </Tab>
    </Tabs>

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/get_started/update_pieces_cli.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

## Onboarding

The Pieces CLI offers a walkthrough to guide you through the steps of saving your first material and introduces you to the Long-Term Memory Engine (LTM-2.7), enabling you to make the most of the Pieces CLI.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/get_started/onboarding_first_step.png" alt="" align="center" fullwidth="true" />

### Save Your First Material

The onboarding will start by providing you with a snippet to copy to your clipboard. Highlight the code and press `⌘+c` (macOS) or `ctrl+c` (Windows/Linux).

After copying the snippet, you can select any key on your keyboard to proceed.

<Callout type="info">
  If you haven’t copied the snippet, Pieces won’t allow you to paste.
</Callout>

After pressing any key, Pieces will prompt you to type `pieces create` into your terminal. With the snippet still copied, enter `pieces create`, and Pieces will ask if you want to save the snippet.

Type `y` and press `return`(macOS) or `enter`(Windows/Linux) to confirm to save the snippet to your [Pieces Drive](/products/cli/drive).

### Finding your Saved Materials

In this step, you'll learn how to open your saved materials. Start by typing `pieces list` in your terminal and pressing `enter`.

This will display a list of all your saved materials. You can navigate through them using the arrow keys on your keyboard.

Select the material you're highlighting by pressing `return`(macOS) or `enter`(Windows/Linux).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/get_started/selecting_pieces_list_onboarding.gif" alt="" align="center" fullwidth="true" />

### Start a Session

After selecting a snippet, Pieces CLI will boot you out to the terminal to prompt you to start a new session.

Typing `pieces run` will open a new session, allowing you to enter Pieces commands without prefixing with `pieces`.

After the session, you can type exit and press `return`(macOS) or `enter`(Windows/Linux) to return to the onboarding.

### Chat with the Copilot

This section will walk you through how to ask [Pieces Copilot](/products/cli/copilot) its first question. You can begin in your terminal by typing `pieces ask 'How to print I love Pieces CLI in Python and Java'` and pressing `return`(macOS) or `enter`(Windows/Linux).

After typing your question and running the command, Pieces Copilot will quickly generate and display the best response for your query.

It will then prompt you to do it with the Pieces CLI running by typing `pieces run` entering the command and then entering `ask $question`, `$question` being the question you’d like to ask Pieces Copilot.

<Callout type="info">
  Your question must be encased in quotations or Pieces won’t capture your full question.
</Callout>

### More Resources

Your feedback is **vital** to us. This onboarding step will prompt you to enter `pieces feedback` where you can optionally open the GitHub discussion board related to Pieces CLI to leave helpful feedback.

If you enter `y` it will open the GitHub discussion board in a new tab in your browser, otherwise it will skip this step.

After completing the <a target="_blank" href="https://github.com/pieces-app/cli-agent/discussions/194">feedback</a>, Pieces will prompt you to type `pieces contribute` and then ask if you’d like to open the <a target="_blank" href="https://github.com/pieces-app/cli-agent">source code for Pieces CLI on GitHub</a> to improve it. You can optionally say yes by entering `y`; otherwise, enter `n`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/get_started/pieces_feedback_onboarding.png" alt="" align="center" fullwidth="true" />

## Uninstalling

Follow the steps below to uninstall the Pieces CLI.

If you also want to uninstall PiecesOS, [follow these steps](/products/core-dependencies/pieces-os/manual-installation#uninstalling-piecesos).

<Steps>
  <Step title="Open a Terminal">
    Opening a terminal on your device depends on your platform: Open your OS’ search bar and enter `terminal`(macOS/Linux) or `CMD`(Windows).
  </Step>

  <Step title="Run Uninstall Command">
    Choose your OS:

    <Tabs>
      <Tab label="Windows">
        Uninstall on Windows:

        ```bash
        py -m pip uninstall pieces-cli
        ```
      </Tab>
      <Tab label="macOS">
        Uninstall with Homebrew on macOS:

        ```bash
        brew uninstall pieces-cli
        ```
      </Tab>
      <Tab label="Linux">
        Uninstall with pip3 on Linux:

        ```bash
        pip3 uninstall pieces-cli
        ```
      </Tab>
    </Tabs>

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cli_assets/get_started/pip_uninstall.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>
