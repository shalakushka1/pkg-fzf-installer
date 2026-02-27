# pkg-fzf-installer

A minimalist, high-performance package manager interface for Arch Linux using `fzf`.

## 🚀 Features
- **Unified Interface**: Manage both Official (Pacman) and AUR (paru) packages in one place.
- **Dynamic Search**: Prevents binary dumps and terminal freezes by searching on-type for AUR packages.
- **Rich Previews**: View package info and PKGBUILDs directly in the terminal.
- **Shell Independent**: Specifically configured to avoid `zsh` subshell fork errors.

## 🛠 Dependencies
- `fzf`
- `paru` (AUR helper)
- `gum` (Optional, for UI spinners)
- `pacman`

## 📦 Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/shalakushka1/pkg-fzf-installer.git
