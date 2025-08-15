# 📚 GitHub Learnings – All-in-One Git Commands

A quick reference of the most-used Git commands for daily development.

```bash
# -------------------------------
# 1️⃣ Setup & Configuration
# -------------------------------
git config --global user.name "Charan"
git config --global user.email "charansaiakkineni123@gmail.com"
git config --list

# -------------------------------
# 2️⃣ Starting a Repository
# -------------------------------
git init                                   # Create a new repo in current folder
git clone <repo-url>                       # Clone an existing repo

# -------------------------------
# 3️⃣ Basic Workflow
# -------------------------------
git status                                 # Check repo status
git add <file>                             # Add single file
git add .                                  # Add all files
git commit -m "Meaningful commit message"  # Commit changes
git log                                    # View commit history

# -------------------------------
# 4️⃣ Branching
# -------------------------------
git branch <branch-name>                   # Create branch
git checkout <branch-name>                 # Switch to branch
git checkout -b <branch-name>              # Create + switch
git checkout main                          # Switch to main
git merge <branch-name>                    # Merge branch into main

# -------------------------------
# 5️⃣ Remote Operations
# -------------------------------
git remote add origin <repo-url>           # Link local repo to GitHub
git push -u origin main                    # Push first time
git push                                   # Push changes
git pull origin main                       # Pull latest changes

# -------------------------------
# 6️⃣ Undoing Changes
# -------------------------------
git reset <file>                           # Unstage file
git checkout -- <file>                     # Discard changes
git reset --soft HEAD~1                    # Undo last commit, keep changes
git reset --hard HEAD~1                    # Undo last commit, discard changes

# -------------------------------
# 7️⃣ Extra Useful Commands
# -------------------------------
git diff                                   # Show differences
git remote -v                              # View remote repos
git branch -d <branch-name>                # Delete branch
git stash                                  # Stash changes temporarily
git stash pop                              # Reapply stashed changes
