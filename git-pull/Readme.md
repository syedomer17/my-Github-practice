---

## **4️⃣ Git Pull (`git-pull`)**

---

### **📖 Explanation**

`git pull` updates your local branch with changes from the remote repository.
It is basically:

```
git pull = git fetch + git merge
```

* **Fetch** downloads changes from remote.
* **Merge** applies them to your current branch.

---

### **🛠 Steps**

#### **1️⃣ Pull latest changes**

```bash
git pull origin main
```

#### **2️⃣ Pull for current branch (after upstream set)**

```bash
git pull
```

#### **3️⃣ Pull with rebase** *(to avoid unnecessary merge commits)*

```bash
git pull --rebase
```

---

### **📝 Notes for `git-pull`**

```
📌 Git Pull
- Updates local branch with remote changes.
- Shortcut for 'git fetch' + 'git merge'.

🛠 Commands:
1. git pull origin main → Pull specific branch.
2. git pull → Pull current branch (upstream must be set).
3. git pull --rebase → Pull without creating extra merge commits.

💡 Tip: Use 'git stash' if you have uncommitted changes before pulling.
```

---