---
title: Git 别名设置
date: 2019-02-22 11:36:19
categories:
    - Git
tags: 
    - Git
---

# Git 常用别名设置 
```
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.ci 'commit -m'
git config --global alias.st status
git config --global alias.unstage 'reset HEAD --'
git config --global alias.last 'log -1 HEAD'

```