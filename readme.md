# Aliases

A collection of aliases I frequently use. 

## Installation

```
# ensure local aliases are available
[[ -f ~/.aliases ]] && source ~/.aliases.local

# then get these aliases
wget -O ~/.aliases.local https://raw.githubusercontent.com/etuchscherer/aliases/master/.aliases
```

```
# https://github.com/etuchscherer/aliases/blob/master/readme.md

# Unix
alias ll="ls -alh"
alias ln="ln -v"
alias mkdir="mkdir -p"
alias e="$EDITOR"
alias v="$VISUAL"
alias src="source ~/.zshrc"
alias ali="vi ~/.aliases.local"
alias aliases="cat ~/.alias/.aliases"
alias nlc="npm-link-check"
alias nlk="nlc"
# yarn links
alias nly="ls -l node_modules"
alias tmof="sudo lsof -n | cut -f1 -d' ' | uniq -c | sort | tail"

# awk shortcuts
alias c1="awk '{printf \$1}'"
alias c2="awk '{printf \$2}'"
alias c3="awk '{printf \$3}'"
alias c4="awk '{printf \$4}'"
alias c5="awk '{printf \$5}'"
alias c6="awk '{printf \$6}'"
alias c7="awk '{printf \$7}'"
alias c8="awk '{printf \$8}'"
alias c9="awk '{printf \$9}'"

# Testing
alias te="test_email | pbcopy"

#Redis
alias sr="redis-server /usr/local/etc/redis.conf"

alias llk="open http://links.local"
alias tu="$CATALINA_HOME/bin/startup.sh" 
alias tl="tail -f $CATALINA_HOME/logs/catalina.out"
alias td="$CATALINA_HOME/bin/shutdown.sh"
alias tbounce="td && tu"
alias mvnci="mvn clean install"

# Ember
alias ember-api="cd ~/Ember/website && bundle exec middleman"
alias ember-guides="cd ~/Ember/guides && bundle exec middleman"
alias cli-docs="cd ~/Ember/cli-docs && jekyll serve"
alias middleman="open http://etuchscherermac.local:4567"

# Git
alias g="git status"
alias gs="git status"
alias gg="git checkout"
alias gb="git branch"
alias gd="git difftool -y"
alias gm="git mergetool -y"
alias gw="git whatchanged"
alias gdd="git log -p -1"
alias gam="git commit --amend"

#svn
alias s="svn status"
alias si="svn info"

# Bundler
alias b="bundle"

# Rails
alias migrate="rake db:migrate db:rollback && rake db:migrate"

# Node
alias nombom="rm -rf node_modules bower_components && npm cache clean && bower cache clean && npm install && bower install" 
alias npmbom="nombom"

# Pretty print the path
alias path='echo $PATH | tr -s ":" "\n"'
```
