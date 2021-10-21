# git tag

- lightweight tag
- annotated tag

## list all tag

```zsh
git tag
```

## create tag

```zsh
git tag <tag_name> # lightweight tag

git tag <tag_name> -a -m <"message"> # annotated tag

git tag <tag_name> <hash> # specific version
```

## delete tag

```zsh
git tag <tag_name> -d
```
