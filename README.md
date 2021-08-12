Configure iTerm2 to have github branch and kubrctl namespace in prompt
1. locally all my settings are in /Users/atse/.bash_profile file
2. add following lines to this file, will add github branch and a hamburger icon to the prompt

export PS1="🍔 \[\033[01;35m\]\u@\h:\[\033[01;34m\]\$(parse_git_branch) \[\033[01;32m\]\w \[\033[01;34m\]\[\e[0m\]"

export CLICOLOR=1
export LSCOLORS=GxFxCxDxBxegedabagaced

3. add folowing lines to this file, will add kubrctl namespace in prompt

source "/usr/local/opt/kube-ps1/share/kube-ps1.sh"
PS1='$(kube_ps1)'$PS1

4. save the file and source the file, prompt will change
