# Deploy to GitHub Pages (github.io)

## 1. Create the repository on GitHub

- Go to [GitHub](https://github.com/new).
- **Repository name:** use **`YOUR_USERNAME.github.io`** (e.g. `sumitsharma.github.io`) so the site is at `https://YOUR_USERNAME.github.io`.
- Set visibility to **Public**. Do **not** add a README, .gitignore, or license (you already have files locally).
- Click **Create repository**.

## 2. Push your site from your computer

In a terminal, from this project folder:

```bash
# Initialize git (if not already)
git init

# Add all files
git add .

# First commit
git commit -m "Initial commit - portfolio site"

# Add GitHub as remote (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/YOUR_USERNAME.github.io.git

# Push (use main branch for GitHub Pages)
git branch -M main
git push -u origin main
```

## 3. Turn on GitHub Pages

- On GitHub, open your repo **Settings** → **Pages** (left sidebar).
- Under **Build and deployment** → **Source**, choose **Deploy from a branch**.
- **Branch:** `main` (or `master`) — **Folder:** `/ (root)`.
- Click **Save**.

## 4. Wait and open your site

- After 1–2 minutes the site will be at **`https://YOUR_USERNAME.github.io`**.
- If you used a different repo name (e.g. `portfolio`), the URL will be `https://YOUR_USERNAME.github.io/portfolio/` and you may need to fix asset paths.

---

**Tip:** For the clean URL `https://YOUR_USERNAME.github.io`, the repo **must** be named exactly `YOUR_USERNAME.github.io`.
