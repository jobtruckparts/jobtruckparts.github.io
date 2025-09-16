# Job Truck Parts — Static Site (GitHub Pages)

A fast, static marketing site for **Job Truck Parts**, deployed from the `main` branch on **GitHub Pages**.

## 🧭 Contents
- [`index.html`](./index.html) — Landing page
- [`css/`](./css) — Stylesheets
- [`js/`](./js) — Scripts (vanilla)
- [`images/`](./images) — Optimized images (WebP + fallbacks if needed)
- [`favicon/`](./favicon) — Favicons & web manifest
- [`CNAME`](./CNAME) — Custom domain for Pages
- [`.nojekyll`](./.nojekyll) — Disable Jekyll processing on Pages


## 🚀 Local Development
No build step is required. Use any static server to preview:
```bash
# Python 3
python3 -m http.server 5500

# or Node
npx http-server -p 5500
```
Then open: http://localhost:5500

## 🔁 Deploying to GitHub Pages
1. Push changes to the `main` branch.
2. In **Repository → Settings → Pages**, set:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main` (root)
3. Confirm the **Custom domain** matches the `CNAME` file.

> Pages will auto‑deploy after each push. No Actions workflow is needed for a plain static site.

## 🌐 Custom Domain (DNS)
If using a root/apex (e.g., `jobtruckparts.com`), add **A records** pointing to GitHub:
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```
For the `www` subdomain, add a **CNAME** to `<your-user>.github.io` (or this repo’s Pages hostname).  
Keep the repo’s **`CNAME`** file set to your domain so Pages issues HTTPS automatically.

## 🧹 Project Hygiene
- See [`.gitignore`](./.gitignore) for common clutter to exclude.
- Use [`.nojekyll`](./.nojekyll) if you ever add folders that start with `_`.
---