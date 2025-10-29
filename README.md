# UnionDeal — Great Prices, UK‑Wide Delivery

UnionDeal is a portfolio-friendly demo e-commerce website built with **HTML, CSS, JavaScript, and PHP**. It’s intentionally lightweight and easy to run locally or on a simple PHP host. The goal is to showcase front-end UI, client-side interactivity, and basic server-side logic (cart handling and order persistence).

---

## Features

* Responsive product catalogue and search
* Add to cart (AJAX) and simple cart management
* Checkout form that writes orders to `data/orders.txt` (JSON lines)
* Product data served from a PHP file (easy to replace with a DB)
* Clean, modern design aimed at portfolio presentation

---

## What’s included

* `public/` — public-facing site files

  * `index.html` — homepage and product grid
  * `cart.php` — server-rendered cart + checkout form
  * `checkout.php` — processes orders
* `assets/` — static assets

  * `css/style.css` — site styling
  * `js/app.js` — client-side interactivity
  * `images/` — product images (placeholders)
* `api/` — small PHP back-end

  * `products.php` — product data
  * `products_json.php` — product JSON endpoint
  * `cart.php` — cart API (add/remove/update/view)
* `data/` — runtime data (orders.txt)

---

## Quick setup (run locally)

1. Ensure you have **PHP 8+** installed.
2. Place the project folder in your web server root or run PHP built-in server from the project root:

```bash
php -S localhost:8000 -t public
```

3. Create a writable `data/` directory next to `public/`:

```bash
mkdir data
chmod 777 data
```

4. Open `http://localhost:8000` in your browser.

Notes: place demo product images in `assets/images/` (see the image README in the project export).

---

## Customisation suggestions (portfolio talking points)

* Swap `api/products.php` to return products from a real database (MySQL / SQLite) and add migrations.
* Harden the checkout: use prepared statements, input validation, CSRF tokens, and proper email confirmations.
* Add user accounts (registration, login) with password hashing and session security.
* Integrate payment sandbox (Stripe test mode) and show secure server-side processing.
* Improve UI with React/Vue or add server-side rendering and caching.

---

## Security & Disclaimer

This project is a demo for portfolio purposes. It intentionally keeps server-side logic minimal and is **not** production hardened. Do not use this code as-is for a live store that handles real payments or sensitive user data. If you intend to deploy publicly, implement proper security best practices (input validation, CSRF protection, prepared statements, HTTPS, XSS protections, and secure file permissions).

---

## License

MIT — feel free to adapt for your portfolio. Please keep attribution to the original author.

---

## 👤 Author

**Michael Semera**
- LinkedIn: [Michael Semera](https://www.linkedin.com/in/michael-semera-586737295/)
- GitHub: [MichaelKS123](https://github.com/MichaelKS123)
- Email: michaelsemera15@gmail.com

## 📞 Contact & Support

For questions, suggestions, or collaboration opportunities:
- Open an issue on GitHub
- Email: michaelsemera15@gmail.com
- LinkedIn: [Michael Semera](https://www.linkedin.com/in/michael-semera-586737295/)
