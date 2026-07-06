# Portfolio site

Single static file: `index.html`. No build step, no dependencies.

## Deploy to Cloudflare (2 min)

**Option A — drag and drop:**
Cloudflare dashboard → Workers & Pages → Create → Pages → Upload assets → drag this `portfolio` folder in. Done — you get `<name>.pages.dev`, add a custom domain if you want.

**Option B — from a GitHub repo (auto-deploys on push):**
1. Push this folder to a repo (e.g. `esvarmajor/portfolio`)
2. Cloudflare dashboard → Workers & Pages → Create → Pages → Connect to Git
3. Build command: none · Output directory: `/`

**Option C — CLI:** `npx wrangler pages deploy portfolio`

## Notes
- Preview locally by just opening `index.html` in a browser.
- Phone/address intentionally omitted (public site) — email, GitHub, LinkedIn only.
- SWARMCORE media (loop video, screenshots, OG image) is hot-linked from `raw.githubusercontent.com` — it only works while the SWARMCORE repo stays **public**. For full control, download the files into this folder and swap the URLs to relative paths.
- The `stonks` and `resume-copilot` cards describe private projects; delete either block if you'd rather not mention them publicly. STONKS copy deliberately avoids dollar amounts and account details.
- `_v1-classic.html` is the previous (pre-SWARMCORE) design, kept as a backup. Don't upload it, or it'll be publicly reachable at `/_v1-classic`.
