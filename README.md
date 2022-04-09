## To initiate a git repo in an directory
git init

## To view the status
git status

## Add all the files
git add . 

## To commit the changes
git commit -m <commit-message>

## To unstage files
git restore --staged <file-name>

## To view the history of git
git log

## To get back to prev commit or to remove all the commits after a particular commit, All the modified files are moved to unstaged area
git reset <commit hash ID>

## To save the progress without commiting or losing the changes (stash)
git add <files> ; git stash

## To move all the files in the stash to the unstaged area
git stash pop

## To remove al the files in the stash
git stash clear

## To add the external repo url to local git
git remote add origin <url>

## To view all the urls attached to the git folder
git remote -v

## Pushing changes
# format : git push <name assigned to url (origin for personal git account)> <branch-name>
git push origin main 

# force pushing when the we do not have the changes that remote has
git push origin main -f

## Creating a new branch
git branch <branch-name>

## Switching to the new branch
git checkout <branch-name>

## Adding an upstream url(The url of the original git repo from where the you have forked it) after forking a repo
git remote add upstream <url-name>

git fetch
# git reset --hard origin/main
git reset --hard <branch-name> 

## List all branches
git branch --list

## Delete a branch
git branch <branch-name> -d

## Listing the config of current git repo
git config --list

## Listing the global configs
git config --global --list

## Getting help e.g. git help branch
git help <command>

## Merging many commits into a single commit
#M1
git reset <commit-ID of the commit after which all the commits have to be merged>; git add .;git commit -m <message for merging commits>
#M2
git rebase -i <commit-ID of the commit after which all the commits have to be merged>

