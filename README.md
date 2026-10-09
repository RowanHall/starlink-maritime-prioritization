# CSC 466 Project Proposal — Maritime Starlink Traffic Prioritization

Static project website for the CSC 466 proposal *"Prioritizing Maritime Starlink
Traffic for Commercial Fishing Vessels"* (Jasper McLennan, Rowan Hall).

Plain HTML/CSS — no build step. `index.html` + `style.css`.

## Preview locally

Open `index.html` directly in a browser, or serve it:

```sh
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Deploy to GitHub Pages

1. Create a repo on GitHub (e.g. `csc466-starlink-qos`) and push these files:

   ```sh
   git init
   git add .
   git commit -m "Initial project proposal site"
   git branch -M main
   git remote add origin https://github.com/<you>/csc466-starlink-qos.git
   git push -u origin main
   ```

2. On GitHub: **Settings → Pages → Build and deployment**, set
   **Source = Deploy from a branch**, **Branch = `main` / `root`**, save.

3. The site goes live at `https://<you>.github.io/csc466-starlink-qos/`
   within a minute or two. Paste that URL into the proposal's
   "public website url" line and the Teams post.
