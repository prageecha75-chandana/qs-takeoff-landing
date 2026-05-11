# [Product] landing page

Static landing page for the [Product] QS takeoff tool. No build step — `index.html` is the production source.

## Local preview

Open `index.html` in a browser, or serve the directory with any static server:

```
npx serve .
```

## Deploy

Vercel auto-detects this as a static site. Push to the linked GitHub repo and a deployment is created.

## Follow-ups before launch

1. **Product name + domain.** Find-and-replace `[Product]` and `[productdomain]` once decided.
2. **Formspree endpoint.** In `index.html`, search for `YOUR_FORMSPREE_ID` and replace with the form's hashid from <https://formspree.io>. While the placeholder is in place the form falls back to a visual-only confirmation.
3. **Watch demo.** The hero button is disabled (`pointer-events: none; opacity: .45`). Enable it once a real demo video URL exists.

## Files

- `index.html` — entire page (HTML + CSS + inline SVGs + tiny form JS).
- `robots.txt` — allow-all.
- `extracted/` — original design handover ZIP unpacked. Ignored by git.
