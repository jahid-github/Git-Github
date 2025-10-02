# Git-Github

---

# 📚 Complete Git & GitHub Hands-on Course (24 Days)

---

## **Module 1: Introduction (Day 1–2)**

### 1. What is Git?

* Git = Version control system (track changes in code, revert anytime).
* Works **locally** on your computer.

### 2. What is GitHub?

* GitHub = Cloud hosting service for Git repositories.
* Lets you share, collaborate, and deploy projects.

### 3. Install Git

* **Windows** → download from [git-scm.com](https://git-scm.com)
* **Mac/Linux** → already preinstalled (check with `git --version`).

### 4. Configure Git

```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
git config --global core.editor "code --wait"   # if using VS Code
```

✅ **Mini Project:**

* Install Git.
* Create a folder `git-practice`.
* Run `git init` inside it.

---

## **Module 2: Tools & Terms (Day 3)**

* **Git Bash** → Command line for Git.
* **Git GUI/GitKraken/Sourcetree** → Visual Git tools.
* **Important terms:**

  * **Repository (Repo):** Folder with `.git` inside.
  * **Commit:** A snapshot of changes.
  * **Branch:** A separate line of development.
  * **Merge:** Combining two branches.
  * **Push:** Send local commits to GitHub.
  * **Pull:** Fetch new changes from GitHub.
  * **Clone:** Download repo with full history.

✅ **Mini Project:**
Make a note file (`git-terms.md`) where you write these definitions.

---

## **Module 3: Basic Git Commands (Day 4–5)**

```bash
git init                # start a repo
git status              # check file status
git add file.txt        # add specific file
git add .               # add all files
git commit -m "first commit"   # save snapshot
git log                 # see commit history
```

✅ **Mini Project:**

* Create `hello.txt`.
* Add text → `git add hello.txt` → `git commit -m "added hello.txt"`.
* Modify file, commit again.
* Run `git log` to see versions.

---

## **Module 4: GitHub Basics (Day 6)**

1. Create a **GitHub account**.
2. Create a new repo → “hello-world”.
3. Connect local to GitHub:

```bash
git remote add origin https://github.com/yourname/hello-world.git
git branch -M main
git push -u origin main
```

✅ **Mini Project:**

* Push your `hello.txt` project to GitHub.
* View it online.

---

## **Module 5: Clone & Download (Day 7)**

```bash
git clone https://github.com/username/repo.git
git clone https://github.com/username/repo.git my-folder   # into custom folder
```

* **Clone** → full history.
* **Download ZIP** → just files (no Git history).

✅ **Mini Project:**

* Clone your own repo into another folder.
* Check if commits are visible.

---

## **Module 6: Commits & History (Day 8–9)**

```bash
git log --oneline       # short view
git log --stat          # with changes
git log --patch         # full diff
git log --graph --oneline --all
git checkout <commit-hash>   # go to old version
```

✅ **Mini Project:**

* Make 3 commits.
* Use `git log` with different flags.
* Switch back to commit 1 → then return to `main`.

---

## **Module 7: .gitignore (Day 10)**

* Create `.gitignore` file:

```
*.log
*.tmp
node_modules/
.DS_Store
```

```bash
git add .gitignore
git commit -m "added gitignore"
```

✅ **Mini Project:**

* Add `test.log`.
* Run `git status` → it won’t show up.

---

## **Module 8: Forking & Collaboration (Day 11)**

* **Fork** = copy of repo into your account.
* **Clone** = copy to your computer.

✅ **Mini Project:**

* Fork any repo from GitHub.
* Clone it to your computer.

---

## **Module 9: File Status & Differences (Day 12–13)**

```bash
git status
git diff
git diff --staged
git diff <commit1> <commit2>
```

✅ **Mini Project:**

* Modify `hello.txt`.
* Compare unstaged vs staged diff.

---

## **Module 10: Staging Control (Day 14)**

```bash
git add file1.txt
git reset file1.txt     # remove from stage
git add .               # add all files
git reset               # unstage all
```

✅ **Mini Project:**

* Practice staging/un-staging multiple files.

---

## **Module 11: HEAD & Tags (Day 15–16)**

```bash
git show HEAD
git checkout HEAD~1
git tag v1.0
git push origin v1.0
git tag -d v1.0
git push origin --delete v1.0
```

✅ **Mini Project:**

* Tag your first working version as `v1.0`.

---

## **Module 12: Remotes & Undo (Day 17–18)**

```bash
git remote -v
git remote add origin <url>
git remote rename origin upstream
git remote remove origin
git reset --soft HEAD~1
git reset --hard HEAD~1
```

✅ **Mini Project:**

* Make 3 commits, undo the last one with `--soft` and `--hard`.

---

## **Module 13: Branching & Merging (Day 19–20)**

```bash
git branch feature-x
git checkout feature-x
git merge feature-x
git branch -d feature-x
```

✅ **Mini Project:**

* Make a branch `new-feature`.
* Add new file → commit → merge to main.

---

## **Module 14: Merge Conflicts (Day 21)**

* If both branches edit same line → conflict.
* Fix conflict manually, then:

```bash
git add .
git commit -m "resolved conflict"
```

✅ **Mini Project:**

* Create conflict between `main` & `feature`.
* Resolve it.

---

## **Module 15: Markdown & Profile (Day 22)**

* Create `README.md`.
* Learn Markdown basics (headings, lists, tables, links, images).
* Create **Profile README** in GitHub by making a repo with same name as your username.

✅ **Mini Project:**

* Make a fancy README with your skills, social links.

---

## **Module 16: GitHub Pages (Day 23)**

* Create `index.html`.
* Push to repo.
* In repo → Settings → Pages → Deploy from branch.

✅ **Mini Project:**

* Publish a simple personal website.

---

## **Module 17: Interview Prep (Day 24)**

* Practice explaining:

  * What is Git vs GitHub?
  * What is commit, branch, merge?
  * What is rebase?
  * What is detached HEAD?
  * Difference between fork & clone?
* Practice solving merge conflict live.
