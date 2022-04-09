## To initiate a git repo in an directory

<code>git init</code>

## To view the status

<code>git status</code>

## Add all the files

<code>git add . </code>

## To commit the changes

<code>git commit -m `<commit-message>`</code>

## To unstage files

<code>git restore --staged `<file-name>`</code>

## To view the history of git

<code>git log</code>

## To get back to prev commit or to remove all the commits after a particular commit, All the modified files are moved to unstaged area

<code>git reset `<commit hash ID>`</code>

## To save the progress without commiting or losing the changes (stash)

<code>git add `<files>` ; git stash</code>

## To move all the files in the stash to the unstaged area

<code>git stash pop</code>

## To remove al the files in the stash

<code>git stash clear</code>

## To add the external repo url to local git

<code>git remote add origin `<url>`</code>

## To view all the urls attached to the git folder

<code>git remote -v</code>

## Pushing changes

<code> format : git push `<name assigned to url (origin for personal git account)> <branch-name>`</code>

<code>git push origin main </code>

### force pushing when the we do not have the changes that remote has

<code>git push origin main -f</code>

## Creating a new branch

<code>git branch `<branch-name>`</code>

## Switching to the new branch

<code>git checkout `<branch-name>`</code>

## Adding an upstream url(The url of the original git repo from where the you have forked it) after forking a repo

<code>git remote add upstream `<url-name>`</code>

<code>git fetch</code>

## git reset --hard origin/main

<code>git reset --hard `<branch-name>` </code>

## List all branches

<code>git branch --list</code>

## Delete a branch

<code>git branch `<branch-name>` -d</code>

## Listing the config of current git repo

<code>git config --list</code>

## Listing the global configs

<code>git config --global --list</code>

## Getting help e.g. git help branch

<code>git help `<command>`</code>

## Merging many commits into a single commit

### M1

<code>git reset `<commit-ID of the commit after which all the commits have to be merged>`; git add </code>.;git commit -m `<message for merging commits>`

### M2

<code>git rebase -i `<commit-ID of the commit after which all the commits have to be merged>`</code>
