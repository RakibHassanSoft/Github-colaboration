
# For Manager/Leader:

### Create a new repository and make it visible for all
1. Go to `Settings` -> `Collaboration`
2. Add people -> Developer's username or email

### Create a new branch:
```bash
git checkout -b development    # Create and switch to the development branch
git add .                      # Stage changes
git commit -m "new branch has been created"  # Commit with a message
git push -u origin development  # Push to the remote development branch
```

---

# For Developers:

## Initial Setup:
1. Clone the repository:
```bash
git clone <Github-link>        # Clone the repository
git checkout -b your-branch-name  # Create and switch to your branch
```

---

## If you worked before:

### 1. Before Starting Work:

#### Update your local development branch:
```bash
git checkout development         # Switch to the development branch
git pull origin development       # Pull the latest changes from development
```

#### Create or switch to your branch:
```bash
git checkout your-branch-name   # Switch to your branch
```

---

### 2. While Working:

#### Commit changes regularly:
```bash
git add .                      # Stage all changes (or specific files with `git add <file-name>`)
git commit -m "Describe your changes"  # Commit with a message
git push origin your-branch-name  # Push your branch to the remote repository
```

#### Periodically merge development into your branch:
```bash
git checkout development          # Switch to the development branch
git pull origin development         # Pull the latest changes
git checkout your-branch-name       # Switch back to your branch
git merge development             # Merge development into your branch
```

---

### 3. Before Pushing Your Code:

#### Final merge with development:
```bash
git checkout development          # Switch to the development branch
git pull origin development         # Pull the latest changes
git checkout your-branch-name       # Switch back to your branch
git merge development             # Merge development into your branch
```

#### Resolve any merge conflicts (if any):
```bash
# Manually resolve conflicts
git add resolved-file-name          # Stage resolved files
git commit -m "Resolved merge conflicts"   # Commit the resolution
```

#### Push your branch:
```bash
git push origin your-branch-name    # Push your branch to the remote repository
```
