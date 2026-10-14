# DealAtlas — multi-affiliate website

Static, responsive affiliate product discovery site, suitable for GitHub Pages.

## Features
- Search and category filtering
- Multiple merchant/network links per catalog (one link per product card; duplicate a product for multiple merchant offers)
- Safe outbound links with `rel="sponsored noopener noreferrer"`
- Local catalog editor, JSON import/export
- Affiliate disclosure, mobile responsive layout
- No paid API or build step

## Publish
1. Create a **public** GitHub repository named `multi-affiliate-site`.
2. Upload `index.html`, `products.json` and `README.md` to its default branch.
3. In **Settings → Pages**, select **Deploy from a branch**, branch `main`, folder `/ (root)` and save.
4. The site should become available at `https://YOUR_USERNAME.github.io/multi-affiliate-site/` after deployment.

## Manage products
The Manage section is a **browser-local editor**, not a secure admin dashboard. Add products, export `products.json`, then commit that file to the repository to update the public catalog. The catalog loads from `products.json` and falls back to example cards if it is empty. Example cards do not contain affiliate links.

Only add approved affiliate links after joining the merchant program. Avoid false price, stock, coupon or review claims. Review each program's rules on link placement and disclosures.

## Limitations / next steps
GitHub Pages is static: no authentication, central database, scheduled crawlers or secret API keys. Add a hosted backend with authentication for a true admin dashboard and AI automation. Never place credentials or API keys in these public files.
