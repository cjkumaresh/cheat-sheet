## To list global git config
```sh
git config --global -l
```

## To Enable long filename

```sh
git config --system core.longpaths true
```

## To List Remote urls

```sh
git remote -v
```

## To replace a branch with another branch

```sh
git checkout [branch2]
git merge -s ours [branch1]
git checkout [branch1]
git merge [branch2]
```

The above will merge [branch2] into [branch1] discarding [branch1] changes


## To Delete branch in local

```sh
git branch -D [branch]
```
