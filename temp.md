# Git Basic

- [Git Basic](#git-basic)
  - [Commit Log](#commit-log)
  - [Delete or Rename](#delete-or-rename)
  - [Add File To Last Commit](#add-file-to-last-commit)
  - [New folder](#new-folder)
  - [Restore File](#restore-file)
  - [Reset Commit](#reset-commit)
  - [Reset](#reset)
  - [Commit Partial Code](#commit-partial-code)

## Commit Log

## Delete or Rename

- delete file

```zsh
git rm <file name> # auto add
```

or

```zsh
rm <file name>

git add <file name>
```

- untracked file

```zsh
git rm <file name> --cached
```

- rename file

```zsh
git mv <file name> <new file name>
```

or

```zsh
mv <file name> <new file name>

git add <new file name>
```

- edit last commit

```zsh
git commit --amend -m "commit content"
```

## Add File To Last Commit

```zsh
git commit --amend --no-edit # --no-edit -> do not want to edit commit content
```

## New folder

new empty folder git can not detect

add `.keep` or `.gitkeep` file let git detect empty file

```zsh
touch newFolder/.gitkeep
```

## Restore File

```zsh
git checkout <file name> # restore specific file

git checkout . # restore all  file

git checkout HEAD~2 <file name> # restore last 2 versions
```

## Reset Commit

```zsh
git reset <commit id^> # ^ mean previous

git reset master^

git reset HEAD^

git reset <commit id> # back to specific commit
```

## Reset

| mode              | mixed      | soft       | hard   |
| ----------------- | ---------- | ---------- | ------ |
| working directory | not change | not change | delete |
| staging area      | delete     | not change | delete |

check reset commit

```zsh
git reflog

git log -g
```

## Commit Partial Code

```zsh
git add -p <file name>
```
