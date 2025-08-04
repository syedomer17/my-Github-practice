---

### **1️⃣ GitHub Repository Setup (`github-repo-setup`)**

This is the very first step in any Git project.

---

#### **📖 Explanation**

A Git repository setup means:

* Initializing a local Git repo.
* Linking it to a remote GitHub repo.
* Making your first commit and push.

---

#### **🛠 Steps**

1. **Initialize Git in a folder**

```bash
git init
```

*(Creates a `.git` folder which tracks changes)*

2. **Check Git status**

```bash
git status
```

3. **Add remote GitHub repository**

```bash
git remote add origin <repo-URL>
```

4. **Add files to staging**

```bash
git add .
```

5. **Commit changes**

```bash
git commit -m "Initial commit"
```

6. **Push to GitHub**

```bash
git push -u origin main
```

---

#### **📝 Notes for `github-repo-setup`**

```
📌 GitHub Repository Setup
1. git init → Initialize Git in local folder.
2. git remote add origin <URL> → Link local repo to GitHub.
3. git add . → Stage all changes.
4. git commit -m "msg" → Save staged changes.
5. git push -u origin main → Push to GitHub.

💡 Tip: Replace 'main' with 'master' if your default branch is named master.
```

---
