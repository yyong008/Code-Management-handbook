---
title: git 分支部分
---

## 问题

1. ***如何查看关联的远程分支？***

- 使用 vim 来查看

```Shell
cd .git

vim.config
```

就会得到一些信息：

```
[core]
        repositoryformatversion = 0
        filemode = true
        bare = false
        logallrefupdates = true
        ignorecase = true
        precomposeunicode = true
[remote "origin"]
        url = git@github.com:username/projectRepoName.git
        fetch = +refs/heads/*:refs/remotes/origin/*
~                                                      
```
