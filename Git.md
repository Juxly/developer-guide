## Create a global ~/.gitignore file

```
# Compiled source #
###################
*.com
*.class
*.dll
*.exe
*.o
*.so

# Packages #
############
# it's better to unpack these files and commit the raw source
# git has its own built in compression methods
*.7z
*.dmg
*.gz
*.iso
*.jar
*.rar
*.tar
*.zip

# Logs and databases #
######################
*.log
*.sql
*.sqlite

# OS generated files #
######################
.DS_Store
.DS_Store?
._*
.Spotlight-V100
.Trashes
ehthumbs.db Thumbs.db
```

## Create a ~/.gitconfig file

```
[color]
    diff = auto
    status = auto
    branch = auto
[user]
    name = YourName
    email = YourEmail
[core]
    autocrlf = input
[alias]
    s = status
    cam = commit -am
    amd = commit -a --amend
    com = commit
    cm = commit -m
    st = status
    d = diff
    dt = difftool
    ci = commit -v
    cia = commit -v -a
    co = checkout
    cob = checkout -b
    cp = cherry-pick
    mg = merge
    mgt = mergetool
    dci = svn dcommit
    l = log
    ll = log -p
    lm = log master..
    llm = log -p master..
    b = branch
    lg = log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --date=relative
[push]
    default = simple
```
