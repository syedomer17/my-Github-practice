---

## **8️⃣ Create Branches (`create-branches`)**

---

### **📖 Explanation**

Branches let you work on features or fixes **without affecting the main branch**.
You can:

* Create new branches.
* Switch between them.
* Delete when no longer needed.

---

### **🛠 Steps**

#### **1️⃣ Create a new branch**

```bash
git branch feature-login
```

#### **2️⃣ Switch to a branch**

```bash
git checkout feature-login
```

*(Shortcut for create + switch)*

```bash
git checkout -b feature-login
```

#### **3️⃣ View all branches**

```bash
git branch
```

#### **4️⃣ Delete a branch**

* **Local delete:**

```bash
git branch -d feature-login     # Safe delete (if merged)
git branch -D feature-login     # Force delete
```

* **Remote delete:**

```bash
git push origin --delete feature-login
```

#### **5️⃣ Rename a branch**

```bash
git branch -m old-name new-name
```

---

### **📝 Notes for `create-branches`**

```
📌 Git Branches
- Branches isolate work (features, fixes) from main code.

🛠 Commands:
1. git branch <name> → Create branch.
2. git checkout <name> → Switch branch.
3. git checkout -b <name> → Create & switch.
4. git branch → List branches.
5. git branch -d <name> → Delete local branch.
6. git push origin --delete <name> → Delete remote branch.
7. git branch -m old new → Rename branch.

💡 Tip: Always merge or rebase before deleting branches.
```

---