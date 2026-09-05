# Smile Architect Dental & Cosmetic Clinic — Website

A single-page, mobile-friendly website for Smile Architect Dental & Cosmetic Clinic
(Dr. Karishma Dalvi), built as plain HTML/CSS/JS so it can be hosted for free on
GitHub Pages — no build step required.

## What's in here

```
index.html      – the whole site (one page, sections linked from the nav)
css/styles.css  – all styling
js/script.js    – mobile menu + photo gallery lightbox
images/         – logo, favicons, and the before/after photos used on the site
robots.txt      – tells search engines they can crawl the site
sitemap.xml     – helps search engines index the site
```

## How to put this on GitHub Pages

1. Create a new repository on GitHub (e.g. `smile-architect-website`).
2. Upload every file in this folder to the repository, **keeping the folder
   structure** (`css/`, `js/`, and `images/` must stay as subfolders).
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`,
   pick the `main` branch and the `/ (root)` folder, then **Save**.
5. GitHub will give you a live link that looks like:
   `https://<your-username>.github.io/<repo-name>/`
   It can take a minute or two to go live the first time.

### If you buy a custom domain (e.g. smilearchitectpune.com)
Add a file called `CNAME` (no extension) in the root of the repo containing just
your domain, e.g.:
```
www.smilearchitectpune.com
```
Then point your domain's DNS at GitHub Pages following GitHub's custom-domain
instructions, and set the same domain in the repo's Pages settings.

## Please double-check / update before publishing

I filled in a few details from what was visible in the photos you sent. Please
confirm or correct these before going live:

- **Address** — used "Shop No. 19, Sunshree Suntech, NIBM Post Office Road,
  Kondhwa Khurd, Pune" from one of your flyers. Confirm this is current.
- **Clinic hours** — I placed a placeholder of Mon–Sat, 10 AM–8 PM. Update the
  "Clinic hours" block in `index.html` (search for `Clinic hours`) with your
  real timings.
- **Phone number** — every Call/WhatsApp button uses **9975356797** as you
  requested. If this ever changes, search-and-replace `9975356797` and
  `919975356797` throughout `index.html`.
- **Domain in SEO tags** — the `<meta>` tags and structured data currently use
  a placeholder domain `https://www.smilearchitectpune.com/`. Once you know
  your final GitHub Pages URL or custom domain, update the `canonical`,
  `og:url`, `og:image`, `twitter:image`, and the JSON‑LD block near the top of
  `index.html` to match it — this is what makes Google Search and social
  sharing previews work correctly.
- **Map** — the embedded map currently searches for "Kondhwa Khurd, NIBM Post
  Office Road, Pune". For a pin-accurate map, replace the map `src` in
  `index.html` with an embed link from Google Maps for your exact location
  (Share → Embed a map on your own listing).
- **Doctor bio** — the About section has general, honest copy since I wasn't
  given Dr. Dalvi's specific qualifications/years of experience. Feel free to
  add degrees, college name, or years in practice for extra credibility.

## Adding more before/after photos later

Drop a new image into `images/`, then copy one of the `<button class="gallery-item">`
blocks in `index.html` (inside `<section id="gallery">`) and change the image
path, alt text, and caption.

## SEO notes

- Title, meta description, Open Graph/Twitter tags, and JSON-LD `Dentist`
  structured data are already in place.
- All images have descriptive `alt` text mentioning the treatment and Pune.
- `robots.txt` and `sitemap.xml` are included — after publishing, submit the
  site in [Google Search Console](https://search.google.com/search-console)
  and paste in your sitemap URL for faster indexing.
- Once live, also create a free **Google Business Profile** for the clinic
  and link it — that matters as much as the website for local "dentist near
  me" searches in Kondhwa/Pune.
