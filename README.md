# 📘 Most Used Git & AWS CLI Commands

This document contains a curated list of commonly used Git and AWS CLI commands based on real-world usage.

---

## 🔀 Git Commands

### 📂 Branch-Based Development (Quick Overview)

Branch-based development is a Git workflow where each new feature, bugfix, or task is developed in its own dedicated branch. This promotes isolation, collaboration, and safer code integration. Typically, developers branch off from a main branch (like `master` or `main`) and later merge changes back after review and testing.

Key Benefits:

* Keeps the main branch stable
* Enables parallel development
* Simplifies code reviews via pull requests

---

### 🧱 Listing Branches

* **List remote branches:**

  ```sh
  git branch -r
  ```

* **List both local and remote branches:**

  ```sh
  git branch -a
  ```

---

### 🌱 Creating and Switching Branches

* **Create a new branch from the current one:**

  ```sh
  git branch <new-branch-name>
  ```

* **Create and switch to the new branch (classic):**

  ```sh
  git checkout -b <new-branch-name>
  ```

* **Create and switch to the new branch (modern):**

  ```sh
  git switch -c <new-branch-name>
  ```

---

### 🔍 Viewing Remote Tracking Branches

* **List all remote branches and their references:**

  ```sh
  git ls-remote --heads origin
  ```

---

### 🚀 Pushing Changes

* **Push your changes safely, ensuring no one else's work is overwritten:**

  ```sh
  git push --force-with-lease
  ```

  > Use this instead of `--force` to avoid accidentally overwriting commits made by others.

---

### 🔄 Rebasing

* **Rebase your current branch onto `master`:**

  ```sh
  git rebase master
  ```

  > Keeps your history clean by replaying your commits on top of the latest `master`. Useful before merging or pushing shared branches.

---

## ☁️ AWS CLI Commands

### 📦 Sync Static Files to S3

* **Upload the latest build and remove outdated files:**

  ```sh
  aws s3 sync dist/ s3://2024ana --delete
  ```

---

### 🌐 Invalidate CloudFront Cache

* **Force CloudFront to serve fresh content from S3:**

  ```sh
  aws cloudfront create-invalidation \
    --distribution-id E1IRVC5C4GFCAP \
    --paths "/*"
  ```

---



### Powershell

Remove-Item -Recurse -Force node_modules, package-lock.json

