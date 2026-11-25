# small-example-text-files
program 1:❤
# Step 1: Create a new project directory and move into it
mkdir gitlab
cd gitlab

# Step 2: Initialize an empty Git repository inside the folder
git init

# Step 3: Create a new text file with initial content
echo "Hello Git" > my_file.txt

# Step 4: Add the file to the staging area
git add my_file.txt

# Step 5: Commit the staged file permanently to the repository history
git commit -m "Initial commit"

program 2🥇
# Step 1: Create a fresh directory and initialize a Git repository
mkdir gitlab
cd gitlab
git init

# Step 2: Create and commit an initial file on the main branch
echo "Hello Git" > my_file.txt
git add my_file.txt
git commit -m "Initial commit"

# Step 3: Verify you are on main, then create and switch to feature-branch
git checkout main
git checkout -b feature-branch

# Step 4: Append new content to the file and commit it on feature-branch
echo "Feature branch content" >> my_file.txt
git add .
git commit -m "Add feature branch content"

# Step 5: Switch back to main and merge feature-branch into main
git checkout main
git merge feature-branch

program3 🥉
# Step 1: Create a directory for cloning and navigate into it
mkdir git_clone
cd git_clone

# Step 2: Clone the remote repository from GitHub onto the local system
git clone https://github.com/cdepillabout/small-example-text-files.git

# Step 3: Move inside the cloned repository directory
cd small-example-text-files

# Step 4: List all local branches and check the active branch
git branch

# Step 5: Fetch the latest metadata and commits from the remote origin
git fetch origin

# Step 6: Check the working tree and branch synchronization status
git status

 program 4🙂
 # Step 1: Create a fresh workspace and clone your GitHub repository
mkdir git_clone
cd git_clone
git clone https://github.com/CYBER-CORE-DEV/small-example-text-files.git
cd small-example-text-files

# Step 2: Check the active branch, fetch origin, and verify clean status
git branch
git fetch origin
git status

# Step 3: Modify or create a local file and stage the change
echo "My local change" >> my_file.txt
git add my_file.txt

# Step 4: Commit the local change to your local repository
git commit -m "Add local change"

# Step 5: Rebase local commits cleanly on top of origin/main
git rebase origin/main

# Step 6: Push the rebased commits to the remote main branch on GitHub
git push origin main

program 5⏰
# Step 1: Create a fresh repository and record an initial commit on main
mkdir gitlab
cd gitlab
git init
echo "Hello Git" > my_file.txt
git add my_file.txt
git commit -m "Initial commit"

# Step 2: Connect the local repository to your remote GitHub repository
git remote add origin https://github.com/CYBER-CORE-DEV/gitlab.git

# Step 3: Make uncommitted edits to the file and save them to the stash
echo "New changes" >> my_file.txt
git stash save "My changes"

# Step 4: Create and switch to a new target branch
git checkout -b target-branch

# Step 5: Reapply the stashed edits onto target-branch
git stash apply

# Step 6: Stage, commit, and push target-branch to the remote repository
git add my_file.txt
git commit -m "Apply stashed changes"
git push -u origin target-branch

program 6🥉
# Step 1: Create a fresh repository and record an initial commit on main
mkdir gitlab
cd gitlab
git init
echo "Hello Git" > my_file.txt
git add my_file.txt
git commit -m "Initial commit"

# Step 2: Create a feature branch, update the file, and commit the change
git checkout -b feature-branch
echo "Feature branch content" >> my_file.txt
git add my_file.txt
git commit -m "Add feature branch content"

# Step 3: Switch back to the main branch and check working tree status
git checkout main
git status

# Step 4: Merge feature-branch into main with a custom merge message
git merge feature-branch -m "Merge feature branch into main"

program 7⤴️
# Step 1: Create a fresh repository and make an initial commit
mkdir gitlab
cd gitlab
git init
echo "Hello Git v1.0" > my_file.txt
git add my_file.txt
git commit -m "Initial commit for v1.0"

# Step 2: Create a lightweight tag on the current commit
git tag v1.0

# Step 3: Make a second commit and create an annotated tag with a message
echo "Added release features" >> my_file.txt
git add my_file.txt
git commit -m "Update for v1.1"
git tag -a v1.1 -m "Release version 1.1"

# Step 4: List all tags and inspect the annotated tag details
git tag
git show v1.1

# Step 5: Link your GitHub repository and push both commits and tags
git remote add origin https://github.com/CYBER-CORE-DEV/gitlab.git
git push -u origin main
git push origin --tags

# Step 6: Delete an unused local tag (optional tag management)
git tag -d v1.0
