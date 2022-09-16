# Git Learning
## Most important git commands
### git init
`git init` creates a new repository on your local filesystem, isolated to your computer and unlinked to a remote.

### git clone
`git clone <repository URL>` lets you clone a remote repository to your local filesystem. This is the beginning of everything!

### git fetch
`git fetch`, when run inside a repository folder, fetches any new changes into the repository, but doesn't affect any files.

### git pull
`git pull` will also fetch any remote changes, but will apply the changes to your local repository.

### git add
`git add <file(s)>` adds new local files to the repository's tracking structure. A file must be added before it can be uploaded. `git add .` will add all untracked (& unignored) files in the repository directory. A file only has to be added once, afterwards changes will be automatically tracked.

### git commit
`git commit -m "<commit message>" is the quintessential git command. Changes in git are stored as commits, which track the changes between different file versions and allow the version management that git is intended for. Commit messages should be descriptive, you'll thank yourself later!

### git push
`git push` is the culmination of all the work so far, and finally uploads your local changes to the remote repository (on GitHub). Sometimes, the terminal will ask you to run `git push -u origin master` once, but afterwards `git push` should work alone.

## Other git commands
### git branch
Git allows multiple developments to happen simultaneously, using what it calls branches. Branches store their own commit history and don't affect one another during development. `git branch -a` lists the branches in a repository.

### git checkout
`git checkout <branch name>` changes your local repository filesystem to the branch specified. `git checkout -b <branch name>` will create a new branch on your local repository, which can then be developed in and pushed to the remote repository.

### git reset, git merge
***Pray you never need these.***

## Developing on GitHub
1. Create a fork of the development repository. Forks let you develop a repository without having write permissions.
2. Create a branch on your fork, named appropriately for your task.
3. Clone your fork locally and checkout the new branch.
4. Develop and commit often.
5. Push changes to your fork feature branch.
6. Create a PR (pull request) into the original dev repository. PRs bring changes in from forks & branches, and are approved by repo maintainers.

Try it now! Follow the steps to modify the line below to include your name, and submit a PR to this repo :)

Hello world! Sebastian knows git!
