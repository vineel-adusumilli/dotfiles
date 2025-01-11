# Dotfiles

The dotfiles are set up using `stow`. Make sure to check out to `~/dotfiles`. To apply, run `stow` for the appropriate subdirectory.

```
stow tmux
stow nvim
```

# Zsh setup

Make sure the submodules for this directory are checked out so that `powerelevel10k` is loaded:

```
$ git submodule init
$ git submodule update
```

First install oh-my-zsh:

```
$ sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Then install fzf:

```
$ brew install fzf
```

Now delete the default `.zshrc` file:
```
$ rm ~/.zshrc
```

Finally, stow things from zsh:

```
$ stow zsh
```

# Appearance

## InconsolataGo Nerd Font

Download (InconsolataGo Nerd Font Complete)[https://github.com/ryanoasis/nerd-fonts/blob/v2.3.3/patched-fonts/InconsolataGo/Regular/complete/InconsolataGo%20Nerd%20Font%20Complete.ttf]. Then move it into `~/Library/Fonts`.

## iTerm2 Solarized Dark Theme

Download [Solarized Dark theme](https://raw.githubusercontent.com/mbadolato/iTerm2-Color-Schemes/master/schemes/Solarized%20Dark%20-%20Patched.itermcolors) from [this Gist](https://gist.github.com/kevin-smets/8568070). Then simply `open Solarized\ Dark\ -\ Patched.itermcolors` and iTerm2 will install it.
