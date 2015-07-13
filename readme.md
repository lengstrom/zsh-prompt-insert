## Installation

Clone from here: https://github.com/lengstrom/zsh-prompt-insert.git

Run the following commands on your command line:

```
#Make a folder (if you don't already have one) for your ZSH functions/widgets
mkdir ~/.zfunc

#Symlink /path/to/zsh-prompt-insert/prompt_insert.sh into your function folder 
ln -s /path/to/zsh-prompt-insert/prompt-insert.sh ~/.zfunc/prompt-insert
```

Then, add the following lines to your `~/.zshrc`:
```
#Put the folder in your $fpath
fpath=( ~/.zfunc "${fpath[@]}" )

#Mark prompt-insert to have zsh automatically load it
autoload -Uz prompt-insert

#Set prompt-insert to a hotkey
bindkey ^i prompt-insert
```