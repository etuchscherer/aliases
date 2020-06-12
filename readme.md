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
# Unix
#---------------------------------------

# Long list [ll]
alias ll="ls -al"
alias ln="ln -v"
# always make the directory -p is for chumps
alias mkdir="mkdir -p"
alias e="$EDITOR"
alias v="$VISUAL"

#Redis
#---------------------------------------
# Start Redis [sr]
alias sr="redis-server /usr/local/etc/redis.conf"

# Classmates siteui specific
#---------------------------------------
alias llk="cd $HOME/links && roots watch"
# TU / TOMCAT UP - is now a script running in /usr/local/bin
# alias tu="$CATALINA_HOME/bin/startup.sh && open http://localhost:8080"
alias tl="tail -f $CATALINA_HOME/logs/catalina.out"
alias td="$CATALINA_HOME/bin/shutdown.sh"
alias tbounce="td && tu"
alias t-reset="kt && cd ~/Sites/siteui/ && git pull && mvn clean install && cp ~/Sites/siteui/target/siteui*.war $CATALINA_HOME/webapps/siteui.war"
alias natom="cd $HOME/Sites/siteuicli && atom ."
alias nn="cd $HOME/Sites/siteuicli"
alias nnn="cd $HOME/Sites/siteuicli && ember build --w"
alias ppp="cd $HOME/Sites/siteuicli && ember build -p -w"
alias patom="cd ~/$HOME/Sites/site-node-api && atom ."
alias vv="cd $HOME/Sites/site-node-api"
alias vvv="refresh_node_api"
alias cc="cd /usr/local/etc/site-config"
alias qanode="i2cssh -F -2 --cluster=qanode"

# Local Ember Docs
#---------------------------------------
alias ember-api="cd ~/Ember/website && bundle exec middleman"
alias ember-guides="cd ~/Ember/guides && bundle exec middleman"
alias cli-docs="cd ~/Ember/cli-docs && jekyll serve"
alias middleman="open http://etuchscherermac.local:4567"

# Git
#---------------------------------------
alias g="git status"
alias gg="git checkout"
alias gb="git branch"
alias gl="git whatchanged"
alias gd="git difftool -y"
alias gdd="git log -p -1"
alias gm="git mergetool -y"

# Bundler
alias b="bundle"

# Rails
alias migrate="rake db:migrate db:rollback && rake db:migrate"
alias s="rspec"

# Node
alias nombom="rm -rf node_modules bower_components && npm cache clean && bower cache clean && npm install && bower install" 
alias npmbom="nombom"

# Pretty print the path
alias path='echo $PATH | tr -s ":" "\n"'

# Include custom aliases
[[ -f ~/.aliases.local ]] && source ~/.aliases.local

# ssh
alias qa09='ssh HOME-APP01.QA09.SEA1.CMATES.COM'
alias node01='ssh nodejs01.qa09.sea1.cmates.com'
alias node02='ssh nodejs02.qa09.sea1.cmates.com'
