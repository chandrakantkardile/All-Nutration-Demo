# All Nutrition – Shop Website (Demo)

A responsive, mobile-first demo website for **All Nutrition**, a nutrition and supplement shop in Georai, Tal. Newasa, Dist. Ahilyanagar, Maharashtra. Built as a single self-contained HTML file (HTML + CSS + vanilla JavaScript), with no build step and no dependencies.

## Features

- **Storefront:** hero section, trust badges, 16 sample products, category filter (Protein, Gainers, Vitamins, Pre/Post Workout, Health Foods)
- **Cart and orders:** add/remove items, quantity control, total, order with Cash on Delivery, or order directly on WhatsApp
- **Customer panel:** simple demo login (name + mobile) and "My Orders" history
- **Admin panel:** dashboard (orders, revenue, products), order status toggle (Pending / Delivered), add and delete products
- **Multi-language:** English, Marathi, Hindi, with a language switcher in the header (choice is remembered)
- **WhatsApp:** floating chat button and a community join section
- **Location and contact:** address, Google Maps link, call button, shop timing
- **Theme:** light and dark mode, follows the device setting
- **Mobile friendly:** works on all screen sizes, safe-area support for modern phones

## Getting Started

No installation needed.

1. Clone the repository
   ```bash
   git clone <your-repo-url>
   cd all-nutrition
   ```
2. Open `all-nutrition.html` in any modern browser.

To serve it locally instead:

```bash
npx serve .
```

## Project Structure

```
all-nutrition/
├── all-nutrition.html   # Entire site (markup, styles, scripts)
└── README.md
```

## Demo Credentials

| Panel | Access |
|-------|--------|
| Customer | Any name + mobile number (demo login) |
| Admin | Footer → "Admin Login", password: `admin123` |

> The admin password is hardcoded for demo purposes only. Do not use this approach in production.

## Customization

- **Shop details:** search for `9960842249` (phone) and the address text in `all-nutrition.html` and replace as needed.
- **Products:** edit the `DEF` array in the script section (name, category, price, MRP, emoji, tag).
- **Translations:** edit the `TR` object. Each entry is `"English text": "Marathi|Hindi"`.
- **Colors:** change the CSS variables in `:root` (`--pr` primary, `--ac` accent).
- **Product images:** products currently use emoji and colored cards. Replace the `.pi` block in `rs()` with `<img>` tags once real photos are available.
- **Map:** the Google Maps link uses a search query. Replace it with the shop's exact Google Maps link.

## Data Storage (Important)

Products, cart, orders, login, and language are stored in the browser's `localStorage`. This means:

- Data is visible only on the same device and browser.
- Clearing browser data resets everything.
- Orders placed by customers do **not** reach the shop owner automatically (WhatsApp order is the real channel in this demo).

## Roadmap

Planned for a production version:

- [ ] React frontend with reusable components
- [ ] Spring Boot REST API with a database (MySQL/PostgreSQL)
- [ ] Secure authentication (JWT) for customers and admin
- [ ] Real product images and image upload from the admin panel
- [ ] Online payments (UPI / Razorpay)
- [ ] Order notifications to the shop owner
- [ ] Product names and descriptions in all three languages from the database

## Contact

**All Nutrition**
At-Post Georai, Tal. Newasa, Dist. Ahilyanagar, Maharashtra
Phone / WhatsApp: 9960842249

## License

This is a demo project prepared for a client presentation. All rights reserved.
