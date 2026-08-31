# Wartlon Free Pattern Library

This version is ready to upload to GitHub Pages and already contains:

- Gosling preview + PDF
- Halloween Goose preview + PDF
- Separate SEO-friendly page for each free pattern
- Etsy calls to action
- Mobile layout

## Publish on GitHub Pages

1. Create a new public GitHub repository, for example `free-cross-stitch-patterns`.
2. Upload the CONTENTS of this folder to the repository root.
3. Open Settings → Pages.
4. Under Build and deployment choose `Deploy from a branch`.
5. Select `main` and `/ (root)`, then Save.

Your site will then be available at:
`https://YOUR-USERNAME.github.io/free-cross-stitch-patterns/`

To add another freebie, copy one of the folders inside `patterns/`, add its image to `assets/images/`, its PDF to `assets/pdf/`, and add a card to `index.html`.


## Blog

The site now includes:
- `/blog/` — blog index
- `/blog/cross-stitch-fabric-size-calculator/` — first article with a working calculator

To add another article, duplicate the existing article folder, rename it with a short lowercase hyphenated slug, edit its `index.html`, and add a new article card to `/blog/index.html`.


## Google Analytics 4

GA4 measurement ID: `G-FTGFHNVJ15`

The site includes:
- consent-based analytics (analytics storage denied until accepted)
- `free_pattern_download` event for PDF links
- `etsy_click` event for outbound Wartlon Etsy links
- `fabric_calculator_use` event for successful calculator use
- `/privacy.html` with visitor controls for analytics consent

After deployment, use Google Analytics Realtime / DebugView to confirm incoming traffic and events.


## Regional Consent Mode

Regional defaults are now configured using Google's built-in `region` parameter:
- EEA + UK + Switzerland: `analytics_storage = denied` until consent.
- Other regions: `analytics_storage = granted` by default.
- `ad_storage`, `ad_user_data`, and `ad_personalization` stay denied everywhere.

The site still provides a visible analytics preference control and privacy page.


## SEO setup

Live site: https://wartlon.github.io/wartlon-free-cross-stitch-patterns/

Added:
- `sitemap.xml`
- `robots.txt`
- canonical URLs for the main page, blog, calculator article and free-pattern pages

After deployment, submit this sitemap in Google Search Console:
https://wartlon.github.io/wartlon-free-cross-stitch-patterns/sitemap.xml
