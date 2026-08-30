# Flossy Smiles Dental Implants & Aesthetics — Luxury Preview

A static, dependency-free redesign of the Flossy Smiles Dental Implants & Aesthetics
(Coral Gables, FL) website, built for GitHub Pages.

## Deploying to GitHub Pages

1. Create (or open) the repository `flossy-smiles-website` under the
   `godwingarrick198-cmyk` GitHub account.
2. Upload every file in this folder to the **root** of the repository
   (do not nest it inside a subfolder) — `index.html` must sit at the
   repository root alongside `styles.css`, `script.js`, `images/`, etc.
3. In the repository, go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to "Deploy from a branch."
5. Choose the branch (typically `main`) and the `/ (root)` folder, then save.
6. GitHub will publish the site at:
   `https://godwingarrick198-cmyk.github.io/flossy-smiles-website/`
7. Allow a few minutes for the first deployment and for HTTPS to provision.

No build step, backend, database, or server is required — every page is a
plain static HTML file.

## Project structure

```
flossy-smiles-luxury/
├── index.html
├── about.html
├── dental-implants.html
├── cosmetic-dentistry.html
├── patient-information.html
├── contact.html
├── 404.html
├── styles.css
├── script.js
├── robots.txt
├── sitemap.xml
├── README.md
└── images/
    ├── hero-patient-care.webp
    ├── implant-closeup.webp
    ├── implant-model-straight.webp
    ├── implant-model-angle.webp
    ├── aligner-invisalign.webp
    ├── xray-consultation.webp
    ├── lifestyle-confidence.webp
    ├── portrait-1.webp
    ├── portrait-2.webp
    ├── portrait-3.webp
    ├── portrait-4.webp
    └── mark-smile-arc.svg
```

## Notes on content accuracy

Business information (name, doctor, address, phone, email, hours, services,
established date, license, and NPI) was sourced from the practice's own
published website and verified business listings. Anything that could not be
verified — Dr. Gio's detailed biography, specific credentials, and current
insurance network participation — is clearly marked
`[VERIFY WITH FLOSSY SMILES]` in the relevant pages rather than invented.

No testimonials, prices, guarantees, or medical outcome claims have been
fabricated. Dr. Gio's photograph has not been included, since none was
provided; the About page uses a clearly labeled placeholder instead of
substituting another person's photo.

## Demo appointment form

The contact form on `contact.html` is a front-end-only demonstration. It
validates input in the browser, then shows a confirmation message stating
that no patient information was transmitted or stored, and that no
appointment was actually booked. Connecting it to a real booking system or
email service is a follow-up step, not part of this preview.

## Technical reliability checklist

- Fully static HTML/CSS/JS — no Node, PHP, Python, or database dependency
- All internal links and image paths are relative (no leading `/`)
- No external fonts, CDNs, analytics, or third-party scripts
- No external image hotlinks — all images live in `/images/`
- HTTPS-ready (GitHub Pages serves HTTPS automatically)
- Valid `robots.txt` and `sitemap.xml` with real, matching URLs
- Consistent canonical URLs across all pages
- Lazy-loaded non-critical images; hero image loads eagerly
- `prefers-reduced-motion` respected for all animation
