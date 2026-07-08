# Condo Owners Alliance — Website

Static website for Condo Owners Alliance (condoownersalliance.com).

## Deploy on Vercel

1. Push this repository to GitHub
2. Go to [vercel.com](https://vercel.com) → New Project → Import from GitHub
3. Select this repository
4. Framework Preset: **Other** (static site)
5. Root Directory: `/` (leave as default)
6. Click **Deploy**

## Custom Domain

After deploy on Vercel:
1. Go to Project Settings → Domains
2. Add your domain (e.g. `condoownersalliance.com`)
3. In your DNS provider, add:
   - **A record**: `@` → `76.76.21.21`
   - **CNAME record**: `www` → `cname.vercel-dns.com`
4. Wait for DNS propagation (up to 48h)

## Files

- `index.html` — Main website (self-contained, all assets embedded as base64)
- `vercel.json` — Vercel deployment configuration
- `.gitignore` — Git ignore rules

## Tech Stack

- Pure HTML5 + CSS3 + Vanilla JavaScript
- No dependencies, no build step required
- All fonts and images embedded as base64 (fully self-contained)
- Responsive: mobile, tablet, desktop
