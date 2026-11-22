FindSarees — Storefront + Product Manager

FILES
index.html: customer storefront
admin.html: local product management dashboard
products.json: public catalog loaded by the storefront
app.js / style.css / sw.js / icons: storefront files

HOW TO USE
1. Upload all files and icons/ folder to the root of your GitHub Pages repository. Commit.
2. Open admin.html in your browser. It edits a local draft only. Import the existing products.json first if editing from a new device.
3. Add products, category, price, quantity, description and photo URL/path. Photos must be hosted separately, e.g. images/product1.jpg uploaded to your GitHub repository. This manager does not upload images.
4. Click Download products.json. Upload that file to your repository root, replacing the old products.json, and commit.
5. Wait for GitHub Pages to deploy, then reload the storefront. Clear cached site data if necessary.

SECURITY AND LIMITATIONS
- admin.html is NOT authenticated and must not be treated as a secure backend. It can be publicly viewed if deployed; its changes remain in the viewer's own browser, not on the live website. GitHub repository write permission is still required to publish.
- Browser local storage is device/browser specific; export backups. Import the current live catalog before editing on a different device.
- Product prices and stock are client-side display values, NOT secure payment or inventory enforcement.
- Storefront currently copies order inquiries only; no real payment integration.
- Shipping display: $10 CA, TX, WI, CO and Seattle WA; $8 elsewhere in USA, once per order. Shipping must be verified by a server-side checkout before charging.
