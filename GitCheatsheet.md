#Git CheatSheet

Various Git commands and workflows I always forget...

Add upstream repo as a remote:
```
git remote add upstream <url of upstream .git>
```

Sync remote master to upstream:
```
git pull upstream master
git push origin master
```

Create and switch to a new local branch:
```
git fetch upstream
git checkout -b <new branch>
```

Rebase local branch on the latest upstream:
```
git fetch upstream
git rebase -i upstream/develop <branch name>
```

Resolve conflicts when doing the above:
```
git add <filename>
git rebase --continue
```

Push local branch up to my fork:
```
git push -f origin <branch name>
```

Delete local branch:
```
git branch -d <branch name>
```

Delete remote branch:
```
git fetch -p
```

