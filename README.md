# neo-vim-setup

## Install NeoVim
Homebrew on macOS or Linux
```bash
brew install neovim
```

Place this repo's `nvim` folder in `~/.config`

## Plugin Manager: lazy.nvim
This setup uses [lazy.nvim](https://github.com/folke/lazy.nvim) for plugin management.

Plugin configuration is handled in [`nvim/lua/fred/lazy.lua`](nvim/lua/fred/lazy.lua). Plugins are organized in the [`nvim/lua/fred/plugins/`](nvim/lua/fred/plugins/) directory.

After cloning the repo and opening Neovim, `lazy.nvim` will automatically install itself and all configured plugins.

### Mason
Once the plugins are installed, run `:Mason` in Neovim to select which linters/formatters to use.

## Keybindings and Commands

The leader key is set to `space`. For example, `<leader>e` means pressing `space` then `e`.

> **Note**: The keybindings listed here are based on a common setup. You can find the specific configurations in `nvim/lua/fred/keymaps.lua` and your LSP plugin file.

### General & Window Management

| Key | Description |
|---|---|
| `<C-h>` | Navigate to the window on the left |
| `<C-j>` | Navigate to the window below |
| `<C-k>` | Navigate to the window above |
| `<C-l>` | Navigate to the window on the right |
| `<leader>nh` | Clear search highlights |
| `<leader>e` | Toggle the file explorer (`nvim-tree`) |

### Telescope (Fuzzy Finder)

| Key | Description |
|---|---|
| `<leader>ff` | Find files in the project |
| `<leader>fg` | Search for a string in the project (Live Grep) |
| `<leader>fb` | Find and switch between open buffers |
| `<leader>fh` | Search help tags |

### LSP (Language Server Protocol)

These keybindings are active in buffers with an attached LSP server.

| Key | Description |
|---|---|
| `gd` | Go to definition |
| `K` | Show hover documentation |
| `gi` | Go to implementation |
| `gr` | Show references |
| `<leader>rn` | Rename symbol |
| `<leader>ca` | Show code actions |
| `[d` | Go to the previous diagnostic |
| `]d` | Go to the next diagnostic |
| `<leader>dl` | Show line diagnostics in a floating window |

### Useful Commands

| Command | Description |
|---|---|
| `:Lazy` | Open the lazy.nvim interface to manage plugins. |
| `:Mason` | Open the Mason interface to manage LSPs, formatters, etc. |
| `:LspInfo` | Show information about active LSP clients. |

## Fonts
I'm using Meslo from Nerd Font which I uploaded in this repo. Install them for all the fancy icons to display correctly in your terminal. It's not strictly needed, but it makes working in the terminal nicer.
 - **iTerm2**: open iTerm2 → Preferences → Profiles → Text and set Font to MesloLGS NF.

## Preview
![Screenshot 2023-12-12 at 10 13 23](https://github.com/instantfred/neo-vim-setup/assets/5740705/4d018e44-335d-4b90-a94d-717ab0a17512)
