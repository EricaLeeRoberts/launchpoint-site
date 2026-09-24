# LaunchPoint Fitness Training website

One-page site for launchpointfitnesstraining.com, hosted on GitHub Pages.

## Files
- `index.html` – the whole site (text, styles, form)
- `images/` – photos
- `CNAME` – tells GitHub Pages to serve the site at www.launchpointfitnesstraining.com

## 1. Connect the form (Formspree)
1. Sign up at formspree.io and create a new form that sends to your email.
2. Copy the form ID (the part after `/f/` in the endpoint, e.g. `xabcdwxyz`).
3. In `index.html`, replace `YOUR_FORM_ID` with that ID. (Done: form "LaunchPoint Get Started", ID `mqpalkbl`, sends to ericaleeroberts@gmail.com.)

## 2. Put it on GitHub
1. Create a new repository (e.g. `launchpoint-site`).
2. Upload `index.html`, `CNAME`, and the `images` folder (Add file → Upload files).
3. Settings → Pages → Source: "Deploy from a branch" → `main` / `(root)` → Save.

## 3. Point the domain at GitHub
In the DNS settings wherever the domain is registered (Squarespace Domains if you bought it there), remove Squarespace's website records and add:

| Type  | Host | Value |
|-------|------|-------|
| CNAME | www  | `<your-github-username>.github.io` |
| A     | @    | 185.199.108.153 |
| A     | @    | 185.199.109.153 |
| A     | @    | 185.199.110.153 |
| A     | @    | 185.199.111.153 |

Then in Settings → Pages, set Custom domain to `www.launchpointfitnesstraining.com` and check "Enforce HTTPS" once it's available. DNS can take up to 24–48 hours.

## 4. Cancel Squarespace
Once the new site loads at your domain, cancel the Squarespace website plan. Keep the domain registration active (or transfer it to another registrar) so the domain doesn't lapse.

## Editing later
Text and prices are plain text in `index.html`. Edit the file on GitHub (pencil icon) and commit; the site updates in a minute or two.
