# Team Topnotch LLP website

A performance-first, responsive company website built from the supplied company profile.

## Preview

Open `index.html` directly in a browser, or serve the folder from any static host.

## Deployment

Upload `index.html`, `robots.txt`, and the complete `assets` folder without changing their relative structure. The site has no framework, package install, database, external font, or runtime dependency.

Before the final domain goes live:

1. Add the production URL as a canonical link in the page head.
2. Add the production URL to the Open Graph metadata.
3. Add a `sitemap.xml` containing the production URL and reference it from `robots.txt`.
4. Replace the email-based enquiry action with the client's CRM or form endpoint if server-side lead capture is required.
5. Re-run Lighthouse on the deployed HTTPS URL; ensure the host keeps Brotli/Gzip compression and long-lived caching enabled for files in `assets`.

## Verified quality

- Responsive desktop and mobile layouts visually checked in Chrome.
- Desktop Lighthouse: 100 Performance, 100 Accessibility, 100 Best Practices, 100 SEO.
- No browser console errors.
- Local images use WebP, responsive source selection, dimensions, lazy loading, and async decoding.

The full audit is saved in `output/lighthouse-desktop.json`.
