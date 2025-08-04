---

## **1️⃣1️⃣ Git Tag (`git-tag`)**

---

### **📖 Explanation**

* **Tags** are labels that mark specific commits (often used for releases like `v1.0.0`).
* **Types of Tags:**

  1. **Lightweight Tag** → Simple name pointing to a commit.
  2. **Annotated Tag** → Stores extra info (tagger, message, date).

---

### **🛠 Steps**

#### **1️⃣ Create a lightweight tag**

```bash
git tag v1.0
```

---

#### **2️⃣ Create an annotated tag**

```bash
git tag -a v1.0 -m "Release version 1.0"
```

---

#### **3️⃣ List all tags**

```bash
git tag
```

---

#### **4️⃣ View tag details**

```bash
git show v1.0
```

---

#### **5️⃣ Push a single tag to GitHub**

```bash
git push origin v1.0
```

---

#### **6️⃣ Push all tags to GitHub**

```bash
git push origin --tags
```

---

#### **7️⃣ Delete a tag**

* **Local:**

```bash
git tag -d v1.0
```

* **Remote:**

```bash
git push origin --delete v1.0
```

---

### **📝 Notes for `git-tag`**

```
📌 Git Tag
- Marks specific commits (usually for releases).

🛠 Types:
1. Lightweight: git tag v1.0
2. Annotated: git tag -a v1.0 -m "msg"

🛠 Commands:
- git tag → List tags.
- git show v1.0 → Show tag details.
- git push origin v1.0 → Push single tag.
- git push origin --tags → Push all tags.
- git tag -d v1.0 → Delete local tag.
- git push origin --delete v1.0 → Delete remote tag.

💡 Tip: Use annotated tags for official releases.
```

---
