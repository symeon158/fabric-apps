# GitHub Setup Guide - Fabric Apps

Follow these steps to create and push your Fabric Apps project to GitHub.

## Step 1: Create a New GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in to your account
2. Click the **"+"** icon in the top-right corner
3. Select **"New repository"**
4. Fill in the repository details:
   - **Repository name**: `fabric-apps`
   - **Description**: "A comprehensive demonstration of building scalable applications using Microsoft Fabric"
   - **Visibility**: Choose "Public" (to share with others) or "Private" (for personal use)
   - **Initialize repository**: Leave unchecked (we'll push existing files)
5. Click **"Create repository"**

## Step 2: Initialize Git Locally

Open your terminal/command prompt and navigate to your project folder:

```bash
cd path/to/your/fabric-apps-folder
```

Initialize Git and add the files:

```bash
# Initialize git repository
git init

# Add all files
git add .

# Create initial commit
git commit -m "Initial commit: Add Fabric Apps project demonstration"
```

## Step 3: Connect to GitHub and Push

Copy the commands from your GitHub repository page (it will look like this):

```bash
# Add the remote repository
git remote add origin https://github.com/yourusername/fabric-apps.git

# Rename branch to main (if needed)
git branch -M main

# Push files to GitHub
git push -u origin main
```

Replace `yourusername` with your actual GitHub username.

## Step 4: Verify Your Repository

1. Go to `https://github.com/yourusername/fabric-apps`
2. Verify that all files are uploaded:
   - ✅ README.md
   - ✅ manpower-budget-demo.html
   - ✅ manpower-budget-demo.mp4
   - ✅ .gitignore
   - ✅ GITHUB_SETUP.md

## Step 5: Update the GitHub Links

Edit the files to replace placeholders with your actual GitHub username:

### In `manpower-budget-demo.html`:
Find this line:
```html
<a href="https://github.com/yourusername/fabric-apps" class="github-link" target="_blank">
```
Replace `yourusername` with your GitHub username.

### In `README.md`:
Replace all instances of:
- `yourusername` with your GitHub username

Then commit and push these changes:

```bash
git add .
git commit -m "Update GitHub links with correct username"
git push
```

## Step 6: Share Your Project

Your project is now live on GitHub! Share the link:
- **Repository URL**: `https://github.com/yourusername/fabric-apps`
- **Demo Link**: `https://github.com/yourusername/fabric-apps/blob/main/manpower-budget-demo.html`

### For Your CV
Add this to your CV or portfolio:
```
Fabric Apps - Microsoft Fabric Project
GitHub: github.com/yourusername/fabric-apps
```

## Optional: Set Up GitHub Pages (To Host the Demo Online)

Make the demo viewable directly from GitHub:

1. Go to your repository settings
2. Scroll to **"GitHub Pages"**
3. Under **"Source"**, select **"main"** branch
4. Save
5. Your demo will be available at: `https://yourusername.github.io/fabric-apps/manpower-budget-demo.html`

## Useful Git Commands

```bash
# Check status of files
git status

# View commit history
git log

# Make changes and update
git add .
git commit -m "Your message here"
git push

# Pull latest changes (if working with others)
git pull origin main
```

## Troubleshooting

**Issue**: "Permission denied (publickey)"
- Solution: Set up SSH keys or use HTTPS with personal access token

**Issue**: Large file (video) won't upload
- Solution: Use Git LFS (Large File Storage) for video files
  ```bash
  git lfs install
  git lfs track "*.mp4"
  git add .gitattributes
  ```

**Issue**: "fatal: not a git repository"
- Solution: Make sure you're in the correct folder and ran `git init`

---

For more help, visit the [GitHub Docs](https://docs.github.com/en/repositories/creating-and-managing-repositories)
