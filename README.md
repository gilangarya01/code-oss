# 🧩 Code - OSS Configuration

This directory contains my personal configuration for **[Code - OSS](https://github.com/microsoft/vscode)** (the open-source build of Visual Studio Code), managed as part of my dotfiles using [GNU Stow](https://www.gnu.org/software/stow/).

## 🛠 Requirements

Make sure you have `stow` installed on your system:

```bash
sudo pacman -S stow      # Arch-based
# or
sudo apt install stow    # Debian/Ubuntu
```

Also ensure that Code - OSS is installed:

```bash
# Arch
sudo pacman -S code

# Or using flatpak
flatpak install flathub com.vscodium.codium
```

## 🚀 Installation

Clone this dotfiles repository:

```bash
git clone https://github.com/gilangarya01/code-oss.git ~/dotfiles/code-oss
cd ~/dotfiles
```

Then use `stow` to symlink the configuration into place:

```bash
stow code-oss
```

This will link `settings.json` and `keybindings.json` to the appropriate directory:

- `~/.config/Code - OSS/User/` (for most Linux setups)

If you're using **VSCodium**, the path might instead be:

- `~/.config/VSCodium/User/`

You can adjust the symlink target if needed.

## 🧪 What's Inside

- `settings.json`: Custom settings for appearance, performance, font, etc.
- `keybindings.json`: Keyboard shortcut customizations for a more efficient workflow.
- `extensions/`: Directory for manually managed Code-OSS extensions.
