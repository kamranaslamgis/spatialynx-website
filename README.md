# Spatialynx — starter website

A complete, responsive static website for **spatialynx.tech**. No build tools, backend, paid plugins or JavaScript frameworks are required.

## Preview locally

Open `index.html` in a web browser. For a more accurate preview, run `python -m http.server 8000` in this directory and open http://localhost:8000.

## Publish on GitHub Pages

1. Create a **public** GitHub repository, e.g. `spatialynx-website`.
2. Upload all the files **including the `assets` folder** to the repository root.
3. Navigate to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**; select `main` and `/ (root)`; save.
4. Wait for GitHub Pages to show the default site address. Test it before connecting your custom domain.
5. In GitHub **Settings → Pages → Custom domain**, enter `spatialynx.tech` and save.
6. In Hostinger DNS management for `spatialynx.tech`, set the website records recommended in GitHub's current documentation (usually four apex `A` records pointing to GitHub Pages and an optional `www` CNAME to your GitHub username's pages host). Remove *conflicting website* A/AAAA/CNAME records. **Preserve MX, SPF, DKIM and DMARC records** to avoid disrupting `contact@spatialynx.tech`.
7. Verify domain and HTTPS status in GitHub Pages. Enable **Enforce HTTPS** once available. DNS propagation can take time.

**Important:** Confirm GitHub's latest DNS record values from https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site before changing Hostinger DNS. Do not delete your domain or mailboxes.

## Change content

- Text and section structure: `index.html`
- Colors, fonts, layout and mobile behavior: `styles.css`
- Mobile navigation and copyright year: `script.js`
- Logos and Earth artwork: `assets/`

## Contact

The contact button opens an email draft to `contact@spatialynx.tech`. A static GitHub Pages site cannot process an HTML contact form by itself. Add a form provider or backend later if needed.

## Branding

The supplied PNG logo is derived from previously approved Spatialynx concept artwork. It has been made approximately transparent for web usage. The final production-ready identity may benefit from a manually redrawn vector/SVG asset.

## Launch checklist

- Check every section and link on desktop and mobile.
- Ensure the mailbox works before publishing.
- Confirm your organization's incorporation status before adding legal suffixes or registration claims.
- Replace concept branding with finalized vector logos if required.
- Connect Google Search Console and submit `sitemap.xml` after domain setup.


## Founder page (new)
- `founder.html` is a standalone biography page, linked from the header, footer, and home page.
- LinkedIn button goes to `https://www.linkedin.com/in/kamran-aslam-04280a6b/`.
- **Profile picture still needs to be supplied:** LinkedIn blocked direct access to the profile image. The included `assets/founder-photo.svg` is a clearly labeled branded placeholder, **not the founder's portrait**. To add the real photo, save a professional photo as `assets/founder-photo.jpg`, then change `src="assets/founder-photo.svg"` to `src="assets/founder-photo.jpg"` in `founder.html` and update its alt text to `Portrait of Kamran Aslam`. Use a photo you own or have permission to use.
