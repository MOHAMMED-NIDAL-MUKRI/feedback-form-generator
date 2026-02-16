# GitHub Pages Hosting Guide

## 🚀 Host Your Presentation on GitHub Pages

Follow these steps to host your presentation online for free using GitHub Pages.

---

## **Step 1: Initialize Git Repository**

Open your terminal/command prompt in the project folder and run:

```bash
# Initialize git repository
git init

# Add all files
git add .

# Create first commit
git commit -m "Initial commit: Intelligent Feedback Form Generation System"
```

---

## **Step 2: Create GitHub Repository**

1. Go to [GitHub.com](https://github.com) and log in
2. Click the **"+"** icon (top right) → **"New repository"**
3. Fill in the details:
   - **Repository name**: `feedback-form-generator` (or any name you prefer)
   - **Description**: "Intelligent Feedback Form Generation System - College Project"
   - **Visibility**: Choose **Public** (required for free GitHub Pages)
   - **DO NOT** initialize with README (we already have files)
4. Click **"Create repository"**

---

## **Step 3: Connect Local Repository to GitHub**

GitHub will show you commands. Use these (replace `YOUR_USERNAME` with your actual GitHub username):

```bash
# Add remote repository
git remote add origin https://github.com/YOUR_USERNAME/feedback-form-generator.git

# Rename branch to main (if needed)
git branch -M main

# Push to GitHub
git push -u origin main
```

---

## **Step 4: Enable GitHub Pages**

1. Go to your repository on GitHub
2. Click **"Settings"** (top menu)
3. Scroll down to **"Pages"** (left sidebar under "Code and automation")
4. Under **"Source"**, select:
   - **Branch**: `main`
   - **Folder**: `/ (root)`
5. Click **"Save"**

---

## **Step 5: Rename presentation.html to index.html**

GitHub Pages looks for `index.html` as the main page. You need to rename your file:

```bash
# Rename the file
git mv presentation.html index.html

# Commit the change
git add .
git commit -m "Rename presentation.html to index.html for GitHub Pages"

# Push to GitHub
git push
```

---

## **Step 6: Access Your Live Presentation**

After a few minutes (usually 1-2 minutes), your presentation will be live at:

```
https://YOUR_USERNAME.github.io/feedback-form-generator/
```

For example, if your GitHub username is `mohdnidal`, it would be:
```
https://mohdnidal.github.io/feedback-form-generator/
```

---

## **Quick Commands Summary**

```bash
# 1. Initialize and commit
git init
git add .
git commit -m "Initial commit: Intelligent Feedback Form Generation System"

# 2. Connect to GitHub (replace YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/feedback-form-generator.git
git branch -M main
git push -u origin main

# 3. Rename for GitHub Pages
git mv presentation.html index.html
git commit -m "Rename for GitHub Pages"
git push

# 4. Enable GitHub Pages in repository settings
# Visit: Settings → Pages → Source: main branch → Save
```

---

## **Updating Your Presentation**

Whenever you make changes to your presentation:

```bash
# Add changes
git add .

# Commit with a message
git commit -m "Updated contact information"

# Push to GitHub
git push

# Changes will be live in 1-2 minutes
```

---

## **Alternative: Quick Deploy with GitHub Desktop**

If you prefer a GUI:

1. Download [GitHub Desktop](https://desktop.github.com/)
2. Open GitHub Desktop → **File** → **Add Local Repository**
3. Select your project folder
4. Click **"Publish repository"**
5. Enable GitHub Pages in repository settings (Step 4 above)
6. Rename `presentation.html` to `index.html`

---

## **Troubleshooting**

### **404 Error**
- Make sure the file is named `index.html` (not `presentation.html`)
- Wait 2-3 minutes after enabling GitHub Pages
- Check that the repository is **Public**

### **Changes Not Showing**
- Clear browser cache (Ctrl + Shift + R)
- Wait a few minutes for GitHub to rebuild
- Check if your commit was pushed: `git log`

### **Git Not Recognized**
- Install Git: [git-scm.com/downloads](https://git-scm.com/downloads)
- Restart your terminal after installation

---

## **Bonus: Custom Domain (Optional)**

If you have a custom domain:

1. Add a file named `CNAME` with your domain name
2. Configure DNS settings with your domain provider
3. Enable HTTPS in GitHub Pages settings

---

## **Share Your Presentation**

Once live, you can share the URL:
- Add it to your LinkedIn profile
- Include it in your project report
- Share with professors and classmates
- Add to your resume/portfolio

**Your live presentation URL will be:**
```
https://YOUR_USERNAME.github.io/feedback-form-generator/
```

🎉 **That's it! Your presentation is now hosted online for free!**
