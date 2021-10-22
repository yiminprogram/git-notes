# edit commit history

## recover working tree status

```zsh
git reset
```

## delete latest commit

```zsh
git reset --hard HEAD^
```

## recover latest version control

```zsh
git reset --hard ORIG_HEAD
```

## delete latest commit and retain change file

```zsh
git reset --soft HEAD^
```

## edit latest commit

```zsh
git commit --amend
```
