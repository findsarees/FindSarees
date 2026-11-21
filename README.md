# FindSarees PWA

A free-hostable, installable storefront prototype for Android and iPhone.

## Publish free using GitHub Pages
1. Create a public GitHub repository (e.g. `findsarees`).
2. Upload the **contents** of this folder to the repository root.
3. Go to repository Settings → Pages → Build and deployment → Deploy from a branch; select `main` and `/ (root)`, then Save.
4. Wait for the HTTPS site URL shown under Pages.
5. Android: open the HTTPS URL in Chrome and choose Install app or Add to Home screen. iPhone: open in Safari, tap Share, then Add to Home Screen (or Open as Web App, depending on iOS).

## Before taking real orders
- Replace emoji placeholders with actual product photos, names, variants, inventory and prices.
- Connect a payment processor and an order backend. The current Copy Order Summary button does **not** place an order or take payment.
- Confirm shipping, returns, privacy, taxes and customer support information.
- Replace the sample products; $35 frocks and $10 USA shipping reflect the initial requirements.
- When updating files, increment `CACHE` version in `sw.js` so installed clients refresh cached assets.

The service worker supports cached browsing of previously visited app assets, but this is not an offline ordering system.
