### Code Change Check-in
```shell
git branch -va
git checkout -b sathvik-pn/feat main
git push -u origin sathvik-pn/feat 

# check-in
git add <files>
git commit -m 'commit msg'

# sync remote
# git fetch origin  # git fetch --all
git checkout main
git pull origin main

# put all feat-commits after main-commits
git checkout sathvik-pn/feat
git rebase -i origin/main

# merge-conflict check
git status

# resolve conflicts
git rebase --continue

# git rebase --abort if any mistake while merging

# Force push (rewritten history)
git push -f origin sathvik-pn/feat

```

### Quick commands

```shell
# Reset working copy to latest committed state
git reset --hard HEAD

# Remove untracked files and dirs
git clean -df

# checkout remote branch
git fetch origin
git checkout -b feat origin/feat

```
