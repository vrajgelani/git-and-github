# 🚀 Git & GitHub Setup Guide (Windows/Laptop/Desktop)

A simple, beginner-friendly guide to install Git, connect it to GitHub, and start pushing your projects like a pro.

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)

---

## 📑 Table of Contents

1. [Install Git](#1️⃣-install-git)
2. [Configure Git](#2️⃣-configure-git)
3. [Verify Your Config](#3️⃣-verify-your-config)
4. [Create a Project Folder](#4️⃣-create-a-project-folder)
5. [Create a GitHub Repository](#5️⃣-create-a-github-repository)
6. [Connect Local Folder to GitHub](#6️⃣-connect-local-folder-to-github)
7. [Push Your First Files](#7️⃣-push-your-first-files)
8. [Daily Workflow (Repeat Cycle)](#8️⃣-daily-workflow-repeat-cycle)
9. [Quick Command Cheat Sheet](#-quick-command-cheat-sheet)

---

## 1️⃣ Install Git

Download and install Git for your OS:

🔗 **[https://git-scm.com/downloads](https://git-scm.com/downloads)**

> 💡 During installation, keep the default options selected unless you know what you're changing.

---

## 2️⃣ Configure Git

Open **Git Bash** on your computer, then run these commands one by one.

**Step 1 — Remove any old config (optional, only if reconfiguring):**
```bash
git config --global --unset user.name
git config --global --unset user.email
```

**Step 2 — Add your details:**
```bash
git config --global user.name "vrajgelani"
git config --global user.email "vrajgelani1@gmail.com"

## 3️⃣ Verify Your Config

Check that everything was saved correctly:

```bash
git config --list
```

✅ Look for `user.name` and `user.email` in the output — make sure they match what you entered.

---

## 4️⃣ Create a Project Folder

On your computer, create a folder for your project.

> ✏️ **Example:** `News-Website`

This folder will hold all your project files and will later be linked to GitHub.

---

## 5️⃣ Create a GitHub Repository

| Step | Action |
|------|--------|
| 1 | Go to **[github.com](https://github.com)** and log in |
| 2 | Click the green **New** button on your dashboard |
| 3 | Enter a repo name (e.g. `News-Website`) |
| 4 | Click the green **Create repository** button |

---

## 6️⃣ Connect Local Folder to GitHub

On the new repo page, GitHub shows a line starting with:

```bash
git remote add origin <your-repo-link>
```

📋 **Copy that entire line.**

Now:
1. Open your project folder in **VS Code**
2. Open the terminal → **Terminal menu → New Terminal**
3. Confirm you're in the right folder (the path should end with your folder name, e.g. `.../News-Website>`)
4. Paste the copied command and press **Enter**

---

## 7️⃣ Push Your First Files

Create, edit, or delete files inside your project folder as needed. Then, in the terminal, run:

```bash
git add .
git commit -m "your commit message"
git push origin main
```

> ⚠️ **Note:** Replace `main` with your actual branch name if it's different. Check your current branch with:
> ```bash
> git branch
> ```

---

## 8️⃣ Daily Workflow (Repeat Cycle) 🔄

Every time you make changes to your project, repeat this cycle:

```
✏️ Edit files
   ⬇️
📦 git add .
   ⬇️
💬 git commit -m "message describing your change"
   ⬇️
🚀 git push origin main
   ⬇️
🔁 Repeat
```

---

## 📋 Quick Command Cheat Sheet

| Command | Purpose |
|---------|---------|
| `git config --global user.name "name"` | Set your Git username |
| `git config --global user.email "email"` | Set your Git email |
| `git config --list` | View current Git config |
| `git remote add origin <link>` | Connect local folder to GitHub repo |
| `git add .` | Stage all changed files |
| `git commit -m "message"` | Save changes with a message |
| `git push origin main` | Upload changes to GitHub |
| `git branch` | Check current branch name |

---

### 🎯 Tip
Keep commit messages short and clear — e.g. `"fix navbar bug"` or `"add homepage layout"` — so your project history stays easy to read.

---

⭐ **If this guide helped you, consider starring the repo!**
