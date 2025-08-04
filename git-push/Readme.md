---

## **3️⃣ Git Push (`git-push`)**

---

### **📖 Explanation**

`git push` sends your local commits to a **remote repository** (like GitHub).
There are two common cases:

1. **First-time push** (need to set branch tracking).
2. **Normal push** (just send changes).
3. **Force push** (overwrite remote history — use carefully).

---

### **🛠 Steps**

#### **1️⃣ First-time push**

```bash
git push -u origin main
```

*(The `-u` sets the upstream so next time just `git push` works.)*

#### **2️⃣ Normal push**

```bash
git push
```

#### **3️⃣ Force push** *(⚠ DANGER: overwrites history)*

```bash
git push --force
```

---

### **📝 Notes for `git-push`**

```
📌 Git Push
- Sends local commits to remote repo.

🛠 Commands:
1. First-time push:
   git push -u origin main

2. Normal push:
   git push

3. Force push (⚠ Overwrites remote history):
   git push --force

💡 Tip: Always pull changes before pushing to avoid conflicts.
```

---