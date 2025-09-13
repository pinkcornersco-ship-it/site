# Pink Corners — GitHub Pages + Formspree

## Files
- `index.html` — static site with Formspree endpoint preconfigured: https://formspree.io/f/mgvlqpkk
- `CNAME` — pinkcorners.com (custom domain)

## Deploy
1) Create a **public** GitHub repo and upload **both** files to the **root**.
2) Settings → Pages → Build and deployment:
   - Source: **Deploy from a branch**
   - Branch: `main` • Folder: `/ (root)`
3) Settings → Pages → Custom domain: `pinkcorners.com` → **Save**
4) DNS (at your registrar):
   - A @ → 185.199.108.153 / 109.153 / 110.153 / 111.153
   - CNAME www → `<your-username>.github.io`
5) After DNS propagates, enable **Enforce HTTPS** in Settings → Pages.