# Belén Carpio Website

Static HTML5 website for `belencarpio.com`.

## Local Preview

```powershell
python -m http.server 8799 --bind 127.0.0.1
```

Open `http://127.0.0.1:8799/`.

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

