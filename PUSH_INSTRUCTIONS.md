# GitHub Push Instructions - HTTPS Method

## Problem
SSH push failing: `Permission denied (publickey)`

## Solution: Switch to HTTPS

### Step 1: Change Remote URL to HTTPS
```bash
cd /home/ubuntu/.openclaw/workspace/mathematical-philosophy

# Change from SSH to HTTPS
git remote set-url origin https://github.com/T4UNLTD/mathematical-philosophy.git

# Verify
git remote -v
```

### Step 2: Push to GitHub
```bash
# This will prompt for GitHub username and password
git push -u origin main
```

**Note:** When prompted for password, use a **Personal Access Token** (not your GitHub account password):
1. Go to https://github.com/settings/tokens
2. Generate new token → Select "repo" scope
3. Use this token as your password

### Alternative: Push from /home/node/.openclaw/workspace/

If the sandbox environment can push with credentials:

```bash
# Copy files from node workspace to ubuntu workspace
cd /home/ubuntu/.openclaw/workspace
rm -rf mathematical-philosophy
cp -r /home/node/.openclaw/workspace/mathematical-philosophy .
cd mathematical-philosophy

# Initialize new git
git init
git config user.email "c.waynethompson@gmail.com"
git config user.name "Chris"
git add .
git commit -m "Initial commit: Mathematical philosophy blog"

# Add HTTPS remote
git remote add origin https://github.com/T4UNLTD/mathematical-philosophy.git
git branch -M main

# Push (will prompt for credentials)
git push -u origin main
```

### After Successful Push

1. Go to https://github.com/T4UNLTD/mathematical-philosophy
2. Navigate to **Settings** → **Pages**
3. **Source**: Deploy from a branch
4. **Branch**: main → /(root)
5. Click **Save**

Your site will be live at: https://t4unltd.github.io/mathematical-philosophy/
