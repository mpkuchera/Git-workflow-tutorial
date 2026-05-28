# Git & GitHub Research Workflow Activity

Welcome! Today’s goal is to practice a realistic collaborative research workflow using Git and GitHub.

You will work with a partner and simulate how collaborative software and research development typically happens in research groups and open-source projects.

---

# Learning Goals

By the end of this activity, you should be able to:

* Fork and clone a repository
* Create task-specific branches
* Make meaningful commits
* Push changes to GitHub
* Open and review Pull Requests (PRs)
* Merge code changes collaboratively
* Resolve small workflow issues as a team

---

# Setup

## Step 1 — Form a Team

Identify your partner.

One person will create a new GitHub repository **by forking this repository**.

This person will fork into their own GitHub account.

The repository owner should then invite their partner as a collaborator.

---

## Step 2 — Both Students Clone the Repository

Each student should clone the repository to their local machine.

```bash
git clone <repository-url>
cd <repository-name>
```

---

# Research Workflow Activity

You will now simulate a common collaborative development workflow.

---

# Part 1 — Student 1 Creates a Feature Branch

Student 1 should create a new branch for their work.

Example:

```bash
git checkout -b fix-typo-and-docstring
```

---

# Part 2 — Modify the File

Open `hello.py`.

1. Fix the typo in the file
2. Add your name and date to the docstring at the top

Example:

```python
edited: A. Student 05/28/26
```

---

# Part 3 — Commit Your Changes

Commit your changes with a meaningful commit message.

Example:

```bash
git add hello.py
git commit -m "Fix typo and update docstring"
```

---

# Part 4 — Push the Branch

Push your branch to GitHub.

```bash
git push origin fix-typo-and-docstring
```

---

# Part 5 — Open a Pull Request

On GitHub:

1. Open a Pull Request (PR)
2. Add your partner as a reviewer
3. Write a short PR description explaining your changes

Your partner should review the PR before merging.

---

# Part 6 — Student 2 Reviews and Merges

Student 2 should:

1. Review the Pull Request
2. Leave a comment or approval
3. Merge the PR into `main`

---

# Part 7 — Sync Local Repositories

After the PR is merged, BOTH students should update their local repositories.

```bash
git checkout main
git pull origin main
```

---

# Part 8 — Student 2 Creates a New Branch

Student 2 should now create their own feature branch.

Example:

```bash
git checkout -b add-image-and-update-docstring
```

---

# Part 9 — Add Additional Changes

Student 2 should:

1. Add another edit line to the docstring
2. Add an image file to the repository

Suggested folder structure:

```text
images/
```

Example:

```text
images/cat.png
```

---

# Part 10 — Commit and Push

```bash
git add .
git commit -m "Add image and update documentation"
git push origin add-image-and-update-docstring
```

---

# Part 11 — Open Another Pull Request

Student 2 should now:

1. Open a second PR
2. Request review from Student 1
3. Merge after approval

---

# Best Practices

## Commit Early and Often

Small commits are easier to understand, review, and debug.

---

## Write Meaningful Commit Messages

Good commit messages describe *what* changed and *why*.

Good examples:

```text
Add preprocessing script for detector data
Fix plotting bug in training notebook
Update README with setup instructions
```

Poor examples:

```text
stuff
changes
fixed things
```

---

## Use Branches for Individual Tasks

Avoid working directly on `main`.

Feature branches help isolate work and reduce merge conflicts.

---

## Pull Frequently

Before starting new work:

```bash
git checkout main
git pull origin main
```

This helps keep your repository up to date.

---

# Deliverables

By the end of class, your repository should contain:

* Multiple branches
* At least two merged Pull Requests
* Multiple commits with meaningful messages
* Updated `hello.py`
* An added image file
* A complete GitHub commit history

---

# Reflection Questions

Discuss briefly with your partner:

1. What advantages do Pull Requests provide?
2. Why are branches useful in collaborative work?
3. What problems can occur if multiple people edit `main` directly?
4. How might this workflow scale to larger research collaborations?

---

# Optional Challenge

If time permits:

* Intentionally create a merge conflict
* Work together to resolve it
* Commit the resolution
* Push the fixed version

---

# Reminder

This workflow is extremely common in:

* Research software development
* Machine learning projects
* Scientific computing collaborations
* Open-source software
* Industry software engineering teams

The goal is not just to “use Git,” but to develop good collaborative habits.
