---
title: How to undo last commit message in Git
publish_date: 2022-11-07
---

## Amend the most recent commit message:

```shell
git commit --amend -m "New message"
```

## Changes already pushed to remote branch

```shell
git push <remote> <branch> -f
```
