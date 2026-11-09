# Northstar Tech — GitHub Pages storefront

This repository contains a static, responsive electronics catalogue built from the product images supplied with the project. **There is no build step, package installation, server, or framework required.**

## Preview locally

Open `index.html` in a browser. For a local web-server preview, run one of these commands from this folder:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Publish with GitHub Pages

1. Create a new GitHub repository.
2. Extract the website ZIP on your computer.
3. Upload the **contents** of the extracted folder to the repository's top level. Make sure `index.html`, `images/`, `assets/`, and `inventory.html` are at the repository root — do not upload the ZIP file itself.
4. On GitHub, open the repository's **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select your publishing branch (usually `main`) and folder **`/(root)`**, then save.
7. Wait for the Pages deployment to finish. GitHub will show the published site URL in **Settings → Pages**.

The site uses relative image and page links, so it supports both a user/organisation site and a project site published beneath a repository path. `.nojekyll` is included so GitHub Pages serves the static files directly.

## What's included

- `index.html` — image-rich homepage, visual category cards, searchable/filterable catalogue, product detail views, image zoom/lightbox, and enquiry bag.
- `images/products/` — supplied product images used in the catalogue.
- `images/unclassified/` — supplied images kept aside for manual review.
- `inventory.html` — image inventory with previews and file paths.
- `assets/image-inventory.csv` — downloadable inventory spreadsheet.
- `assets/products.json` — catalogue data.
- `assets/records.json` — source image audit records.
- `404.html` — custom not-found page.
- `.nojekyll` — tells GitHub Pages not to run Jekyll processing on the static site.
- `.gitignore` — ignores common operating-system files.

## Image audit

- 67 image files found in the supplied ZIP.
- 65 unique images integrated into the website.
- 2 exact duplicate files were not repeated in the product catalogue.
- 5 unique images are kept in the manual-review category because the product identity is unclear.
- All catalogue image paths were checked against the website files; no missing catalogue image files were found.
- Supplied image files are preserved in their original formats and dimensions.

## Before accepting orders

This is a front-end catalogue demonstration. It does not process payments, submit orders, calculate shipping, or connect to live inventory. Product names are generic catalogue labels where an exact model could not be established visually. No prices, specifications, stock levels, ratings, or discounts have been invented.

Before going live as a real shop, add the business-approved name and logo, contact details, accurate product titles and specifications, prices, delivery/returns information, privacy terms, and a secure checkout or enquiry service. Confirm that you have permission to publish all supplied photographs.
