---

## **2️⃣ Git Stages (`git-stages`)**

---

### **📖 Explanation**

In Git, there are **three stages** where your files can exist:

1. **Working Directory** → Your local files (not yet tracked by Git).
2. **Staging Area (Index)** → Files marked for commit (`git add`).
3. **Repository (Commit History)** → Files saved permanently (`git commit`).

---

### **🛠 Steps**

1. **Check file status**

```bash
git status
```

2. **Move files from Working Directory → Staging Area**

```bash
git add <filename>     # Add single file
git add .              # Add all files
```

3. **Commit files from Staging Area → Repository**

```bash
git commit -m "Your commit message"
```

4. **View commit history**

```bash
git log
```

---

### **📝 Notes for `git-stages`**

```
📌 Git Stages
1. Working Directory → Untracked/Modified files.
2. Staging Area → Files added via 'git add'.
3. Repository → Files saved with 'git commit'.

🛠 Commands:
- git status → View file status.
- git add <file> / git add . → Stage changes.
- git commit -m "msg" → Commit changes to repo.
- git log → View commit history.

💡 Tip: Use 'git diff' to see unstaged changes.

