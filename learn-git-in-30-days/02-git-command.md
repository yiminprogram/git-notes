# git command

## git add

- all file

```zsh
git add .
```

- specific file

```zsh
git add <filename>

git add .* # all filename start .
```

## git commit

```zsh
git commit

git commit -m "version information"
```

## git log

- all history

```zsh
git log
```

- limit quantity

```zsh
git log -10
```

## delete file

```zsh
git rm <filename>
```

## change file name

```zsh
git mv <old_filename> <new_filename>
```

## git status

```zsh
git status

git status -s # simplify version
```

## reset git status

```zsh
git reset # cannot recover delete file or rename file

git reset --hard # recover delete file or rename file
```

## recover file

```zsh
git checkout main <filename>
```
