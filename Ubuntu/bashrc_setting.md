# set eternal history & history timestamp
``` bash
# Eternal bash history
# ---------------------
# https://stackoverflow.com/questions/9457233/unlimited-bash-history
export HISTSIZE= 
export HISTFILESIZE=
export HISTTIMEFORMAT="[%F %T] "
# Change the file location because certain bash sessions truncate .bash_history file upon close.
export HISTFILE=~/.bash_eternal_history
# Force Prompt to write history after every command.
PROMPT_COMMAND="history -a; $PROMPT_COMMAND"
```
# set bash to show git branch 
``` bash
export PS1='${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[93m\]$(__git_ps1)\[\033[00m\]\$ '
```
