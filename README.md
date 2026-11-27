# Bookline landing page

Static, single-file landing page for Bookline, an AI assistant for HVAC companies (an Entrext venture).
No build step, no dependencies. The only external request is Google Fonts (Inter).

## Run locally
Open `index.html` in a browser, or serve the folder:

    python3 -m http.server 8000

## Scroll
Smooth scrolling, in-view reveals and light parallax use [Locomotive Scroll](https://github.com/locomotivemtl/locomotive-scroll) v4.1.4, loaded from jsDelivr. It switches off automatically for visitors who prefer reduced motion.

## Deploy
- **GitHub Pages:** Settings > Pages > deploy from the `main` branch, root folder.
- **Vercel / Netlify / Cloudflare Pages:** import the repo, no build command, output directory `.`

## Collect emails
In `index.html`, set `FORM_ENDPOINT` (near the top of the script) to a Formspree, Google Form or your own API URL.
It receives `POST {"email": "..."}` as JSON. Until then the form only shows the thank-you message.

## Before launch
- The company name "Summit Heating & Air" and the sample conversations are placeholders.
- The trust cards ("You stay in control", "Humans can step in", etc.) describe principles for the product. Make sure each is true before launch.
