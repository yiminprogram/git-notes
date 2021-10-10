# Git History

- [Git History](#git-history)
  - [Edit history](#edit-history)

## Edit history

```zsh
git rebase -i <SHA-1> # edit history from specific commit to current commit
```

```zsh
# result
pick 123456 commit content
pick 123456 commit content
pick 123456 commit content
pick 123456 commit content
pick 123456 commit content
```

- pick -> no edit
- reword(edit commit) -> want to edit
- squash(merge commit) -> merge previous commit
- edit -> disassemble commit or add new commit between old commit

> SHA-1 after edited commit will all change

```zsh
git rebase --continue
```

undo rebase

```zsh
git reset ORIG_HEAD --hard
```
