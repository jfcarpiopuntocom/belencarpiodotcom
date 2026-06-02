# Belén Carpio Website

Static HTML5 website for `belencarpio.com`.

The site is intentionally one bilingual page at `/`. Spanish is handled with the in-page language switch, not a separate `/es/` route.

## Local Preview

```powershell
python -m http.server 8799 --bind 127.0.0.1
```

Open `http://127.0.0.1:8799/`.

## Static Extras

- `sitemap.xml`: canonical sitemap for the single public URL.
- `robots.txt`: crawl policy and sitemap discovery.
- `llms.txt`: LLM-readable site summary.
- `humans.txt`: human-readable site summary.
- `site.webmanifest`: browser manifest.
- `404.html`: fallback back to the central page.
- `_redirects`: Cloudflare Pages redirects from old `/es/` paths to `/`.
- `_headers`: Cloudflare Pages headers for security and cache behavior.

## Deployment Notes

Recommended path:

1. Create a new GitHub repository for this folder.
2. Connect the repository to Cloudflare Pages.
3. Use these Cloudflare Pages settings:
   - Framework preset: `None`
   - Build command: empty
   - Build output directory: `/`
4. After buying `belencarpio.com`, add it as a custom domain in Cloudflare Pages.
5. Point DNS to Cloudflare and let Cloudflare manage the Pages records.
