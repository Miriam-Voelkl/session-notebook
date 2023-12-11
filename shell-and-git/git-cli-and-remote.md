## Basic Git Workflow mit GitHub :github:

## Once

In the shell

git init # create a repo (once per project)

# don't forget to add a .gitignore file

git remote add origin <ssh-path-to-github>

## For each feature

In the shell
git switch -c <branchname> # create a new branch
git add <file> # add a file to the stage
git status # check, if everything is ok
git commit -m "<message>" # commit your changes
git push -u origin <branchname> # push to GitHub

# continue on GitHub

## On GitHub

- Create a pull request for that branch (to merge it into main)
- Send a link to the changed files to your team
- Get a code review
- Optional: implement changes, push again to update pull request
- Merge and delete the branch on GitHub
- Continue in the shell

## Again in the shell

git switch main
git pull # get the merged commits in your local main
git branch -d <oldbranchname> # delete the merged branch

## Git branch commands

| command                    | functionality                        |
| -------------------------- | ------------------------------------ |
| git switch -c <branchname> | create a new branch and switch to it |
| git switch <branchname>    | switch branches                      |
| git branch                 | list your branches                   |
| git branch -a              | list all branches (local and remote) |
| git branch -d <branchname> | delete a branch                      |
