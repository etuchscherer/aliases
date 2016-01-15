# Aliases
A collection of aliases I frequent.

## Installation

Add this to your `~/.zshrc` and profit.

    # include aliases
    [[ -f ~/.aliases ]] && source ~/.aliases

## Aliases
### Unix
    ll="ls -al"
    ln="ln -v"
    mkdir="mkdir -p"
    e="$EDITOR"
    v="$VISUAL"
    src="source ~/.zshrc"

### Redis
    sr="redis-server /usr/local/etc/redis.conf"

### SITEUI specific
    llk="cd $HOME/links && roots watch"
    st="$HOME/apache-tomcat-6.0.44/bin/startup.sh && open http://localhost:8080"
    kt="$HOME/apache-tomcat-6.0.44/bin/shutdown.sh"
    nn="cd $HOME/Sites/siteuicli"
    nnn="cd $HOME/Sites/siteuicli && ember build --w"
    vv="cd $HOME/Sites/site-node-api"
    vvv="cd $HOME/Sites/site-node-api && node run-eslint.js -s"
    cc="cd /usr/local/etc/site-config"

### Git
    g="git status"
    gs="git status"
    gg="git checkout"
    gb="git branch"
    gl="git whatchanged"
    gd="git difftool -y"
    gm="git mergetool -y"

### Bundler
    b="bundle"

### Rails
    migrate="rake db:migrate db:rollback && rake db:migrate"
    s="rspec"

### Node
    nombom="rm -rf node_modules bower_components && npm cache clean && bower cache clean && npm install && bower install" 

### Pretty print the path
    path='echo $PATH | tr -s ":" "\n"'
