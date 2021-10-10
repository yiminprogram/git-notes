# Git Basic

- [Git Basic](#git-basic)
  - [Initial](#initial)
  - [Add](#add)
  - [Commit](#commit)
  - [Skip Add (untracked file not working)](#skip-add-untracked-file-not-working)
  - [Commit Log](#commit-log)
  - [Delete or Rename](#delete-or-rename)
  - [Add File To Last Commit](#add-file-to-last-commit)
  - [New folder](#new-folder)
  - [Restore File](#restore-file)
  - [Reset Commit](#reset-commit)
  - [Reset](#reset)
  - [Commit Partial Code](#commit-partial-code)

## Initial

```zsh
git init
```

## Add

- add all file

```zsh
git add . # current directory

git add --all # all repository file
```

- add specific file

```zsh
git add <file name>

git add *.html # all html file
```

## Commit

```zsh
git commit # into editor edit message"

git commit -m "commit message"
```

- empty commit

```zsh
git commit --allow-empty -m
```

## Skip Add (untracked file not working)

```zsh
git commit -a -m "commit"
```

## Commit Log

- all

```zsh
git log

git log --oneline --graph
```

- author

```zsh
git log --author="name"

git log --author="name1\|name2"
```

- commit cotent

```zsh
git log --grep="search string"
```

- file name

```zsh
git log -S "file name"
```

- time

```zsh
git log --since="9am" --until="12am" #today 9am to 12am commit list

git log --since="9am" --until="12am" --after="2021-06" # after 2021-06 every day at 9am to 12am commit list
```

- specific file commit

```zsh
git log <file name>

git log -p <fiile name> # look edit record
```

- code author detail

```zsh
git blame <file name>

git blame -L 5,10 <file name> # check file line 5 to 10 author
```

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
