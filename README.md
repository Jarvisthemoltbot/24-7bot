# 24-7bot.com

Simple static landing page for **24/7 Virtual Personal Assistant**.

## Folder structure
```
.
├── index.html                # Main page markup
├── assets/
│   ├── css/
│   │   └── style.css         # All site styles
│   └── js/                   # (Reserved) future JS files
└── .netlify/                 # Netlify metadata (auto-created)
```

## How it works
- `index.html` is the only page.
- All styles live in `assets/css/style.css`.
- The **Launch** and **Premium** buttons link to Stripe Checkout URLs.
- The **Free** tier uses a Netlify form (no backend required).

## Editing content (non‑technical)
1. Open `index.html`.
2. Update text in the sections:
   - **Hero** (top headline/description)
   - **How it works**
   - **Pricing**
   - **FAQ**
3. Save and push to GitHub — Netlify auto‑deploys.

## Stripe links
Update these in `index.html` when needed:
- Launch: `https://buy.stripe.com/14AcN560m5kIanqdYU5wI01`
- Premium: `https://buy.stripe.com/fZuaEX9cyfZm8fi1c85wI02`

## Netlify Form (Free guide)
Form is defined in `index.html`:
```html
<form name="free-guide" method="POST" data-netlify="true">
  <input type="hidden" name="form-name" value="free-guide" />
  ...
</form>
```
Submissions show in Netlify → Site → Forms.

## Deploy
This repo is connected to Netlify. Any push to `master` auto‑deploys to:
- **https://24-7bot.com**
