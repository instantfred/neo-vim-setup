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

## Fonts
I'm using Meslo from [Nerd Font](https://www.nerdfonts.com/) which I uploaded in this repo. Install them for all the fancy icons to display correctly in your terminal. It's not strictly needed, but it makes working in the terminal nicer.
 - **iTerm2**: open iTerm2 → Preferences → Profiles → Text and set Font to MesloLGS NF.

## Preview
![Screenshot 2023-12-12 at 10 13 23](https://github.com/instantfred/neo-vim-setup/assets/5740705/4d018e44-335d-4b90-a94d-717ab0a17512)
