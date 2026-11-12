# Trixie Misheen website

This is a standalone static website for `trixiemisheen.site`. It is intentionally
separate from the DevSuite application and can be deployed independently.

## Preview locally

From the repository root:

```powershell
python -m http.server 8080
```

Open <http://localhost:8080> in a browser.

## Publish with GitHub Pages

1. Push this repository to GitHub.
2. Open the repository's **Settings → Pages**.
3. Under **Build and deployment**, choose **GitHub Actions**.
4. Run the **Deploy website** workflow manually once, or push a change under
   `website/` to trigger it.
5. Keep the included `CNAME` file at the published site root.
6. In your domain registrar's DNS panel, add:

   - `A` records for `@` pointing to GitHub Pages' current IP addresses
   - a `CNAME` record for `www` pointing to your GitHub Pages hostname

   GitHub will show the exact DNS values in **Settings → Pages → Custom domain**.
   Enable HTTPS after DNS finishes propagating.

Do not put registrar passwords, API tokens, or private keys in this repository.
# Trixie Misheen website

The public home for Trixie Misheen: software, experiments, support, and ideas.
This is a standalone static site for `trixiemisheen.site`, deployed independently
from the DevSuite desktop application.

## Public endpoints

- `/` — home, current work, and contact links
- `/support.html` — support center and developer resources
- `/privacy.html` — plain-language privacy policy
- `/project-devsuite.html` — DevSuite project showcase
- `/ideas.html` — public idea lab
- `/changelog.html` — project updates
- `/roadmap.html` — current direction and priorities
- `/docs.html` — documentation starting points
- `/status.html` — current service and release status
- `/downloads.html` — release information and future installers
- `/404.html` — friendly missing-page fallback
- `/sitemap.xml`, `/robots.txt`, and `/feed.xml` — discovery and updates

## Preview locally

From the repository root:

```powershell
python -m http.server 8080
```

Then open <http://localhost:8080>.

## Publish with GitHub Pages

Push the repository to GitHub and configure **Settings → Pages** to deploy from
the repository’s publishing branch. Keep [CNAME](./CNAME) at the repository
root. The custom domain should point to GitHub Pages, with HTTPS enabled after
DNS propagation finishes.

Do not put registrar passwords, API tokens, private keys, or personal support
attachments in this repository.
