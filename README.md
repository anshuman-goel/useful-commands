[TOC]
# Useful Commands irrespective of Platform

------
### Git
#### Revert a commit
`git revert <commit hash>`

#### Checkout to remote branch
`git checkout -t origin/<branch name>`

#### Create a new branch and switch to it
`git checkout -b <branch name>`

#### Pushing a new branch created locally
`git push --set-upstream origin <branch name>`

#### Pushing an existing local and remote branch
`git push`

#### Check remote url for repo
`git remote -v`

#### Checkout file to original or origin/master
`git checkout origin/master -- path/to/file`

#### Delete a remote branch
`git push origin --delete <branch name>`

#### Delete a local branch
`git branch -f -d <branch names>`

#### Delete all local branches except master
##### Powershell
`git branch | %{ $_.Trim() } | ?{ $_ -ne 'master' } | %{ git branch -D $_ }`

#### error: local refs could not be updated
Error similar to:
```
error: cannot lock ref 'refs/remotes/origin/master': is at 2e4bfdb24fd137a1d2e87bd480f283cf7001f19a but expected 70ea06a46fd4b38bdba9ab1d64f3fee0f63806a5
 ! 70ea06a46f..2e4bfdb24f  master     -> origin/master  (unable to update local ref)
```
`git remote prune origin`
This will delete local refs of branches that doesn't exists in origin master

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

#### Updating forked repo with upstream
```
git remote add upstream https://github.com/microsoft/onefuzz
git fetch upstream
git checkout main
git rebase upstream/main
```

------
### Python
#### Install pip package
`pip install <package name>`

------
