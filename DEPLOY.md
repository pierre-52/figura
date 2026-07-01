# Deploying Figura to GitHub Pages (free hosting)

This puts Figura online at a URL you can open from any computer, and backs up your code.

## One-time setup

### 1. Create a GitHub account
If you don't have one: https://github.com/signup

### 2. Create an empty repository
- Go to https://github.com/new
- **Repository name:** `figura`
- Visibility: **Public** (required for free GitHub Pages) or Private (Pages needs a paid plan for private)
- Do **NOT** tick "Add a README" (this project already has one)
- Click **Create repository**

### 3. Connect this folder to it and push
Copy the commands GitHub shows under "…or push an existing repository", or run these
(replace `YOUR-USERNAME` with your GitHub username):

```
cd C:\Users\hannap\figura
git remote add origin https://github.com/YOUR-USERNAME/figura.git
git push -u origin main
```

The first push will ask you to sign in to GitHub (a browser window opens) — approve it.

### 4. Turn on GitHub Pages
- In the repo: **Settings → Pages**
- Under **Build and deployment → Source**, choose **Deploy from a branch**
- **Branch:** `main`, folder: `/ (root)` → **Save**
- Wait ~1 minute. Your site will be live at:

```
https://YOUR-USERNAME.github.io/figura/
```

That URL works on any computer, phone or tablet.

## Updating the site later

Whenever `index.html` changes, publish the update with:

```
cd C:\Users\hannap\figura
git add -A
git commit -m "Describe what changed"
git push
```

GitHub Pages redeploys automatically within a minute or so.

## Custom domain (optional)
If you buy a domain (e.g. `figura.com`), you can point it at GitHub Pages under
**Settings → Pages → Custom domain**.

## Notes
- Hosting makes the **app** available everywhere. Teachers' **saved canvases** still live in
  each browser's local storage — cross-device sync needs a backend (a later phase).
- Keep the repo **Public** for free Pages. If the code must stay private, use Netlify or
  Cloudflare Pages (both offer free hosting of private repos) instead.
