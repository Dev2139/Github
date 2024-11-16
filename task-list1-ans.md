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

