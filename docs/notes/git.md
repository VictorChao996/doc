# Git
  - [config](#config)
  - [Basic usage](#basic-usage)
  - [Remote](#remote)
  - [Branch](#branch)
---

## config
```bash
git config --list

git config user.name "Your Name"
git config user.email your-email@gmail.com

git config --global
git config --local

```

## Basic usage

```
git init
git add .
git commit -m "commit-message"
git log

```

## Remote
```
git remote -v
git remote add <name> <remote-url>

git push 
git pull

git clone
```

## Branch
```
git branch -v
git checkout -b "new-branch"
git checkout <branch>

git merge <branch> //合併分支<branch>到當前分支
git rebase <branch> //將當前分支的基準定義為 <branch>
```