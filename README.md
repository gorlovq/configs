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
