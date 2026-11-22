# FindSarees — Modern PWA storefront

## Upload to GitHub Pages

1. Extract this ZIP.
2. In your existing `findsarees/FindSarees` GitHub repository, upload **all files and the `icons` folder contents** into the repository root, replacing the matching files. Ensure `index.html`, `app.js`, `style.css`, `sw.js`, and `manifest.webmanifest` are in the root. GitHub's browser upload may need a desktop browser for convenient multi-file replacement.
3. Commit changes. Your GitHub Pages URL stays the same.
4. Refresh the website; if the old version remains installed, close/reopen the PWA or clear site data.

## Catalog management

Edit the `PRODUCTS` array near the top of `app.js` to replace the eight **sample** products and prices. The current cards use decorative placeholders, **not actual merchandise photographs**. For real photos, add files and modify the product card markup to show `<img>` elements.

## Shipping

- $10 per order: California (CA), Texas (TX, including Dallas), Wisconsin (WI), Colorado (CO), Seattle city in Washington (WA).
- $8 per order: all other US states and DC.
- Customers select a state and enter a city. Washington requires a city. City names are not address-validated, so **the server-side checkout must verify shipping destination and apply the correct rate**. Alaska and Hawaii are included at $8 per the provided 'all states' rule.
- Taxes are not calculated.

## Payment status — important

This is a **demo storefront** with a working multi-item cart, estimated shipping, and a copyable order inquiry. It **does not process payments**. Do not advertise it as a live checkout until you connect a secure server-side payment provider and verify the destination shipping charge there. GitHub Pages cannot safely hold Stripe secret keys or create Checkout Sessions by itself. Never put private Stripe keys in browser JavaScript.

## PWA

Includes install manifest, app icons, and offline service worker. Android Chrome may offer Install App; on iPhone Safari use Share > Add to Home Screen.
