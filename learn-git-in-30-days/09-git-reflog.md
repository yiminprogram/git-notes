# git reflog

## list git version records

edit ref will record history

```zsh
git reflog

git reflog <branch_name>
```

## list reflog detail

```zsh
git log -g
```

## delete reflog

```zsh
git reflog delete ref@{specifier}
```

## set reflog delte time

default will retain 30 days

```zsh
git config --global gc.reflogExpire "never"

git config --global gc.reflogExpireUnreachable "never"
```

```zsh
git config --global gc.reflogExpire "7 days"

git config --global gc.reflogExpireUnreachable "7 days"
```

```zsh
git config --local gc.reflogExpire "7 days"

git config --local gc.reflogExpireUnreachable "7 days"
```

## clean all reflog

```zsh
git reflog expire --expire=now --all
```

## refresh

refresh or delete can not found and track version

```zsh
git gc
```
