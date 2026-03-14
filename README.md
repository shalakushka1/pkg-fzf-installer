# Package FZF Installer

A terminal-based tool designed to streamline package management and system maintenance on Arch Linux. It provides a clean, searchable interface for official repositories and the AUR while centralizing system cleanup and updates.

## ✨ Features

* **Dual Repository Support**: Separate modes for installing packages from official repositories and the AUR.
* **AUR Exclusive Search**: Uses `paru -Ssq -a` to ensure the AUR search only displays community-driven packages, avoiding duplicates from official repos.
* **Centralized Management**: A dedicated submenu for system updates, package removal, and cache cleanup.
* **Interactive Cleanup**: Safely remove orphan packages and clean caches with manual `[Y/n]` confirmation prompts to prevent accidental loss of optional dependencies.
* **Modern UI**: Integrated with `fzf` for fuzzy searching and `gum` for stylized loading spinners.

## 📦 Dependencies

The following packages are required for the script to function correctly:

| Package | Role | Installation |
| :--- | :--- | :--- |
| **fzf** | Interactive menu and search engine | `sudo pacman -S fzf` |
| **gum** | Styled spinners and feedback | `sudo pacman -S gum` |
| **paru** | AUR helper and update manager | `sudo pacman -S paru` |
| **bash** | Shell interpreter | Pre-installed |

## 🛠️ Installation

To install the script globally to `/usr/bin/`, follow these steps:

1.  **Clone or create the script file**:
    Save your script as `pkg-fzf-installer.sh`.

2.  **Make it executable**:
    ```bash
    chmod +x pkg-fzf-installer.sh
    ```

3.  **Move it to /usr/bin/**:
    ```bash
    sudo mv pkg-fzf-installer.sh /usr/bin/pkg-fzf-installer
    ```

4.  **Run it from anywhere**:
    Simply type:
    ```bash
    pkg-fzf-installer
    ```

## ⌨️ Navigation & Shortcuts

* **Arrows / Ctrl-j/k**: Navigate the list.
* **TAB**: Select multiple packages for bulk installation/removal.
* **ALT-P**: Show detailed package information in the preview window.
* **ALT-B**: Display the PKGBUILD (AUR mode only).
* **Enter**: Confirm the action.

## 📄 License

This project is licensed under the **GNU General Public License v3.0**.

See the [LICENSE](LICENSE) file for the full text.

---
