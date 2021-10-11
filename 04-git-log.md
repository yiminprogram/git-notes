# git log

## all

```zsh
git log

git log --oneline --graph
```

## author

```zsh
git log --author="name"

git log --author="name1\|name2"
```

## commit cotent

```zsh
git log --grep="search string"
```

## file name

```zsh
git log -S "file name"
```

## time

```zsh
git log --since="9am" --until="12am" #today 9am to 12am commit list

git log --since="9am" --until="12am" --after="2021-06" # after 2021-06 every day at 9am to 12am commit list
```

## specific file commit

```zsh
git log <file name>

git log -p <fiile name> # look edit record
```

## code author detail

```zsh
git blame <file name>

git blame -L 5,10 <file name> # check file line 5 to 10 author
```
