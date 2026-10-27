# Sunchem — static HTML site

Static HTML/CSS/JS version of the Base44 app (same layout, colors, Inter font, icons and animations).
No build step or server needed: open `index.html` in a browser, or upload the three files to any static host.

- `index.html` — page markup
- `styles.css` — compiled Tailwind CSS (same config/theme as the Base44 export)
- `script.js` — nav, scroll reveal, hero parallax, product tabs, contact form

## Contact form
Base44 stored enquiries in its own database, which a static site doesn't have. In `script.js`, set
`FORM_ENDPOINT` to a form service URL (e.g. Formspree) to receive submissions. While it is empty,
submitting opens the visitor's email app with the enquiry pre-filled for `enquiries@sunchem.in`.

## Images
The hero image and logos are loaded from Base44's media CDN. To make the site fully independent,
download them into an `assets/` folder and update the `src` URLs in `index.html`.
