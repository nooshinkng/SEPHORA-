# Sephora Mini Missions (Static Web Game)

A single-file, mobile-friendly mini-game (Levels 1–4, soft audio, glassy shader).  
Just host as a static site.

## Local preview
Open `index.html` in a modern browser, or serve with any static server.

## Deploy to GitHub + Vercel

### 1) New GitHub repo
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/<YOUR-USER>/sephora-mini-missions.git
git push -u origin main
```

### 2) Vercel
- Go to https://vercel.com/new
- Import your new repo
- Framework Preset: **Other** (or **Static HTML**)
- Root directory: `/` (project root)
- Build command: **None**
- Output directory: `/` (since it's just `index.html`)
- Deploy

That's it — Vercel will serve `index.html` at your domain.

### Optional: Custom domain
- In your Vercel project → Settings → Domains → Add.

---

## Notes
- Everything is in `index.html` (Three.js from CDN). No build step required.
- If you add assets later, just keep relative paths and commit them.
- To invalidate caches after updates, create a new deployment on Vercel (auto on push).
