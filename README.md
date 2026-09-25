# SmartShoes — GitHub Pages storefront

A mobile-first static footwear storefront for Pakistan. The current implementation includes:

- Branded responsive home page
- Product catalog with search, category, price, and sorting controls
- Product details with size selection
- Persistent localStorage shopping cart
- GitHub Pages-compatible root `404.html`
- Accessible semantic markup and responsive styling

## Run locally

Because this is a static site, serve the folder with any local server:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Publish with GitHub Pages

1. Push the repository to GitHub.
2. Open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select `main` and the `/ (root)` folder, then save.
5. Open the generated Pages URL.

All links use relative paths so the site works at a project URL such as `/my/`.

## Production configuration

Product data is currently in `js/app.js` and image URLs use Unsplash placeholders. Replace these with owned/licensed product images and connect a real catalog source before launch.

GitHub Pages cannot securely create orders, authenticate users, manage inventory, send email, or process payments. Add a serverless/backend service for checkout and payment verification. Never commit payment private keys, database credentials, admin secrets, or other private API keys.

Before launch, replace placeholder delivery, return, contact, and legal copy with SmartShoes' actual policies.
