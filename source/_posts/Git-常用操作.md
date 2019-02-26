---
title: Git 常用操作
date: 2019-02-26 21:05:55
tags:
    - Git
---
# 1. 将远程git仓库里的指定分支拉取到本地（本地不存在的分支）
当我想从远程仓库里拉取一条本地不存在的分支时：
`git checkout -b 本地分支名 origin/远程分支名`
这个将会自动创建一个新的本地分支，并与指定的远程分支关联起来。
例如远程仓库里有个分支dev2,我本地没有该分支，我要把dev2拉到我本地：
若成功，将会在本地创建新分支dev2,并自动切到dev2上。
如果出现提示：
```
fatal: Cannot update paths and switch to branch 'dev2' at the same time.
Did you intend to checkout 'origin/dev2' which can not be resolved as commit?
```
表示拉取不成功。我们需要先执行
`git fetch`
然后再执行
`git checkout -b 本地分支名 origin/远程分支名`
即可。