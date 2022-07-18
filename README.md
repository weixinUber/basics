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

# temporary save (locally)
git stash save
git stash list #list all the temporarily saved changes
git stash pop #reload the temporarily saved changes
git stash drop #remove the temporarily saved changes
```

### 1.5 sync difference between branches
```bash
# clone and generate a new branch
git checkout -b new_branch 

# propagate changes from source branch to the target branch
git rebase src_branch dst_branch
```

### 1.6 go back to the previous committed version

```bash
# go back to a previous commit
git checkout commit_id .

# discard the changes
git reset --hard commit_id

# not discard
git reset commit_id
git stash save
```

### 1.7 delete branch
```bash
# locally
git branch -d branch_name #checkout to another branch first

# remote
git branch origin --delete remote_branch_name
```
