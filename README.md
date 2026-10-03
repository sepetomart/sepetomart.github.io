# Sepeto Mart — GitHub Pages Website

A responsive, mobile-first static storefront for Sepeto Mart, Dharwad.

## Files
- `index.html` — modern storefront, search, category filters, product cards, quantity controls, cart, WhatsApp ordering, and UPI QR section.
- `products.json` — 225 products from the supplied Sepeto Mart catalogue, including image URLs.
- `sepeto-upi-qr.png` — UPI QR for `SBIBHIM.INSTANT58532849532162184@sbipay`.

## Publish on GitHub Pages
1. Create a GitHub repository, for example `sepeto-mart`.
2. Upload `index.html`, `products.json`, and `sepeto-upi-qr.png` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then Save.
6. Wait for GitHub Pages to publish, then open the website URL shown on the Pages settings screen.

Keep all three files in the same folder. The site loads products from `./products.json`.

## Update products
Edit `products.json` and commit the changes. Each item uses:
`id`, `name`, `category`, `price`, `image`, `available`, `brand`.

## Important checks before launch
- The catalogue's image URLs are carried over from the provided sheet. Some Google thumbnail links may fail or change; replace them with stable, public HTTPS image URLs when possible.
- One source item had a blank product name. It is marked as `Product SM072 — name to be updated`; replace it with the correct name.
- Review prices and availability before accepting orders.
- The site uses WhatsApp number `+91 90367 04201` and UPI ID `SBIBHIM.INSTANT58532849532162184@sbipay`. Confirm both are correct.
- WhatsApp ordering opens a pre-filled message; the customer must press Send in WhatsApp.
- The UPI QR does not include a payment amount. Customers should verify the payee and enter the confirmed order amount in their UPI app.
- This is a static site; it does not process payments, reserve stock, or maintain an online database.
