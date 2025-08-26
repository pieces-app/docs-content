---
title: Troubleshooting
path: /extensions-plugins/untitled-pageasd/troubleshooting
visibility: PUBLIC
status: PUBLISHED
---

## Troubleshooting Pieces for Neovim

Here are links to support resources, documentation, and our Discord channel for troubleshooting related to the [Pieces for Neovim Extension](https://plugins.jetbrains.com/plugin/17328-pieces).

You can also find some specific troubleshooting steps for Neovim issues below.

## Setting you Pieces Runtime for Neovim

If you’re getting an issue with your Python Runtime environment, you may have to edit your `init.vim`:

<Steps>
  <Step title="Open init.vim">
    Within `init.vim` above the line `plug#begin('~/.vim/plugged')` enter the line:

    * `let g:python3_host_prog ='/path/to/your/python3.exe'`
  </Step>
</Steps>

## Issues Installing PlugInstaller on Windows

Installing `PlugInstaller` on Windows can cause some issues due to differences from native terminals. To quickly install `PlugInstaller` on Windows, enter the command:

```powershell
New-Item -ItemType Directory -Path "$env:LOCALAPPDATA\nvim-data\site\autoload" -Force; Invoke-WebRequest "https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim" -OutFile "$env:LOCALAPPDATA\nvim-data\site\autoload\plug.vim"
```

## Check Neovim Providers Health

A quick way to check if the Neovim provider health status is to follow the steps below:

<Steps>
  <Step title="Open Neovim">
    Open Neovim within a terminal with the command:

    * `nvim`
  </Step>

  <Step title="Enter Checkhealth Command">
    To enter a commend, press the `esc` key on your keyboard and then enter:

    * `:checkhealth provider`

    This will check the status of your providers and will indicate which providers aren’t enabled or working.

    **The only provider Pieces requires is Python.**
  </Step>
</Steps>

## Updating[​](/extensions-plugins/jetbrains#updating)

The Pieces for Neovim Extension will update with a simple command within Neovim:

* `:UpdateRemotePlugins`

You need to use this command within Neovim. You can do this in a simple `nvim` window and then exit.

### Check PiecesOS Status

You can check PiecesOS health with:

* `:PiecesHealth`

You can also check your PiecesOS version with the command:

* `:PiecesOSVersion`

Both of these will return a warning if PiecesOS isn’t running properly.

### Restart Neovim After Updates

After updating PiecesOS, exit Neovim and

## Reloading the Pieces Copilot Chat Window
