---

## **6️⃣ Git Merge (`git-merge`)**

---

### **📖 Explanation**

`git merge` combines changes from one branch into another.
There are **two main types** of merge:

1. **Fast-forward merge** → Happens when no new commits exist in the target branch.
2. **3-way merge** → Happens when both branches have commits; Git creates a merge commit.

---

### **🛠 Steps**

#### **1️⃣ Merge another branch into current branch**

```bash
git checkout main       # Switch to target branch
git merge feature-branch
```

#### **2️⃣ Fast-forward merge example**

* If `main` has no new commits since `feature-branch` started:

```bash
git merge feature-branch
# Simply moves the pointer ahead (no merge commit).
```

#### **3️⃣ 3-way merge example**

* If `main` and `feature-branch` both have commits:

```bash
git merge feature-branch
# Creates a merge commit.
```

#### **4️⃣ Merge with conflicts**

* If the same file lines are changed in both branches, Git will show a conflict.
* Resolve manually, then:

```bash
git add <resolved-file>
git commit
```

---

### **📝 Notes for `git-merge`**

```
📌 Git Merge
- Combines changes from one branch into another.

🛠 Commands:
1. git checkout main
2. git merge <branch> → Merge branch into main.

🛠 Types of Merge:
- Fast-forward: Moves pointer ahead, no merge commit.
- 3-way merge: Creates merge commit if both branches changed.
- Conflicts: Must be resolved manually before committing.

💡 Tip: Always pull latest changes before merging.
```

---
