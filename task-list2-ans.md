# Git Basics

### ** Install Git from git-scm.com **

# **configure Your global Git settings:**

### git config --global user.name "Your Name"
### ANS:specifies the name that will be shown in commit history

### git config --global user.mail "your-email@example.com"
### ANS:specifies the email that will be shown in commit history

### git config --list
### ANS:shows all configurations

### mkdir MyProject
### ANS:makes a directory called MyProject
### cd MyProject
### ANS:changes to the directory MyProject
### git init
### ANS:initializes a new git repository in the current directory

# Basic WorkFlow
# ** Creating and Commiting Files **

## 1. Create a File:

### echo "Hello Git " > file1.txt
### ANS:creates a new file named file1.txt and adds a text "Hello Git"

## 2. Stage and Commit the file:

### git add file1.txt
### ANS:adds the file1 to the staging area

### git commit -m "Initial commit: Added file1.txt"
### ANS:commits the file1.txt with a message "Initial commit : Added file1.txt"

## Task4: Viewing Changes

# ** Modify the file:

### echo "Git is awesome!" >> file1.txt
### ANS:modifies the file1.txt by adding new line "Git is awesome!"

# **check file status an diferences**

### git status
### ANS: shows the status of the repository,inclding modified files

### git diff
### ANS:Shows the difference between the last commit and the current state of the file

## TASK5: Undoing Changes:

# **Unstage a staged Fie:**

### git reset file1.txt
### ANS:Unstage the file1.txt

### git checkout -- file1.txt
### ANS:file1.txt ko revert karta hai staging area se

# PART3: Branching and Merging

# TASK6: Branch Management

# 1. Create a branch and switch to it:

### git checkout -b feature-branch
### fetaure-branch name ki nai branch banati hai aur us pr switch karta hai

### git branch
### ANS: repository ki sari branch dikhati hai

### git branch -m feature-branch feature-enhanced
### ANS:feature-branch ka name change karke feature-enhanced kar deti hai


# task7: Merging Branches

# 1. Merge a feature-enhanced into the main branch:

### git checkout main
### main branch me switch karta hai

### git merge feature-enhanced
### ANS: feature-enhanced branch ko main branch ke sath merge karta hai

# TASK8: Handing Merge Conflicts
# 1.Create two conflicting branches and resolve a confict  manualy

### git merge <branch-name>
### AN: merge conflict ho jata hai. matlab dono branch same file me change hai aur merge karna hai to conflict aata hai


# 2.USE;

### git add <resolved-file>
### ANS: resolved file ko staging area me add karta hai

### git commit
### ANS:resolved file ko commit karta hai

# Part4: Remote Repositoris

# TASK9: Remote setup

# 1. Add a remote repository:
### git remote add origin <repository-url>
### ANS: remte repository ko origin name se add karta hai

# 2.verify the remote
### git remote -v
### ANS: remote repository ki details show karta hai

# TASK10:Push and Pull
# 1.push changes to the remote repository:
### git push -u origin main
### ANS: local main branch ko remote repository ke main ranch me pushbh karta hai

### git pull origin main
### ANS: remote reposiory ke main branch ko local main branch me pull karta hai


# TASK11: Clonning a Repo
# 1. Clone a remote repository:
### git clone <repository-url>
### ANS: remote repository ko local machine par clone karta hai
