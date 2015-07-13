## Installation

Clone from here: https://github.com/lengstrom/zsh-prompt-insert.git

Run the following commands on your command line:

```
#Make a folder (if you don't already have one) for your ZSH functions/widgets
mkdir ~/.zfunc

#Add `/path/to/zsh-prompt-insert/prompt_insert.sh"` to your ZSH function folder with a symlink
ln -s ~/.zfunc/prompt-insert /path/to/zsh-prompt-insert/prompt-insert.sh
```

Then, add the following two lines to your `~/.zshrc`:
```
`fpath=( /path/to/zsh-prompt-insert/prompt-insert "${fpath[@]}" )` #Put the folder in your $fpath
autoload -Uz prompt-insert #Mark `prompt-insert` to have zsh automatically load it

```
