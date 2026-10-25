# Aqib Mehmood | Portfolio

Static, dependency-free portfolio (HTML + CSS + vanilla JS). No build step.

The portfolio includes a responsive developer-workspace project explorer, GitHub and Instagram links, and a floating browser-based assistant. The assistant can jump to relevant case studies and offer interview scheduling through WhatsApp.

## Structure
```
index.html
css/style.css
js/main.js
assets/
  profile.jpg                              <- ADD your photo (square, ≥600×600)
  Aqib_Mehmood_AI_ML_Engineer_CV_2k26.pdf  <- ADD your CV (for the Download buttons)
  favicon.svg
  profile-fallback.svg                     (shown until profile.jpg exists)
```

## Before going live
1. Put `profile.jpg` and the CV PDF inside `assets/`.
2. Replace `https://your-domain.com/` in `index.html` (canonical + JSON-LD) with your real domain, and make the `og:image` URL absolute.
3. Contact form: create a free form at https://formspree.io and replace `YOUR_FORM_ID` in the form `action`.
   Until then the form falls back to opening the visitor's email client (mailto).
4. Optional: add a GitHub link in the top bar / footer.

## Run locally
```
python -m http.server 8000
# open http://localhost:8000
```

## Deploy
Drag-and-drop the folder to Netlify / Vercel / Cloudflare Pages, or push to a GitHub repo and enable GitHub Pages.
