# git object structure

## object

- blob object
- tree object
- commit object
- tag object

## show last tree object

```zsh
git cat-file -p main
```

## show tree object detail

```zsh
git cat-file -p <tree object hash>
```

## calculate object hash

```zsh
git hash-object <filename>
```

1. create file
2. git add, track file
3. git will create blob object(only contain file content)
4. git commit
5. git will create commit object and tree object
6. commit object contain tree object
7. tree object contain track file blob object
8. edit file, or create new file
9. create new blob object, same file content will assign same blob object
