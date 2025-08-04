---

## **9️⃣ Git Conflicts (`git-conflicts`)**

---

### **📖 Explanation**

* A **merge conflict** happens when **two branches modify the same part of the same file** and Git can’t decide which change to keep.
* You must manually edit the file to resolve it.

---

### **🛠 Steps**

#### **1️⃣ Create a simple conflict**

Example:

```bash
# On branch main
echo "Hello from Main" > hello.txt
git add hello.txt
git commit -m "Main change"

# Create new branch
git checkout -b feature
echo "Hello from Feature" > hello.txt
git add hello.txt
git commit -m "Feature change"

# Switch back to main and make change
git checkout main
echo "Hello from Main Branch" > hello.txt
git add hello.txt
git commit -m "Main second change"

# Merge feature (conflict will appear)
git merge feature
```

---

#### **2️⃣ Resolve conflict**

When conflict appears, file will look like:

```plaintext
<<<<<<< HEAD
Hello from Main Branch
=======
Hello from Feature
>>>>>>> feature
```

* **Choose** which code to keep (or combine both).
* Remove conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`).

---

#### **3️⃣ Mark resolved and commit**

```bash
git add hello.txt
git commit
```

---

### **📝 Notes for `git-conflicts`**

```
📌 Git Conflicts
- Occur when two branches edit the same part of a file.
- Must be resolved manually.

🛠 Conflict Workflow:
1. Merge/rebase causes conflict.
2. Open conflicted file.
3. Edit to keep desired code (remove markers).
4. git add <file>
5. git commit → Conflict resolved.

💡 Tip: Use VS Code or tools like 'git mergetool' for easier resolution.
```

---