## Steps

1. Install Apple's Command Line Tools, which are prerequisites for Git and Homebrew.

```sh
xcode-select --install;
git clone https://github.com/oozygrub/.dotfiles;
ln -s ~/.dotfiles/.zshrc ~/.zshrc;
ln -s ~/.dotfiles/.gitconfig ~/.gitconfig;
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)";
brew bundle --file ~/.dotfiles/Brewfile
```

2. Install Oh My Zsh

```sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)";
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting;
git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-completions;
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions;
```

## Source

- https://github.com/eieioxyz/Beyond-Dotfiles-in-100-Seconds
- https://github.com/sindresorhus/github-markdown-css/blob/main/github-markdown.css
