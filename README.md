# Vaibhav Aggarwal — Personal Website

A fast, single-page personal site for Vaibhav Aggarwal (Head of Applied AI · ServiceNow AI Specialist). Self-contained static HTML with inline CSS and JS — no build step, no dependencies.

## Files
- `index.html` — the entire site (markup, styling, and scripts inline)
- `assets/vaibhav.jpg` — headshot (optimized)
- `assets/Vaibhav-Aggarwal-CV.pdf` — downloadable CV
- `netlify.toml` — Netlify config + headers

## Run locally
Open `index.html` in a browser, or serve it:

```bash
python3 -m http.server 8000
# → http://localhost:8000
```

## Deploy to Netlify

**Option A — drag & drop (fastest)**
1. Go to https://app.netlify.com/drop
2. Drag this whole folder onto the page. Done — you get a live URL instantly.

**Option B — Git-connected (recommended for ongoing edits)**
1. Push this folder to a GitHub repo.
2. In Netlify: *Add new site → Import an existing project* → pick the repo.
3. Build command: *(leave empty)* · Publish directory: `.`
4. Deploy. Every push auto-publishes.

**Option C — Netlify CLI**
```bash
npm i -g netlify-cli
netlify deploy --prod
```

## Customise
- Colours/theme: the `:root` variables at the top of the `<style>` block in `index.html`, plus the "Vaibhav palette overrides" block at the end of it.
- Copy: all content lives in `index.html`.
- Add a custom domain in Netlify → *Domain settings*.
