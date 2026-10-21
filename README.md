# Roofing Solutions Ltd. - one-page site

Static site, no build step. Deploy the folder as-is.

## Deploy on Vercel

Option A (dashboard): vercel.com > Add New > Project > drag this folder in, Framework Preset = Other, Build Command empty, Output Directory empty, Deploy.

Option B (CLI):

    npm i -g vercel
    vercel --prod

## Before going live

- Replace dummy details: phone, WhatsApp, email, address, hours, town names, reviews, stats (search index.html for "Manchester", "0161", "07700", "info@roofingsolutionsltd").
- Put the logo in the "Your logo" box (header and footer).
- Quote form: in index.html change `var DEMO=true` to `var DEMO=false` and set the real email in the form `action` (FormSubmit). First submission triggers a FormSubmit activation email.
- Privacy Policy link in the footer points to "#", add a page or link.

## Files

- index.html  - the whole site
- images/     - client photos + stock photos (images/stock, Unsplash licence)
- vercel.json - clean URLs, caching and security headers
