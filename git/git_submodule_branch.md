---
date: 2023-04-01
author: "Josh Cowley"
---

# Git Submodules Notes

## Setting Up Submodule to Track Branch

Looking into setting up git submodules to follow branches over commits.

To set up a submodule and track some branch `<branch`, use the `-b` flag.

```sh
git submodule add -b <branch> <remote_url>
```

If a submodule already exists, adding a branch can be done using the
`set-branch` subcommand, available since Git 2.22 (Q2 2019).

```sh
git submodule set-branch --branch <branch> -- <path_to_submodule>
```

We can make all submodules checkout the latest commit on the remote version
of the chosen branch, typically in a detached head state.

```sh
git submodule update --recursive --remote
```

Recall if the repository is a fresh clone, the submodules must be initialised
first.

```sh
git submodule update --init --recursive
```

Which could have been done on clone with

```sh
git clone --recurse-submodules https://github.com/username/repo.git
```