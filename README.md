
# Git Commands Cheat Sheet

This README provides essential Git commands for working with GitHub using Git CMD (Command Prompt), along with brief explanations.

---

## Setup & Config

Sets your global Git username (used for all repositories).
```bash
git config --global user.name "Your Name"
```

Sets your global email.
```bash
git config --global user.email "your_email@example.com"
```

Check local or global Git username.
```bash
git config user.name
git config --global user.name
```

List all config values (local or global).
```bash
git config --list
git config --global --list
```


---

## Create / Clone Repos

```bash
git init
```
Initialize a new Git repository.


```bash
git clone https://github.com/username/repo.git
```
Clone an existing repository from GitHub.

---

## Basic Workflow

```bash
git status
```
Check the status of your working directory and staging area.

```bash
git add filename
git add .
```
Stage file(s) or all files for commit.

```bash
git commit -m "Your commit message"
```
Commit staged changes.

```bash
git push origin branch_name
```
Push commits to GitHub on specified branch.

```bash
git pull origin branch_name
```
Pull latest changes from GitHub.

---

## Branching

```bash
git branch
```
List local branches.

```bash
git branch new_branch
```
Create a new branch.

```bash
git checkout new_branch
```
Switch to a branch.

```bash
git checkout -b new_branch
```
Create and switch to a new branch.

```bash
git merge branch_name
```
Merge specified branch into current branch.

---

## Undo / Reset

```bash
git restore filename
```
Discard changes in working directory (Git 2.23+).

```bash
git reset HEAD filename
```
Unstage a file.

```bash
git reset --hard
```
Reset all files to last commit (warning: destructive).

---

## Remove / Rename

```bash
git rm filename
```
Delete a file and stage the removal.

```bash
git mv oldname newname
```
Rename a file and stage the rename.

---

## Logs

```bash
git log
```
Show commit history.

```bash
git log --oneline --graph --all
```
Compact graph of all commits.

---

## Authentication

```bash
git push https://username@github.com/username/repo.git
```
Push with username (use PAT/token in place of password).

---

## Change Global Username / Email

```bash
git config --global user.name "New Name"
git config --global user.email "new_email@example.com"
```
Update global Git identity.

---

## Additional Useful Commands

```bash
git stash
```
Temporarily save changes without committing.

```bash
git stash pop
```
Apply stashed changes.

```bash
git remote -v
```
Show remote URLs.

```bash
git fetch
```
Download changes without merging.

```bash
git diff
```
See unstaged changes.

```bash
git show commit_id
```
Show details of a specific commit.

## 📬 Contact

Maintained by **Balaji Kudumu**  
If you use this project in your research, please give appropriate credit.

---

## 📄 License

MIT License - see `LICENSE` file for details.
---

**Tip:** Use SSH or Personal Access Tokens (PAT) for GitHub authentication to avoid password issues.
