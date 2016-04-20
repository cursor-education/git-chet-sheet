# Git Cheat Sheet

http://explainshell.com/

## Config
```shell
$ git config --global alias.co checkout
$ git config --global alias.br branch
$ git config --global alias.ci commit
$ git config --global alias.st status
```

## Branch
```shell
$ git branch BRANCH   # to create a new branch
$ git checkout -b BRANCH   # to create & switch to a new branch

$ git checkout BRANCH   # to switch to a new branch

$ git branch -d BRANCH   # to delete a branch locally
$ git branch -D BRANCH   # to delete a local branch (that wasn't merged)
$ git push origin :BRANCH   # to delete a remote branch
```

## Merge
```shell
$ git checkout master
$ git pull origin master
$ git merge feature
$ git push origin master

$ git checkout feature
$ git rebase master   # to merge master's changes to feature-branch

$ git add file.txt
$ git rebase --continue
```

## Revert
```shell
$ git lg -p    # to view log \w diff per commit
```

## Log
```shell
$ git log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit
```
![](http://new.tinygrab.com/7020c0e8b09291f70b7a01c3231a53e9b46f26de34.png)
