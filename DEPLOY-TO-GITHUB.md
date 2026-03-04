# 🚀 Deploy Bar CRM to GitHub Pages

**Quick setup - 5 minutes to get your live URL**

---

## Step 1: Create GitHub Repo

1. Go to **https://github.com/new**
2. **Repository name:** `bar-crm` (or whatever you want)
3. **Visibility:** Public (required for free GitHub Pages)
4. **DO NOT** check "Add README" or "Add .gitignore" (we already have files)
5. Click **"Create repository"**

---

## Step 2: Push Your Code

GitHub will show you commands - **ignore those** and run these instead:

```bash
cd /Users/11-mac-alpha/.openclaw/workspace/bar-crm-github

# Set your GitHub username and email (one-time setup)
git config user.name "YOUR_GITHUB_USERNAME"
git config user.email "YOUR_EMAIL"

# Add GitHub as remote (replace YOUR_USERNAME with your actual GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/bar-crm.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**If it asks for credentials:**
- Username: your GitHub username
- Password: use a **Personal Access Token** (NOT your GitHub password)
  - Get one here: https://github.com/settings/tokens
  - Click "Generate new token (classic)"
  - Give it a name like "Bar CRM"
  - Check the "repo" scope
  - Copy the token and paste it as password

---

## Step 3: Enable GitHub Pages

1. Go to your repo on GitHub: `https://github.com/YOUR_USERNAME/bar-crm`
2. Click **Settings** (top right)
3. Click **Pages** (left sidebar)
4. Under "Source", select **`main`** branch
5. Click **Save**
6. Wait 1-2 minutes, then refresh - you'll see your URL!

**Your live URL will be:** `https://YOUR_USERNAME.github.io/bar-crm/bar-crm-app.html`

---

## 🎉 Done!

**Save that URL to your phone's home screen:**
- iPhone: Open in Safari → Share → Add to Home Screen
- Android: Open in Chrome → Menu → Add to Home screen

Now when I update the CRM data, I just push to GitHub and you refresh the page!

---

## 🔄 How Updates Work (After Setup)

**When you voice message me:**
1. I transcribe it
2. Update `bar-crm-data.json`
3. Run:
   ```bash
   cd /Users/11-mac-alpha/.openclaw/workspace/bar-crm-github
   git add bar-crm-data.json
   git commit -m "Updated CRM: [your update]"
   git push
   ```
4. You refresh the page on your phone → see changes

**Fully automated!**
