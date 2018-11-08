# Config
- `git config --global user.name "Daniel Schaefer"` | sets global username
- `git config --global user.email schaefer.dev@gmail.com` | sets global useremail

# Remote
- `git remote -v` | view existing remotes
- `git remote add origin https://github.com/schaefer-dev/project.git` | add remote origin
- `git remote set-url origin https://github.com/schaefer-dev/project.git` | change remote origin
- `git clone --recursive https://github.com/schaefer-dev/project.git` | clone repo including submodules
- `git push origin master` | push master to origin

# Branches
- `git branch amazing_new_feature` | creates new branch
- `git branch` | lists branches
- `git checkout amazing_new_feature` | switches branch, commits now in this branch
- `git checkout master` `git merge amazing_new_feature` | new feature is completed, back to the master branch and merging it
- `git branch -d awesome_new_feature` | deletes branch

# Submodules
- `git submodule add https://github.com/schaefer-dev/project.git path` | adds submodule to existing repo
- `git submodule init path` | initializes submodule
- `git submodule update --init --recursive` | updates submodules and initializes uninitialized ones

# Advanced
- `git show [commit]` | shows commit content
- `git diff [commit1]..[commit2]` | shows differences between both commits
- `git commit --amend` | fix commit typo (or missing added file) before push happened
