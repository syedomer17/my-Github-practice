---

## **🔟 Git Stash (`git-stash`)**

---

### **📖 Explanation**

* `git stash` saves **uncommitted changes** temporarily so you can work on something else.
* Your working directory becomes clean, and you can bring changes back later.

---

### **🛠 Steps**

#### **1️⃣ Save changes to stash**

```bash
git stash
```

*(Stashes tracked file changes)*

To stash untracked files too:

```bash
git stash -u
```

---

#### **2️⃣ View all stashes**

```bash
git stash list
```

---

#### **3️⃣ Apply stash (keep in stash)**

```bash
git stash apply stash@{0}
```

---

#### **4️⃣ Pop stash (apply and remove from stash)**

```bash
git stash pop
```

---

#### **5️⃣ Drop stash (remove specific stash)**

```bash
git stash drop stash@{0}
```

---

#### **6️⃣ Clear all stashes**

```bash
git stash clear
```

---

### **📝 Notes for `git-stash`**

```
📌 Git Stash
- Temporarily saves uncommitted changes.

🛠 Commands:
1. git stash → Save changes.
2. git stash -u → Save untracked + tracked files.
3. git stash list → View stashes.
4. git stash apply stash@{n} → Apply stash (keep it).
5. git stash pop → Apply & remove stash.
6. git stash drop stash@{n} → Delete stash.
7. git stash clear → Remove all stashes.

💡 Tip: Stash is useful before pulling or switching branches.
```

---