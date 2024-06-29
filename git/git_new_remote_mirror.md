---
date: 2023-04-11
author: "Josh Cowley"
---

# Git New Remote as Mirror

Suppose we have a repository where `origin` points to GitLab and we want to
    create a mirrored remote URL that we can also push to.

Within the local version of the repo, create a new remote with

```sh
git remote add <github> git@github.com:username/repo.git
```

where `<github>` is the name of the remote and can be changed and it is
    assumed that `git@github.com:username/repo.git` is an empty repository.

We then push using the mirror option.

```sh
git push --mirror github
```
