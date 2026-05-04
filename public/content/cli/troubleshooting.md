---
title: Troubleshooting
path: /cli/troubleshooting
visibility: PUBLIC
status: PUBLISHED
---

***

## Troubleshooting the Pieces CLI

Most CLI issues clear up after updating to the latest version, restarting PiecesOS, or restarting your shell. If those don't help, find your symptom in *Common Issues* below.

## Update Pieces CLI

The first thing to try for any unexpected behavior. An outdated CLI is the single most common cause of broken commands and integration errors.

<Callout type="alert">
  Before updating, close any running instance of the Pieces Desktop App and PiecesOS. On Windows, run your terminal as administrator (right-click `Command Prompt` or `PowerShell` → `Run as administrator`).
</Callout>

<Tabs>
  <TabItem title="PIP">
    ```bash
    pip install pieces-cli -U
    ```
  </TabItem>

  <TabItem title="Conda">
    ```bash
    conda update pieces-cli
    ```
  </TabItem>

  <TabItem title="Homebrew">
    ```bash
    brew upgrade pieces-cli
    ```
  </TabItem>
</Tabs>

PiecesOS may also need updating—if updating the CLI alone doesn't help, [reinstall PiecesOS](/products/core-dependencies/pieces-os/manual-installation#manual-download--installation) and restart your system so any new environment variables take effect.

## Common Issues

Find your symptom below for the recommended fix.

<AccordionGroup>
  <Accordion title="`pieces` command not found">
    Your shell can't locate the `pieces` binary on your `PATH`.

    - Confirm the CLI is installed: `pip install pieces-cli` (or your package manager of choice—see *Update Pieces CLI* above).
    - Restart your shell so any new `PATH` entries take effect. On macOS/Linux you can also run `source ~/.zshrc` or `source ~/.bashrc`.
    - If you installed with `pip install --user`, make sure your Python user-scripts directory is on your `PATH`.
    - On Windows, close and reopen `Command Prompt` or `PowerShell` after install so it picks up the new `PATH`.
  </Accordion>

  <Accordion title="PiecesOS isn't running">
    The CLI needs PiecesOS running in the background to serve your Pieces Drive and *Conversational Search* requests.

    - Start it with `pieces open`, or launch the Pieces Desktop App or applet manually.
    - Confirm it's running: `pieces version` should return a PiecesOS version alongside the CLI version.
    - If PiecesOS won't start at all, [reinstall it](/products/core-dependencies/pieces-os/manual-installation#manual-download--installation).
  </Accordion>

  <Accordion title="Conversational Search hangs or times out">
    Common when you're using a cloud LLM and your network drops—the model can appear to generate forever, loop, or eventually time out.

    - Force-quit the active chat with `⌘+C` (macOS) or `Ctrl+C` (Windows/Linux), then re-issue your `pieces ask "..."` command.
    - Switch to a different model with `pieces list models`. If one provider is degraded, another usually still works.
    - Confirm you're online and that your firewall or VPN isn't blocking the CLI's outbound HTTPS traffic.
  </Accordion>

  <Accordion title="Errors right after an update">
    Upgrades sometimes need the system to settle before everything lines up.

    - Restart your terminal—and your computer if you also updated PiecesOS.
    - Run `pieces version` and confirm the CLI and PiecesOS versions are both current. If one lags, update the lagging side.
    - If errors persist, [reinstall PiecesOS](/products/core-dependencies/pieces-os/manual-installation#manual-download--installation).
  </Accordion>

  <Accordion title="Permission denied during install or update">
    Your user doesn't have permission to write to the install location.

    - On Windows, run your terminal as administrator and retry the update command.
    - On macOS/Linux, prefer a user-scoped install with `pip install --user pieces-cli`. Avoid `sudo pip install`—it can leave your system Python in a broken state.
    - With Conda, run `conda update pieces-cli` from the same environment where you originally installed it.
  </Accordion>
</AccordionGroup>

***

## Still Stuck?

If none of the above resolves your issue, reach out and we'll help.

- File a <a target="_blank" href="https://github.com/pieces-app/support/issues">GitHub issue</a> with your CLI version (`pieces version`), OS, and a description of the problem.
- Or <a target="_blank" href="https://getpieces.typeform.com/to/mCjBSIjF#docs-vscode">contact the Pieces support team</a> directly.
