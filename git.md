# Config
- `git config --global user.name "Daniel Schaefer"`
- `git config --global user.email schaefer.dev@gmail.com`

# Remote
- `git remote add origin https://github.com/schaefer-dev/project.git`
- `git push origin master`

# Branches
- `git branch amazing_new_feature` | creates new branch
- `git branch` | lists branches
- `git checkout amazing_new_feature` | switches branch, commits now in this branch
- `git checkout master` `git merge amazing_new_feature` | new feature is completed, back to the master branch and merging it
- `git branch -d awesome_new_feature` | deletes branch

# Advanced
- `git show [commit]` | shows commit content
- `git diff [commit1]..[commit2]` | shows differences between both commits
- `git commit --amend` | fix commit typo (or missing added file) before push happened
