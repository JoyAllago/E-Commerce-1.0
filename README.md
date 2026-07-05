# 🌸 YsabelShop

An original pink-aesthetic e-commerce marketplace concept, built with React + Vite. Inspired by the *features* of popular marketplace apps (search, categories, cart, delivery options, checkout) but with entirely original branding, copy, and a soft blush/rose/cream visual identity.

## Features

- **Login & Register pages** — email/password login, full account creation with confirm password
- **Shop / Home page** — sticky header with logo, search bar, category menu, delivery-location strip, and a cart icon with a live item-count badge
- **Product grid** — cards with image placeholder (emoji), name, price + discount, rating, sold count, and delivery label
- **Cart** — slide-in panel, quantity +/- controls, remove item, subtotal/delivery/total breakdown
- **Delivery options** — Standard vs Express, each with its own fee and estimated arrival window
- **Checkout** — full order summary, delivery form, Place Order button, and an order-success confirmation screen

## Tech stack

- React 18 (functional components + hooks only)
- Vite 5
- Plain CSS (no UI framework) — all styling lives in `src/App.css`

## Getting started

```bash
npm install
npm run dev
```

Then open the printed local URL (usually `http://localhost:5173`) in your browser.

To build for production:

```bash
npm run build
npm run preview
```

## Project structure

```
blushmart/
├── index.html
├── package.json
├── README.md
└── src/
    ├── main.jsx
    ├── App.jsx
    ├── App.css
    ├── data/
    │   └── products.js
    └── components/
        ├── Header.jsx
        ├── ProductCard.jsx
        ├── Cart.jsx
        ├── Login.jsx
        ├── Register.jsx
        ├── Delivery.jsx
        └── Checkout.jsx
```

## Notes

- This is a front-end demo: login/register accept any filled-in values (no real backend/auth), and "Place Order" simulates a successful checkout.
- Product images are represented with large emoji on soft gradient tiles to keep the demo dependency-free — swap in real photos by replacing the `emoji` field in `src/data/products.js` with an `<img>`.
- Prices are shown in ₱ (Philippine peso) — change the currency symbol in `ProductCard.jsx`, `Cart.jsx`, and `Checkout.jsx` if needed.
