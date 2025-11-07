# Git & GitHub Workshop — Hands-on Activities

Welcome to the **Git & GitHub Workshop**! 🎉
This repository contains exercises and activities designed to help you practice using Git and GitHub effectively.

---

## ⚙️ General rules

Before you begin, please read these important rules:

1. **Do not overwrite or modify other participants’ files.** Always create and work on your own files or branches.
2. **Use your own name** (or GitHub username) in filenames and branches. Example: `tan_shan_chien.txt` or `branch_tan_shan_chien`.
3. **Pull before you push!** Run `git pull` before pushing to avoid merge conflicts.
4. **Commit with clear messages.** Example:

   ```bash
   git commit -m "added tan_shan_chien.txt"
   ```

5. **Ask for help** if you get merge conflicts or push rejections — don’t panic! 😄

---

## 🧩 Activity 1 — First GitHub repo

Goal: learn how to set up Git and push your first file to GitHub.

Steps:

1. Check if Git is installed:

   ```bash
   git --version
   ```

2. Configure Git (only once):

   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "you@example.com"
   ```

3. Create a new GitHub repository (on your GitHub account):

   - Go to GitHub → Repositories → New
   - Enter a name and click Create repository

4. Push your first file:

   ```bash
   echo "hello world" > hello_world.txt
   git init
   git add .
   git commit -m "first commit"
   git remote add origin <your_repo_url>
   git push -u origin main
   ```

You should now see your file in your GitHub repository.

---

## 🧑‍💻 Activity 2 — Collaborating on the workshop repo

Goal: learn how to clone, pull, push, and collaborate safely on a shared repository.

Steps:

1. Clone the workshop repository:

   ```bash
   git clone https://github.com/stanX19/git-github-workshop.git
   cd git-github-workshop
   ```

2. Pull the latest version:

   ```bash
   git pull
   ```

3. Create your own file (replace `your_name` with your name or GitHub username):

   ```bash
   echo "hello world" > your_name.txt
   ```

4. Commit and push your changes:

   ```bash
   git add .
   git commit -m "added your_name.txt"
   git push
   ```

   ⚠️ If your push is rejected, someone else might have pushed changes first. Run:

   ```bash
   git pull && git push
   ```

5. Check the GitHub repo to confirm your file appears online.

You’ve now contributed to a shared GitHub repository.

---

## 🌿 Activity 3 — Branching and merging

Goal: understand how to use branches to work independently and safely merge your work.

Steps:

1. Create and switch to a new branch:

   ```bash
   git checkout -b your_name
   ```

2. Create a new file and commit it:

   ```bash
   echo "hello from my branch" > hello_world.txt
   git add .
   git commit -m "created hello_world.txt on my branch"
   ```

3. Push your branch to GitHub:

   ```bash
   git push -u origin your_name
   ```

4. Check your branch online: visit the repository and look under the branches tab.

This is how developers work safely in parallel without breaking the main branch.

---

## 💡 Bonus tips

- Commit often with meaningful messages.
- Don’t use `git push -f` unless you fully understand what it does (it overwrites history).
- To undo a mistake safely, you can use one of the following:

  Restore a single file:

  ```bash
  git restore <filename>
  ```

  Or reset the last commit (destructive):

  ```bash
  git reset --hard HEAD~1
  ```

---

### 📚 Workshop repo

🔗 https://github.com/stanX19/git-github-workshop

---

**Happy coding and collaborating! 💻🚀**

---

## For the pros

If you're already comfortable with Git and GitHub and want to contribute improvements, please fork this repository, make your changes, and open a pull request against the original repository.

Quick checklist:

- Fork this repository on GitHub (use the "Fork" button in the top-right).
- Clone your fork locally, create a feature branch, make changes, and push the branch to your fork.
- Open a Pull Request (PR) from your branch on your fork to the `main` branch of the original repository.

Example steps (replace placeholders with your values):

```bash
# clone your fork (replace <your-username>)
git clone https://github.com/<your-username>/git-github-workshop.git
cd git-github-workshop

# create a feature branch
git checkout -b feat/your-change

# make changes, then commit and push
git add .
git commit -m "Describe your improvement"
git push -u origin feat/your-change
```

Then open a PR on GitHub from `feat/your-change` (your fork) → `stanX19:main` (original repo). In your PR description, explain the change, why it's useful, and include any testing or verification steps.

Suggested advanced contributions for pros:

- Add or improve CI (GitHub Actions) to run tests or linters.
- Add automated tests or example scripts demonstrating workshop exercises.
- Improve documentation: add a `CONTRIBUTING.md`, clearer challenge instructions, or troubleshooting tips.
- Add accessibility or localization improvements for non-English participants.
- Propose small refactors or fixes to any scripts, and include tests or examples.

Thanks for helping improve the workshop — we welcome thoughtful PRs and good commit messages.




feat/ANGKAIXIN-change
