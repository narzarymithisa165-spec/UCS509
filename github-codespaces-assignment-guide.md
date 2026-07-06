


# How to Submit Your Coding Assignments via GitHub (No Local Install Needed)

Everything below happens in your browser using **GitHub Codespaces** — a full coding environment that runs in the cloud. You don't need to install Python, Git, or anything else on your computer.

Follow these steps once, and every future assignment will follow the same pattern.

---

## Part 1: One-Time Setup

### Step 1: Create a GitHub account
Go to [github.com](https://github.com) and sign up. Use your real name and roll number — your instructor needs to identify you. You can login using Institute Gmail Account also.

### Step 2: Send your instructor your GitHub username
Class representative will compile the list of usernames and submit to the instructor. They'll need it to be added as a collaborator on your repos.

That's it — no software to install.

---

## Part 2: Assignment 1 — Array Basics

**Task:** Write a program that takes an array of numbers and:
1. Finds the smallest number
2. Finds the largest number
3. Reverses the array
4. Finds duplicate values

### Step 1: Create a new repository
1. Log in to GitHub, click the **+** icon (top right) → **New repository**
2. Name it exactly: `UCS509_rollnumber` 
3. Set visibility to **Private**
4. Check **"Add a README file"**
5. Click **Create repository**



### Step 2: Add your instructor as a collaborator
1. In your new repo, go to **Settings** → **Collaborators**
2. Click **Add people**
3. Enter your instructor's GitHub username     (**Bikram-cit**)
4. Send the invite

> Without this step, your instructor cannot see a private repo, even if they know it exists.

### Step 3: Open a Codespace
1. On your repo's main page, click the green **Code** button
2. Click the **Codespaces** tab
3. Click **Create codespace on main**
4. Wait 30–60 seconds — a full VS Code environment loads in your browser, with a file explorer on the left and a terminal at the bottom

This is now your coding environment. Nothing to install — it already has Python (or whatever language runtime you need) built in.

### Step 4: Create your solution file
1. In the file explorer (left sidebar), right-click the folder → **New File**
2. Name it `arrays.c` (or `.js`, `.java` — use whatever language your instructor specified)
3. Write your code in the editor. 


### Step 5: Run your code in the built-in terminal
At the bottom of the Codespace window, click **Terminal** (or press `` Ctrl+` ``), then type:
```bash
gcc arrays.c -o main
./main
```
Check the output matches what you expect. Fix and re-run as needed.

### Step 6: Save your work back to GitHub (commit + push)
This is done entirely with clicks — no typed Git commands required.

1. Click the **Source Control** icon in the left sidebar (looks like a branching icon)
2. You'll see your changed files listed
3. Type a short message in the box at the top describing what you did, e.g. `Implement array smallest, largest, reverse, duplicates`
4. Click the **✓ Commit** button
5. Click **Sync Changes** (or **Push**) to upload it to GitHub

### Step 7: Verify on GitHub
Go back to your repository page (github.com, not the Codespace) and confirm `arrays.py` appears with your latest commit message.

### Step 8: Commit early and often (recommended)
Repeat Step 6 each time you finish a function, not just at the end. This gives you a safety net and shows your working process over time.

### Step 9: Stop your Codespace when done
Codespaces use free monthly hours. When you're finished for the session:
1. Click the **Codespaces** menu (bottom-left corner, or via the Command Palette)
2. Choose **Stop Codespace**

It saves your work either way, but stopping it preserves your free quota. Idle Codespaces auto-stop after a period of inactivity regardless.

---

## Deadline Rule
Your submission is whatever is in your repository at the deadline time. You can check your commit history any time from the **Source Control** panel, or on the GitHub repo page under "commits." Late pushes are visible via timestamp — don't push after the cutoff expecting it to go unnoticed.

---

## Quick Reference

| Action | Where |
|---|---|
| Open your coding environment | Repo page → **Code** → **Codespaces** → **Create codespace on main** |
| Run your code | Terminal panel inside Codespace: `gcc arrays.c -o main` |
| Save + upload your work | Source Control panel → write message → **Commit** → **Sync Changes** |
| Check submission history | Repo page → **Commits** |
| Resume work later | Repo page → **Code** → **Codespaces** → click your existing codespace |

---

## Common Problems

**I don't see a "Codespaces" tab under the Code button**
→ Make sure you're logged in and it's your own repo (or one you're a collaborator on). Codespaces is enabled by default for personal accounts.

**"Sync Changes" button isn't showing up / nothing to commit**
→ Make sure you actually saved the file first (`Ctrl+S` / `Cmd+S`). Unsaved changes won't show in Source Control.

**My Codespace disappeared or says it stopped**
→ Codespaces auto-stop after ~30 minutes idle to save quota, but your files are preserved. Just click **Create codespace** again on the same repo, or select the existing one from the Codespaces list — it will resume with your files intact.

**I'm running low on free Codespace hours**
→ Always click **Stop Codespace** when you're done working instead of just closing the tab — an open-but-unused Codespace can keep burning hours until it auto-stops.

**Instructor says they can't see my repo**
→ Check Settings → Collaborators — confirm the invite was accepted and the repo is private+shared, not just private.
