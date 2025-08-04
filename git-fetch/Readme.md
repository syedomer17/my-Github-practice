---

## **5️⃣ Git Fetch (`git-fetch`)**

---

### **📖 Explanation**

* `git fetch` **downloads changes** from the remote repository but does **not** automatically merge them into your current branch.
* It’s a safe way to check what’s changed on remote before updating your local code.

---

### **🛠 Steps**

#### **1️⃣ Fetch all branches**

```bash
git fetch
```

#### **2️⃣ Fetch from a specific remote**

```bash
git fetch origin
```

#### **3️⃣ View fetched changes**

```bash
git log origin/main
```

#### **4️⃣ Merge manually (if needed)**

```bash
git merge origin/main
```

---

### **📝 Notes for `git-fetch`**

```
📌 Git Fetch
- Downloads commits, branches, and tags from remote.
- Does NOT merge into local branch automatically.

🛠 Commands:
1. git fetch → Fetch all changes.
2. git fetch origin → Fetch from specific remote.
3. git log origin/main → View fetched changes.
4. git merge origin/main → Merge fetched changes manually.

💡 Tip: Use fetch when you want to review changes before merging.
```

---