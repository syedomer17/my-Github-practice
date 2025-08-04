---

## **1️⃣2️⃣ Delete File (`delete-file`) & Remove File (`remove-file`)**

---

### **📖 Explanation**

* Both deal with deleting files, but the approach differs:

  * **`git rm`** → Deletes file from working directory **and** staging area.
  * **Manual delete + `git rm --cached`** → Removes file only from Git tracking but keeps it locally.

---

### **🛠 Steps**

#### **1️⃣ Delete a file completely (from repo & local)**

```bash
git rm filename.txt
git commit -m "Delete filename.txt"
git push
```

---

#### **2️⃣ Remove file only from Git tracking (keep file locally)**

```bash
git rm --cached filename.txt
git commit -m "Remove filename.txt from tracking"
git push
```

---

#### **3️⃣ Delete multiple files**

```bash
git rm file1.txt file2.txt
```

---

#### **4️⃣ Delete folder**

```bash
git rm -r foldername
```

---

### **📝 Notes for `delete-file` & `remove-file`**

```
📌 Delete vs Remove in Git

🛠 Delete file completely:
- git rm filename.txt
- Removes file from repo & local.
- Commit & push to update remote.

🛠 Remove file only from tracking (keep local):
- git rm --cached filename.txt
- File stays on disk but removed from Git.
- Commit & push.

💡 Tip: Use .gitignore to prevent Git from tracking files in the future.
```

---