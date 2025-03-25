# Terminal Setup Instructions

This document outlines the steps required to set up my terminal environment.

## Ghostty Setup

To install Ghostty using Homebrew, run the following command:

```bash
brew install --cask ghostty
```

Setup theme

```bash
mkdir -p ~/.config/ghostty/themes
```
Create and enter a temporary directory for cloning
```bash
mkdir -p ~/foo && cd ~/foo
```
Clone the Ghostty Noctis Themes repository
```bash
git clone https://github.com/EastSun5566/ghostty-noctis-themes.git
```
Copy the themes to your Ghostty configuration directory
```bash
cp ghostty-noctis-themes/themes/* ~/.config/ghostty/themes/
```
Clean up by deleting the temporary directory
```bash
cd .. && rm -rf ~/foo
```

## Starship Setup
```bash
brew install starship
```
Open your zsh configuration file
```bash
vim ~/.zshrc
```
Add the following line to your ~/.zshrc file:
```bash
eval "$(starship init zsh)"
```
Apply the changes:
```bash
source ~/.zshrc
```

Create and enter a temporary directory for cloning
```bash
mkdir -p ~/foo && cd ~/foo
```
Clone Configs repository
```bash
git clone https://github.com/gorlovq/configs.git
```
Overwrite the existing Starship configuration
```bash
cp -f configs/starship.toml ~/.config/starship.toml
```
Apply the changes
```bash
source ~/.zshrc
```
Clean up by deleting the temporary directory
```bash
cd .. && rm -rf ~/foo
```
