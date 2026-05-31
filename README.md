# Setup documentation

This public repository completes **step 1** of the portfolio application: install the required tools, create a GitHub repo, and document what was done.

---

## Tools I installed

- **[Cursor IDE](https://cursor.com/)** — main editor for the portfolio project (Windows)
- **Claude Code** — Cursor extension (Extensions → search “Claude Code” → Install → sign in)
- **Codex** — Cursor extension (Extensions → search “Codex” → Install → sign in)
- **Git** — for commits and pushes from the terminal
- **GitHub** — public repository hosting ([github.com](https://github.com/))

---

## Steps I completed

| # | Step | What I did |
|---|------|------------|
| 1 | Install Cursor IDE | Downloaded from [cursor.com](https://cursor.com/) and installed on my machine |
| 2 | Add Claude Code | Opened **Extensions** in Cursor, searched for **Claude Code**, installed it, and signed in |
| 3 | Add Codex | Opened **Extensions**, searched for **Codex**, installed it, and signed in |
| 4 | Create a public GitHub repo | Created a new **public** repository on GitHub for this project |
| 5 | Open the repo in Cursor | Cloned/opened this repository in Cursor as my workspace |
| 6 | Create this README | Added this file describing tools, steps, and any issues |
| 7 | Commit and push | Committed `README.md` and pushed to the `main` branch on GitHub |
| 8 | Send the link | Shared the link to this README with the hiring team |

---

## Issues I ran into (and how I fixed them)

### 1. Terminal commands on Windows (PowerShell)

**What happened:** Commands chained with `&&` failed in PowerShell with a parser error.

**Fix:** Used semicolons to run commands in sequence, or ran them one at a time:

```powershell
Set-Location "E:\repos\workspace-init"
git status
```

### 2. Local folder was not a Git repo yet

**What happened:** After creating the repo on GitHub, opening a new folder in Cursor showed `fatal: not a git repository`.

**Fix:** Initialized Git locally and connected it to GitHub:

```powershell
git init
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git add README.md
git commit -m "Add setup documentation"
git push -u origin main
```

*(If the repo was created on GitHub with files already in it, I used `git clone` instead of `git init`.)*

### 3. Extensions needed a separate sign-in

**What happened:** Claude Code and Codex were installed but did not work until I signed in.

**Fix:** Opened each extension after install and completed the sign-in flow in the browser / in-editor prompt.

---

## Repository link for reviewers

- **Repository:** `https://github.com/udeeptimodi/workspace-init`
- **This README on GitHub:** `https://github.com/udeeptimodi/workspace-init/edit/master/README.md`
