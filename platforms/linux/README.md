# WSL Setup

## Install Homebrew (Linuxbrew)

```shell
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Install Devtools

Use Homebrew to install the required terminal applications:

```bash
brew install zoxide eza fzf gh lazygit lazydocker mise starship tree cloc stow
brew install zsh-syntax-highlighting zsh-autosuggestions
```  

## Configuration

### Clone Dotfiles and Link

Clone this repository:

```bash
git clone https://github.com/wzhudev/dotfiles.git .dotfiles
```

Copy and link configuration files:

```bash  
cp ~/.dotfiles/config/git.gitconfig ~/.gitconfig  

stow tmux nvim mise vim starship

conda config --set changeps1 False
```  

### Update `.zshrc`

Add your custom `.zshrc` configuration by sourcing it:

```bash
echo "source ~/.dotfiles/zsh/.zshrc" >> ~/.zshrc
```

## Miscellaneous

If a proxy is required, use the following command to set it up:

```bash
export ALL_PROXY="http://127.0.0.1:7890"
export HTTPS_PROXY="http://127.0.0.1:7890"
export HTTP_PROXY="http://127.0.0.1:7890"
```
