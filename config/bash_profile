if [ "$TERM" = "xterm" ]; then
	export TERM=xterm-256color
fi

gb() {
    echo -n ' (' && git branch 2>/dev/null | grep '^*' | colrm 1 2 | tr -d '\n' && echo  -n ')'
}
git_branch() {
    gb | sed 's/ ()//'
}

#export PS1="   λ \[\033[0;35m\]\W\[\033[0m\]$(git-ps1 " (%s)"): "
export PS1="   λ \W\$(git_branch): "
