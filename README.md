# Useful Commands irrespective of Platform

------
### Git
#### Revert a commit
`git revert <commit hash>`

#### Checkout to remote branch
`git checkout -t origin/<branch name>`

#### Create a new branch and switch to it
`git checkout -b <branch name>`

#### Check remote url for repo
`git remote -v`

#### Checkout file to original or origin/master
`git checkout origin/master -- path/to/file`

#### Delete a remote branch
`git push origin --delete <branch name>`

#### Delete a local branch
`git branch -f -d <branch names>`

#### error: some local refs could not be updated
`git remote prune origin`

#### Branch in which commit exists remotely (`-r`)
`git branch --contains <commit hash> -r`

*(Do remember to pull latest changes)*

#### Removing untracked files from Git working Tree
```
# Print out the list of files which will be removed (dry run)
git clean -n

# Delete the files from the repository
git clean -fd
```

------
### Python
#### Install pip package
`pip install <package name>`

------
