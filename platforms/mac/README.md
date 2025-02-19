# macOS Setup

First, follow the [WSL Setup Guide](../linux/README.md).

## GUI Applications

Use Homebrew to install the necessary applications:

```sh
brew install visual-studio-code raycast hammerspoon google-chrome ghostty
brew install --cask docker
```

### Link Configuration Files

Link the configuration files for Hammerspoon and Ghostty:

```sh
stow ghostty
stow hammerspoon
```
