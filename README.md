# Portfolio Site

A single-file static portfolio site (HTML/CSS/JS, no build step) covering
About, Skills, Projects, Résumé, and Contact — ready to host free on GitHub
Pages.

## Before you publish

Just double-check the links in `index.html` point to your real GitHub repos,
LinkedIn, and email — they're already filled in, but confirm the URLs are
correct: search for `github.com/Nakshu`, `linkedin.com/in/`, and `mailto:`.

## Hosting on GitHub Pages (free)

You have two options depending on whether you want the site at
`nakshu.github.io` directly, or as a project page under a named repo.

### Option A — Your main GitHub Pages site (recommended)

This makes your site live at `https://nakshu.github.io`.

1. Create a **new repository** on GitHub named **exactly**:
   ```
   Nakshu.github.io
   ```
   (must match your GitHub username exactly, case doesn't matter for the
   username part but the format `username.github.io` is required)
2. Don't add a README or license during creation (we already have files).
3. On your Mac, open Terminal:
   ```bash
   cd ~/Downloads/portfolio-site
   git init
   git add .
   git commit -m "Initial portfolio site"
   git remote add origin https://github.com/Nakshu/Nakshu.github.io.git
   git branch -M main
   git push -u origin main
   ```
4. Wait 1-2 minutes, then visit `https://nakshu.github.io` — it should be
   live automatically. GitHub Pages auto-publishes `username.github.io`
   repos with no extra settings needed.

### Option B — A project page under a different repo name

If you'd rather keep it under a repo like `portfolio` instead:

1. Create a repo named `portfolio` (or anything you like)
2. Push the same way as above, but with that repo's URL
3. Go to the repo on GitHub → **Settings** → **Pages** (left sidebar)
4. Under "Build and deployment" → Source: select **"Deploy from a
   branch"** → Branch: `main`, folder: `/ (root)` → **Save**
5. Wait 1-2 minutes, then visit `https://nakshu.github.io/portfolio`

## Making updates later

Any time you want to change something (add a project, update a metric,
tweak the About text), edit `index.html` directly, then:

```bash
git add .
git commit -m "Update site"
git push
```

Changes go live within a minute or two of pushing.
