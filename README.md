# GitHubBasics
Basic Codes in Github

Setting Up Git
bash

# Set up global username and email (one-time setup)
git config --global user.name "YourName"
git config --global user.email "YourEmail@example.com"

# Check current Git settings
git config --list
Basic Commands
Initialize and Clone
bash

# Initialize a new Git repository in a directory
git init

# Clone a repository (creates a local copy)
git clone <repository-url>
Status and Logs
bash

# Show the working tree status
git status

# Show commit logs
git log

# Show a compact view of commit history
git log --oneline
Adding and Committing
bash

# Stage all changes for commit
git add .

# Stage specific files
git add <file1> <file2>

# Commit with a message
git commit -m "Your commit message"

# Combine staging and committing
git commit -a -m "Your commit message"
Branching and Merging
bash

# List all branches
git branch

# Create a new branch
git branch <branch-name>

# Switch to a branch
git checkout <branch-name>

# Create and switch to a new branch
git checkout -b <branch-name>

# Merge a branch into the current branch
git merge <branch-name>

# Delete a branch
git branch -d <branch-name>
Pushing and Pulling
bash

# Push changes to a remote repository
git push <remote> <branch>

# Pull changes from a remote repository
git pull <remote> <branch>

# Set a default remote (e.g., origin) for push
git push -u <remote> <branch>
Remotes
bash

# List all remotes
git remote -v

# Add a new remote
git remote add <name> <url>

# Remove a remote
git remote remove <name>
Stashing Changes
bash

# Stash current changes (temporarily save work)
git stash

# Apply the most recent stash
git stash apply

# List stashed changes
git stash list

# Apply and drop the stash
git stash pop
Viewing Diffs
bash

# View differences between working directory and last commit
git diff

# View differences between staged changes and last commit
git diff --cached

# View differences between two commits
git diff <commit1> <commit2>
Undoing Changes
bash

# Unstage a file (keeps changes in working directory)
git reset <file>

# Undo the last commit (keeps changes in working directory)
git reset --soft HEAD~1

# Undo the last commit (deletes changes)
git reset --hard HEAD~1
Tagging
bash

# Create a new tag
git tag <tag-name>

# Push tags to remote
git push <remote> <tag-name>
________________________________________
GitHub-Specific Commands
Connecting to GitHub
1.	SSH Setup (Recommended)
bash

# Generate SSH key (if not created already)
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

# Start SSH agent and add the SSH key
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
2.	Add SSH Key to GitHub
o	Copy SSH key to clipboard: cat ~/.ssh/id_rsa.pub
o	Paste it in GitHub under Settings > SSH and GPG keys > New SSH key.
Forking and Pull Requests
•	Forking: Fork a repository on GitHub to create your copy.
•	Pull Requests: Submit code for review by opening a pull request from your branch to the main branch of the repository.
________________________________________
Common Flags and Shortcuts
bash

# Shortcuts for Git commands
git status -s        # Short status output
git log --oneline    # Single-line log output
git add -A           # Add all changes
git commit -am "msg" # Add and commit all files with a message

