# 📘 Git & GitHub Commands Notes

A complete guide to essential Git & GitHub commands with explanations and steps for each.

---

## **1️⃣ GitHub Repository Setup (`github-repo-setup`)**
```bash
git init                       # Initialize Git in local folder
git remote add origin <URL>    # Link to GitHub repo
git add .                      # Stage all changes
git commit -m "Initial commit" # Commit changes
git push -u origin main        # Push to GitHub
```
💡 Tip: Replace `main` with `master` if needed.

---

## **2️⃣ Git Stages (`git-stages`)**
```bash
git status              # Check file status
git add <file> / git add .   # Stage files
git commit -m "msg"    # Commit changes
git log                # View commit history
```
Stages:
- **Working Directory** → Local changes
- **Staging Area** → Files marked for commit
- **Repository** → Committed files

---

## **3️⃣ Git Push (`git-push`)**
```bash
git push -u origin main   # First-time push
git push                  # Normal push
git push --force          # Force push (⚠ Overwrites history)
```
💡 Always pull before pushing to avoid conflicts.

---

## **4️⃣ Git Pull (`git-pull`)**
```bash
git pull origin main    # Pull specific branch
git pull                # Pull current branch
git pull --rebase       # Rebase to avoid merge commits
```
💡 Pull = Fetch + Merge.

---

## **5️⃣ Git Fetch (`git-fetch`)**
```bash
git fetch               # Fetch all branches
git fetch origin        # Fetch from specific remote
git log origin/main     # View fetched commits
git merge origin/main   # Merge manually if needed
```
💡 Fetch downloads changes but does NOT merge.

---

## **6️⃣ Git Merge (`git-merge`)**
```bash
git checkout main
git merge feature-branch   # Merge feature branch into main
```
Types:
- **Fast-forward** → Moves pointer forward.
- **3-way merge** → Creates merge commit.
- **Conflict** → Resolve manually.

---

## **7️⃣ Git Rebase (`git-rebase`)**
```bash
git checkout feature-branch
git rebase main           # Rebase onto main
git rebase --continue     # Continue after fixing conflicts
git rebase --abort        # Cancel rebase
```
💡 Rebase creates cleaner history than merge.

---

## **8️⃣ Create Branches (`create-branches`)**
```bash
git branch feature-login              # Create branch
git checkout feature-login            # Switch branch
git checkout -b feature-login         # Create + switch
git branch -d feature-login           # Delete local branch
git push origin --delete feature-login# Delete remote branch
git branch -m old-name new-name       # Rename branch
```

---

## **9️⃣ Git Conflicts (`git-conflicts`)**
Conflict markers in file:
```plaintext
<<<<<<< HEAD
Code from current branch
=======
Code from merging branch
>>>>>>> feature
```
Resolve by editing, then:
```bash
git add <file>
git commit
```

---

## **🔟 Git Stash (`git-stash`)**
```bash
git stash           # Save changes
git stash -u        # Save untracked files too
git stash list      # List stashes
git stash apply     # Apply stash (keep it)
git stash pop       # Apply & remove stash
git stash drop      # Remove specific stash
git stash clear     # Remove all stashes
```

---

## **1️⃣1️⃣ Git Tag (`git-tag`)**
```bash
git tag v1.0                         # Lightweight tag
git tag -a v1.0 -m "Release v1.0"    # Annotated tag
git tag                             # List tags
git show v1.0                       # View tag details
git push origin v1.0                # Push single tag
git push origin --tags              # Push all tags
git tag -d v1.0                     # Delete local tag
git push origin --delete v1.0       # Delete remote tag
```
💡 Use annotated tags for releases.

---

## **1️⃣2️⃣ Delete File & Remove File (`delete-file` & `remove-file`)**
```bash
# Delete file completely (repo + local)
git rm filename.txt
git commit -m "Delete file"

# Remove file from tracking (keep local)
git rm --cached filename.txt
git commit -m "Remove from tracking"

# Delete folder
git rm -r foldername
```
💡 Add to `.gitignore` to prevent tracking in future.

---

## ✅ Summary
This README covers:
- Repository setup
- Staging & committing
- Push, pull, fetch
- Merge vs rebase
- Branching
- Conflict resolution
- Stash & tag
- Deleting/removing files

🎯 **Use this as a quick reference for Git & GitHub commands.**
