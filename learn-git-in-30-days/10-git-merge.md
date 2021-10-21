# git merge

## merge branch

```zsh
git merge <target_branch>
```

## delete branch

```zsh
git branch -d <branch_name>
```

## recover branch

```zsh
git branch <target_branch> <last_branch_hash>
```

## recover merge

```zsh
git reset --hard ORIG_HEAD # back to previous version
```

## compare specific file

```zsh
git diff <file_path>
```

## list conflict file

```zsh
git ls-files -u
```
