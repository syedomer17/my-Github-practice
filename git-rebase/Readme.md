---

## **7️⃣ Git Rebase (`git-rebase`)**

---

### **📖 Explanation**

* `git rebase` moves or reapplies commits **on top of another branch**.
* It keeps a **linear commit history** (no extra merge commits).
* It’s like saying: *“Pretend I started my branch from the latest commit of main.”*

---

### **🛠 Steps**

#### **1️⃣ Rebase feature branch onto main**

```bash
git checkout feature-branch
git rebase main
```

#### **2️⃣ Continue after conflicts**

If conflicts occur during rebase:

```bash
# Fix conflicts in files
git add <resolved-file>
git rebase --continue
```

#### **3️⃣ Abort rebase**

```bash
git rebase --abort
```

---

### **🔍 Merge vs Rebase (Key Difference)**

* **Merge**: Keeps history of both branches (can be messy).
* **Rebase**: Moves commits to a clean line (linear history).

Example:

```
Merge history:    A---B---C (main)
                  \       \
                   D---E---M (feature)

Rebase history:   A---B---C---D'---E' (feature rebased)
```

---

### **📝 Notes for `git-rebase`**

```
📌 Git Rebase
- Moves commits from one branch on top of another.
- Creates linear history (no extra merge commits).

🛠 Commands:
1. git checkout feature-branch
2. git rebase main → Rebase onto main.
3. git rebase --continue → Continue after fixing conflicts.
4. git rebase --abort → Cancel rebase.

💡 Tip: Use rebase for clean history; merge for preserving exact commit history.
```

---