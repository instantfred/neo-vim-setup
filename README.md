# neo-vim-setup

## Install NeoVIm
Homebrew on macOS or Linux
```bash
brew install neovim
````

Place this repo's nvim folder in `~/.config`

## Packer
I'm using [packer](https://github.com/wbthomason/packer.nvim)https://github.com/wbthomason/packer.nvim to handle packages installs, but it's been deprecated so I suggest going over [lazy.nvim](https://github.com/folke/lazy.nvim)https://github.com/folke/lazy.nvim

Plugin placement is done in `nvim/lua/<your-name>/plugins-setup.lua` by adding the `use` command plus a repo's path.
````bash
 use("wbthomason/packer.nvim")
````
Once a plugin is added, run the packer installer `PackerInstall`. A new window should pop-up letting you know what's been installed. 

### Mason
Once the plugins are installed, run `Mason` to select which linters/formatters to use. 

## Fonts
I'm using Meslo from [Nerd Font](https://www.nerdfonts.com/)https://www.nerdfonts.com/ which I uploaded in this repo. We just need to install them in order for all the fancy icons to be displayed correctly in our terminal. It's not really needed, but it makes working on the terminal nicer. 
 - **iTerm2**: open iTerm2 → Preferences → Profiles → Text and set Font to MesloLGS NF.

## Preview
![Screenshot 2023-12-12 at 10 13 23](https://github.com/instantfred/neo-vim-setup/assets/5740705/4d018e44-335d-4b90-a94d-717ab0a17512)
