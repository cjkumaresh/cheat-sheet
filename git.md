### To list global git config
```sh
git config --global -l
```

### To Enable long filename

```sh
git config --system core.longpaths true
```

### To List Remote urls

```sh
git remote -v
```

### To replace a branch with another branch

```sh
git checkout [branch2]
git merge -s ours [branch1]
git checkout [branch1]
git merge [branch2]
```

The above will merge [branch2] into [branch1] discarding [branch1] changes


### To Delete branch in local

```sh
git branch -D [branch]
```

### To create a new branch

```sh
git checkout -b [branch]
```

### To stage modified/deleted files only

```sh
git add -u
```

### To revert ranges of commit

```sh
git revert <oldest_commit_hash>..<latest_commit_hash>
```

### To delete branch in remote
```sh
git push origin --delete [branch_name]
```

### To change the origin url after repo name changed
```sh
git remote set-url origin [new_url]
```

### To remove latest commit, keeping the work you've done
```sh
git reset --soft HEAD~1
```

### To remove latest commit, destroying the work you've done
```sh
git reset --hard HEAD~1
```
### To remote sync the forked repo
```sh
git remote add upstream [upstream_url]
git fetch upstream
git checkout master
git merge upstream/master
git push
```
### Tp remove information on branches that were deleted on origin
```sh
git remote prune origin or git fetch --prune
```
