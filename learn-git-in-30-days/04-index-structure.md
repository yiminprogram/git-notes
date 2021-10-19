# index structure

create git version -> update index status -> commit

# file status

1. untracked
2. unmodified
3. modified
4. staged

## git status

git version control -> working tree change -> update index -> create git object

## git add

working tree change write in index

```zsh
git add

git add -u # only add tracked file
```

## git rm

delete file

```zsh
git rm <filename> # will delete physical file

git rm <filename> --cached # only delete file in the index
```

## git mv

filename change

```zsh
git mv <old_filename> <new_filename>
```

## git commit

compare index to new version, and commit version difference to a commit object

## git ls-files

list all tracked file in index

```zsh
git ls-files
```
