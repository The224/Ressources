# Terminal

Prettify every instance of a terminal

## Bash

Change your default terminal for ZSH

```bash
sudo apt install zsh
chsh -s $(which zsh)
# Logout/login and confirm
echo $SHELL
# Should be something like -> /bin/zsh
```

## ZSH

Use *Oh My Zsh* framework:

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

Then change the theme for

```zsh
# Clone the theme in themes folder
git clone https://github.com/denysdovhan/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt"
# Symlink to your oh-my-zsh custom themes directory
ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"
# Change the theme for ZSH_THEME="spaceship"
sudo vi .zshrc
# Logout/login
```
