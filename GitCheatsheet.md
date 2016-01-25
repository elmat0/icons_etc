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
git reset --hard upstream/master

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
git push origin :<branch name>
```

