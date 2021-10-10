# Git Branch

- [Git Branch](#git-branch)
  - [List branch](#list-branch)
  - [Create branch](#create-branch)
  - [Rename branch](#rename-branch)
  - [Delete branch](#delete-branch)
  - [Switch branch](#switch-branch)
  - [Merge branch](#merge-branch)
  - [Graph](#graph)
  - [Restore branch](#restore-branch)
  - [Create branch in specific commit](#create-branch-in-specific-commit)

## List branch

```zsh
git branch
```

## Create branch

```zsh
git branch <branch name>
```

## Rename branch

```zsh
git branch -m <target branch> <branch name>
```

## Delete branch

```zsh
git branch -d <target branch>

git branch -D <target branch> # force to delete (not merge)
```

## Switch branch

```zsh
git checkout <target branch>
```

## Merge branch

```zsh
git merge <target branch>
# base branch is current branch, HEAD is current branch
```

```zsh
git rebase <target branch>
# base branch is target branch, HEAD is current branch
```

## Graph

```zsh
git merge <target branch> --no-ff # not use fast ofrward
```

## Restore branch

```zsh
git branch <branch name> <SHA-1>
```

## Create branch in specific commit

```zsh
git branch <branch name> <SHA-1>

git checkout -b <branch name> <SHA-1>
```
