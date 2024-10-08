---

## Challenge

In this exercise, you'll learn how to use `git stash` to temporarily save your uncommitted work while switching branches to fix an urgent issue. You'll stash your changes, switch branches, apply a fix, and then retrieve your stashed changes afterward.

## Steps to Follow

### 1. **Create a GitHub Repository**

- Go to GitHub and create a new repository (e.g., "git-stash-exercise").
- Leave it empty without a README for now.

### 2. **Initialize a Local Git Repository**

- In your terminal, create a new directory and initialize it as a Git repository.

   ```bash
   mkdir git-stash-exercise
   cd git-stash-exercise
   git init
   ```

### 3. **Add and Commit Initial Files**

- Create some initial files like `index.html` and `style.css`:

  ```bash
  touch index.html style.css
  ```

- Add some content to the files, then stage and commit them.

   ```bash
   git add .
   git commit -m "Initial commit with basic project structure"
   ```

### 4. **Link the Local Repository to GitHub**

- Link your local repo to the GitHub repo you created earlier by adding a remote.

   ```bash
   git remote add origin https://github.com/yourusername/git-stash-exercise.git
   ```

- Check if `main` is the default branch for your GitHub repo:

   ```bash
   git branch -M main
   ```

### 5. **Push the Initial Commit**

- Now push the initial commit to the `main` branch on GitHub.

   ```bash
   git push -u origin main
   ```

### 6. **Create a New Feature Branch**

- Create a new branch for the feature you want to work on.

   ```bash
   git checkout -b feature/new-feature
   ```

### 7. **Make Changes on the Feature Branch**

- Modify or create new files to represent work on the feature.

### 8. **Stash the Changes**

- Stash the changes when you are interrupted by an urgent bug fix.

   ```bash
   git stash
   ```

### 9. **Switch to the Main Branch**

- Switch back to the `main` branch to address the bug.

   ```bash
   git checkout main
   ```

### 10. **Fix the Bug and Commit**

- Fix the bug, then stage and commit the changes.

   ```bash
   git add .
   git commit -m "Bug fix on main branch"
   git push origin main
   ```

### 11. **Switch Back to the Feature Branch**

- Switch back to the feature branch where your unfinished work is stashed.

   ```bash
   git checkout feature/new-feature
   ```

### 12. **Retrieve Stashed Changes**

- Retrieve the changes you stashed earlier.

   ```bash
   git stash pop
   ```

### 13. **Verify and Continue**

- Ensure the changes have been restored, and continue working on the feature.

---

This should resolve any issues with missing branches or unpushed commits! Let me know if you run into any further issues.
