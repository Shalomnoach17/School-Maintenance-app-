# School Maintenance Request (Ward 5) — FINAL

This is the final static build based on your v23 design with incremental fixes:
- Location chips fixed (single-select, auto-fill field, clear, and “Other” flow)
- Header text updated to **School Maintenance Request**
- Oval removed from header
- Thank-you confirmation modal after submit
- Common Issues and photo upload behavior kept as in v23

## Files
- `index.html` — main page
- (Any other assets from your original v23 are preserved.)

## Quick local test
1. Download and unzip this folder.
2. Open `index.html` in a desktop browser.
3. For **iPhone** testing: Airdrop the folder to Files → open `index.html` in Safari, or host it (see below) and scan the URL QR.

## Deploy options

### Option A — GitHub Pages (free)
1. Create a new repo on GitHub (e.g., `school-maintenance-request`).
2. Upload the contents (not the zip) — be sure `index.html` is at the root.
3. In **Settings → Pages**, set **Build and deployment** to **Deploy from a branch**, branch **main**, folder **/** (root), and save.
4. Wait 1–2 minutes; your site will be live at `https://<your-username>.github.io/school-maintenance-request/`.

### Option B — Netlify (drag & drop)
1. Go to https://app.netlify.com/ and log in.
2. Drag the unzipped folder into **Sites → Drag and drop**.
3. Netlify will assign a URL like `https://your-site-name.netlify.app/` which you can rename.

### Option C — Simple static host (any server)
Upload the folder to any static host (S3/CloudFront, Nginx, Apache, etc.) and ensure `index.html` is served as the default document.

## Email wiring (future step)
Right now this is a static demo. To send the form to a Council inbox (e.g., `elite.prints.info2@gmail.com` or the Ward 5 team), you’ll need a small serverless function or form service (Netlify Forms, Google Apps Script, Vercel function) to accept the POST and send an email. I can wire that up when you’re ready.

## Version
`v23-FINAL` (header updated, oval removed, location fix, confirmation modal)
