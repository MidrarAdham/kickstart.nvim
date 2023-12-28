# kickstart.nvim

https://github.com/kdheepak/kickstart.nvim/assets/1813121/f3ff9a2b-c31f-44df-a4fa-8a0d7b17cf7b

### Introduction

This repo is meant to be used by **YOU** to begin your Neovim journey; remove the things you don't use and add what you miss.

Kickstart.nvim targets *only* the latest ['stable'](https://github.com/neovim/neovim/releases/tag/stable) and latest ['nightly'](https://github.com/neovim/neovim/releases/tag/nightly) of Neovim. If you are experiencing issues, please make sure you have the latest versions.

## Source:

Refer to where this repository is forked from for better instructions.

## Important Information for Python Users:

To get Autocomplete working for your python distribution, follow the instructions below.

- Open nvim and execute ":Mason".
- Search for "python-lsp-server"
- If not installed, type "I" to install it.
- Once installed, quit nvim.
- In your Terminal, change directory to ".local/share/nvim/mason/packages/python-lsp-server/venv/"
- Open "pyvenv.cfg" and change "include-system-site-packages" to true
- Save and exit


Editing a Python script using nvim gives a lot of warnings. The only way I managed to silence some of these errors is by adjusting the pylsp.lua file.
The pylsp.lua is located in .local/share/nvim/lazy/nvim-lspconfig/lua/lspconfig/server_configurations. To revert the file to its default state, comment
out the lua block (lines 31-43)
