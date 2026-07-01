# The GoodLife Foundation (GLAF) — Website

A 9-page static site for The GoodLife Foundation, built with plain HTML5, CSS3 and vanilla JavaScript. No build step, no dependencies.

## Pages
- `index.html` — Home
- `about.html` — About Us
- `programs.html` — Our Programs
- `projects.html` — Projects & Impact
- `get-involved.html` — Get Involved
- `donate.html` — Donate
- `partners.html` — Partners
- `news.html` — News & Events
- `contact.html` — Contact Us

Each file is fully self-contained (CSS and JS are embedded inline), so any page works on its own with no external folders required.

## Deploying on Vercel

1. Push this folder to a GitHub repo (all files at the repo root).
2. In Vercel: **Add New Project** → import the repo.
3. Leave the framework preset as **Other** and leave the build command / output directory blank — this is a static site.
4. Deploy.

`vercel.json` in this repo enables **clean URLs**, so:
- `/about` serves `about.html`
- `/programs` serves `programs.html`
- etc.

All internal navigation links already point to the clean, extensionless paths.

## Still to connect before going fully live
- **Forms** (contact, volunteer registration, donation, partnership inquiry) currently show a client-side "success" message only — they don't send data anywhere. Wire them to a form service (e.g. Formspree) or a Vercel serverless function.
- **Donation payments** — the Donate page has a payment-method placeholder; connect a gateway such as Paystack or Flutterwave.
- **Google Maps embed** on the Contact page is a placeholder — swap in a real embed once you have an address.
- **Real photography** — all image slots are labeled gradient placeholders; replace with real photos as they become available.
- **CAC registration, annual report, financial statements, partner logos** — placeholders throughout the site, ready to populate once available.
