# basics
for personal use only


## 1. Git

### 1.1 set up user name and email for commits
```bash
git config --global user.name=""
git config --global user.email=""
```

### 1.2 obtain/fetch changes from remote
```bash
git clone url # obtain for the first time
git pull url # fetch the updates
```

### 1.3 check the changes
```bash
git status # file-level change between current version and the last commited version
git diff # code-level unstaged change
```

### 1.4 save the change
```bash
# commit
git add * or git add file
git commit -m "message"

# temporary save
git stash save
```
