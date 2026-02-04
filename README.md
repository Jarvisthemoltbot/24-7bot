# 24-7bot.com

Simple static landing page for **24/7 Virtual Personal Assistant**.

## Folder structure
```
.
├── index.html                # Main page markup
├── success.html              # Form success page
├── assets/
│   ├── css/
│   │   └── style.css         # All site styles
│   └── js/                   # (Reserved) future JS files
├── vercel.json               # Vercel configuration
└── .gitignore                # Git ignore rules
```

## How it works
- `index.html` is the main landing page.
- All styles live in `assets/css/style.css`.
- The **Launch** and **Premium** buttons link to Stripe Checkout URLs.
- The **Free** tier uses Formspree (form submissions go to Formspree dashboard).

## Editing content (non‑technical)
1. Open `index.html`.
2. Update text in the sections:
   - **Hero** (top headline/description)
   - **How it works**
   - **Pricing**
   - **FAQ**
3. Save and push to GitHub — Vercel auto‑deploys.

## Stripe links
Update these in `index.html` when needed:
- Launch: `https://buy.stripe.com/14AcN560m5kIanqdYU5wI01`
- Premium: `https://buy.stripe.com/fZuaEX9cyfZm8fi1c85wI02`

## Formspree Form (Free guide)
Form is defined in `index.html`:
```html
<form name="free-guide" method="POST" action="https://formspree.io/f/YOUR_FORM_ID">
  <input type="hidden" name="_next" value="https://24-7bot.com/success.html" />
  ...
</form>
```
Submissions show at: https://formspree.io/forms/YOUR_FORM_ID

## Deploy
This repo is connected to Vercel. Any push to `master` auto‑deploys to:
- **https://24-7bot.com**

## Analytics
Plausible Analytics is configured for privacy-friendly tracking.
