## git config --global user.name "Your Name"
### Specifies the name that will be shown in your commit history

## git config --global user.email "your-email@example.com"
### Specifies the email that will be shown in your  commit history

## git config --list
### Displays a list of all the configuration settings in your Git repository

## mkdir myproject
### Creates a new directory called myproject

## cd myproject
### Changes the current directory to myproject

## git init
### Initializes a new Git repository in the current directory

## echo "My First Project" >> README.md
### Creates a new file called README.md and adds the text "My First Project" to it

## git add REDME.md 
### Stages the file README.md for the next commit

## git commit -m "Initial commit:Added README.md"
### Commits the changes to the repository with a meaningful commit message

## git status
### Displays the status of your repository, including any changes that have not been committed yet

## git log --oneline --graph --decorate
### Displays a graphical representation of your commit history


## *2f8d6a2 (HEAD -> main) Updated README with a description
### allow git to identify each commit in the repository

## *d3c4b21 Initial commit: Added README.md
### allow git to identify each commit in the repository

# Create and clone a repository

## git clone https://github.com/username/repository.git
### Clones a repository from a URL

## echo "workflow example" > workflow.md
### Creates a new file called workflow.md and adds the text "workflow example" to it
### there is difference between > and >> when we use > it will overwrite the file and >> will add the text to the end of the file

## git add workflow.md
### Stages the file workflow.md for the next commit

## git commit -m "Added workflow example"
### Commits the changes to the repository with a meaningful commit message


# Working with repositories

# Branching and merging

## git branch feature-login
### Creates a new branch called feature-login

## git checkout feature-login
### Switches to the feature-login branch
<!-- OR USE -->
## git checkout -b feature-login
### Creates a new branch called feature-login and switches to it

<!-- Add new file and commit changes -->

## echo "Login Page" > login.html
### Adds the text "Login Page" to the end of the file login.html

## git add login.html
### Stages the file login.html for the next commit

## git commit -m "Added login page"
### Commits the changes to the repository with a meaningful commit message

## git checkout main
### Switches to the main branch

## git merge feature-login
### Merges the feature-login branch into the main branch

## git branch branch-A
### Creates a new branch called branch-A

## git branch branch-B
### Creates a new branch called branch-B

## git checkout main
## git merge branch-A
### Merges the branch-A branch into the main branch

## git checkout main
## git merge branch-B
### Merges the branch-B branch into the main branch

## git add README.md
## git commit -m "Resolved merge conflict between branch-A and branch-B"
### Adds the file README.md and commits the changes with a meaningful commit message

## git branch -m branch-A feature-A
### Renames the branch-A branch to feature-A

## git branch -d feature-login
### Deletes the feature-login branch

# Advaced Git Operations

## echo "Temporary work" >> temp.md
### Adds the text "Temporary work" to the end of the file temp.md

## git stash
### Saves the changes to the file temp.md in a temporary stash

## git stash list
### Lists the stashes

## git stash apply
### Applies the stash to the working directory

## git stash drop
### Drops the stash

# Rewriting History with Interactive Rebase

# Create multiple commits

## echo "Commit 1" > file1.txt && git add file1.txt && git commit -m "Commit 1"
## echo "Commit 2" > file2.txt && git add file2.txt && git commit -m "Commit 2"
## echo "Commit 3" > file3.txt && git add file3.txt && git commit -m "Commit 3"
### 

## git rebase -i HEAD~3
### Opens an interactive rebase menu

## git checkout -b cherry-pick-example
### Creates a new branch called cherry-pick-example

## git cherry-pick <Commit 1>
### Applies the changes from the specified commit to the current branch

## git tag -a v1.0 -m "Release 1.0 release"
### Creates a new tag called v1.0 with a meaningful commit message

## git push origin v1.0
### only pushes the tag to the remote repository

## git remote add origin <repository-url>
### Adds a new remote repository called origin


## git push origin main
### pushes the changes  to the remote repository


# Forking and Contributing

## git clone <forked-repo-url>
### Clones the forked repository to the local machine

# Create a new branch, make changes, and push

## git checkout -b fix-typo
## echo "Typo fixed" >> README.md
## git add README.md
## git commit -m "Fixed a typo"
## git push origin fix-typo
### Pushes the changes to the remote repository

# Git Ignore

## echo "node-modules/" >> .gitignore
### Adds the node-modules directory to the .gitignore file

## git add . 
### add files and ignred files to the staging area