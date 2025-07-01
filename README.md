# AccuSalt Redirect Site

This is a simple static redirect site for Netlify. It detects mobile vs desktop devices and redirects users to:

- 🖥️ Desktop: https://accusalt-desktop.netlify.app
- 📱 Mobile: https://accusalt-mobile.netlify.app

## Deployment

1. Push this repo to GitHub.
2. Log into Netlify, choose **"Add new site" → "Import from Git"**.
3. Connect your GitHub repo (e.g. `accusalt-redirect`).
4. For build settings:
   - Build command: *(leave blank)*
   - Publish directory: `.`

Netlify will deploy it as a static site (e.g. `accusalt.netlify.app`). You can also add a custom domain later.

> 🔧 You can customize `destination` URLs in `index.html` if your Netlify URLs change.

---

## How it works

- The JavaScript checks `navigator.userAgent` for mobile indicators.
- Redirects using `window.location.replace(location)`.
- Includes a fallback link for manual navigation.

---

Feel free to edit and customize!

