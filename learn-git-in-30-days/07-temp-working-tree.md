# temp working tree

## create temp working tree

```zsh
git stash # only add tracked file

git stash -u # add all file

git stash save -u <"message">
```

> `git stash` = `git stash save`

## check temp commit object

```zsh
git cat-file -p stash
```

## merge temp working tree

```zsh
git stash pop # delete temp

git stash apple # retain temp

git stash apple <"stash_id"> # specific temp version
```

## list all temp working tree

```zsh
git stash list
```

## delete temp

```zsh
git stash drop <"stash_id">
```

## delete all temp

```zsh
git stash clear
```
