# Step Tasks — deploy to GitHub Pages (free)

This folder has everything you need. It's a single static page, so there's
no build step and no cost.

**Files:**
- `index.html` — the app itself
- `.nojekyll` — tells GitHub Pages to serve the file as-is, skipping its
  default Jekyll processing (harmless to include, avoids edge-case issues)

## Steps

### 1. Create the repo
Go to https://github.com/new, name it something like `step-tasks`, set it
to **Public** (required for free GitHub Pages on a personal account), and
create it. You can leave "Add a README" unchecked since you already have one.

### 2. Add these files to it
Easiest way, no git required:
1. Open your new repo on github.com.
2. Click **Add file → Upload files**.
3. Drag in `index.html` and `.nojekyll` from this folder (unzip first if
   you downloaded the zip).
4. Scroll down, click **Commit changes**.

(If you're comfortable with git instead: `git init`, `git add .`,
`git commit -m "add step tasks app"`, then push to the repo you created.)

### 3. Turn on Pages
1. In the repo, go to **Settings → Pages** (left sidebar, under "Code and
   automation").
2. Under **Build and deployment → Source**, choose **Deploy from a branch**.
3. Under **Branch**, choose `main` and folder `/ (root)`, then **Save**.
4. Wait a minute or two. Refresh the Pages settings page and you'll see
   "Your site is live at https://<your-username>.github.io/step-tasks/".

That link is your app — open it on any device, bookmark it, share it.

## Updating it later

Edit `index.html` on your computer, then on github.com use **Add file →
Upload files** again (or `git add`, `commit`, `push` if using git) — Pages
redeploys automatically within a minute of any push to `main`.

## Notes

- No environment variables, backend, or database needed — it's entirely
  client-side.
- The app saves your tasks automatically to the browser's local storage on
  whatever device/browser you use to open the link. Use the Export/Import
  buttons inside the app if you want to move your list between devices or
  keep a backup file.
