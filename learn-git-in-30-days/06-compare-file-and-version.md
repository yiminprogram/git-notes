# compare file and version

- `git diff`

compare working tree to index

- `git diff <commit hash>`

compare working tree to specific commit object

```zsh
git diff HEAD # compare working tree to latest version
```

- `git diff --cached <commit hash>`

compare current index status to specific commit object

```zsh
git diff --cached HEAD # compare current index to latest version
```

> `git diff --cached` same as `git diff --staged`

> `--staged` is `--cached` alias

> `git diff --cached` same as `git diff --cached HEAD`

- `git diff <old commit object> <new commit object>`

compare two specific version

```zsh
git diff HEAD^ HEAD # compare previous version to latest version
```
