# My Dotfiles

Welcome to my dotfiles repository, managed with GNU Stow.

## What are Dotfiles & Why Stow?

Dotfiles are hidden configuration files (e.g., `.zshrc`) that customize your system. Managing them with gnu stow allows for easy synchronization across machines and a clean home directory by creating symbolic links from this repo to your home.

## Getting Started

### Prerequisites

Ensure `stow` is installed:

* **macOS (Homebrew):** `brew install stow`

* **Debian/Ubuntu:** `sudo apt install stow`

### Installation

1. **Clone:**

```
git clone https://github.com/camdenwithrow/dotfiles.git ~/dotfiles
```

2. **Navigate:**

```
cd ~/dotfiles
```

3. **Run Stow:**
Either stow each config package individual:
```
stow $PACKAGE_NAME
```
Or, install all packages:
```
chmod +x ./install
./install
```

This links all top-level directories (e.g., `.config`, `.zshrc`) to your home directory.

**Note:** Back up or remove conflicting existing dotfiles before running `stow .`.
