# Git Commands
## Configuration Level
### Local Configuration
```
git config --local user.name="Phanupong"
git config --local user.email="phanupong.pe@gmail.com"
```

### Global Configulation
```
git config --global core.editor "code --new-window --wait"
```

### System Configuration
```
git config --system -e
```

## Git Log
### Filter
```
git log --since=2022-08-14
git log --since="1 days ago"
git log --since=1.days
git log --until=1.days
git log --since=2.weeks --until=1.days
git log --after=2.weeks --before=1.days
git log --grep="readme"
git log --author="phanupong"
git log 34b3..HEAD
git log Readme.md
```

### Format
```
git log -p
git log --stat
git log --format=oneline
git log --oneline
git log --oneline --graph --decorate
```

## Git show
```
git show 6b36
git show HEAD
git show HEAD^
git show HEAD^^^
git show HEAD~5
```

## Git blame
```
git blame Readme.md
```

## Git ls-tree
```
git ls-tree HEAD
git ls-tree main
git ls-tree 13db
```

## Git add and commit
```
git add .
git add Readme.md
git commit -m "commit message"
git commit -am "add and commit"
git commit --amend
git commit --amend -m "commit and add new message"
git remote add origin <URL of remote repository>
git remote -v
```

## Git Remove(git rm)
```
git rm <filename>
git rm --cached <filename>
```

## Git diff
```
git diff 
git diff 9f53..4dde
git diff HEAD..HEAD~2 (Move back)
git diff HEAD~2..HEAD (Move forward)
```

## Git reset
```
git reset --soft HEAD^
git reset --mixed HEAD^
git reset --hard HEAD^
```

## Git revert
```
git revert HEAD^
git revert HEAD^ -e
git revert HEAD^ --no-edit
git revert HEAD^ --no-commit
```