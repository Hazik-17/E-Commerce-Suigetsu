# Suigetsu Clothing Web Application

Suigetsu Clothing Web Application is a simple online store for browsing and buying clothes.

## About This Project

This project was built as a final year diploma project. It started as basic coding practice and grew into a working web application during the learning journey. The goal was to build a small e-commerce site to learn HTML, CSS, JavaScript, PHP and how to connect to a database.

## What This Website Does

This website lets users view products, sign up, log in, add items to a cart, and check out by uploading payment proof. It includes a separate admin area to add and manage products, view orders, and see payments.

Key user features:

- Browse products with images and descriptions.
- Search for items.
- Create an account and log in.
- Add products to cart and see cart totals.
- Upload payment proof to complete an order.
- View order history and profile information.

## Technologies Used

- HTML — page structure (`index.html` and other `.php` pages).
- CSS — custom styles (`style.css` and other CSS files).
- JavaScript — UI behavior and simple form checks (`script.js`, `customer.js`).
- Bootstrap — responsive layout and components (CDN used in admin and customer pages).
- PHP — server-side pages and forms (`*.php`).
- MySQL / MariaDB — database (connection in `connect.php`).
- Font Awesome & Unicons — icons used across the UI.

Note: There are no external social-sharing APIs found in the code. Social links use icon buttons (Font Awesome) and can be hooked to share APIs later.

## Features

- **Responsive design:** Pages adapt to phones, tablets, and desktops using CSS and Bootstrap.
- **User accounts:** Signup and login with password hashing for customers.
- **Shopping cart:** Add items, change quantities, view total price.
- **Admin area:** Add products, manage stock, view orders and payments.
- **Payment upload:** Customers upload payment proof for admin review.
- **Search:** Simple client-side search on the customer homepage.
- **Icons & UI helpers:** Uses Font Awesome and Unicons for buttons and visuals.

## How to Run This Project (for beginners)

1. Download or clone the project files to your computer.
2. Install and run a local web server with PHP and MySQL (for example, XAMPP or WAMP).
3. Place the project folder inside the server web root (for XAMPP put it in `htdocs`).
4. Start Apache and MySQL from your server control panel.
5. Create a MySQL database named `suigetsu`.
   - The project connects with user `root` and an empty password (see `connect.php`).
   - If you have an SQL export, import it. If not, create the needed tables: `customers`, `admin`, `clothes`, `cart`, `payments` (the code expects these tables).
6. Open the site in your browser by visiting `http://localhost/<project-folder>/index.html` or the equivalent local URL.
7. Use the Login form to sign in as a customer, or log in as an admin (admin accounts are stored in the `admin` table).

Tips for beginners: Run the site with XAMPP and use phpMyAdmin to create the database and tables. Keep `connect.php` settings if you use the same local environment.

## Project Structure

- `index.html` — Landing page with signup/login form.
- `style.css`, `script.js` — Main styles and small JavaScript UI logic.
- `connect.php` — Database connection settings (MySQL).
- `login.php`, `signup.php`, `logout.php` — Authentication handlers.
- `admin/` — Admin pages and styles. Contains product management and images (`clothes_images/`).
- `customer/` — Customer pages: cart, homepage, profile, payment upload, and related CSS/JS.
- `favicon/` — Icons and web manifest.

Files of interest:

- `admin/insert_clothes.php` — Add new products and upload images.
- `customer/cart.php` — View and manage the shopping cart.
- `customer/customer_payment/` — Payment upload and related files.

## Future Improvements

- Add real payment gateway integration (Stripe, PayPal).
- Implement social media share APIs for products.
- Add email confirmation and password reset flows.
- Improve input validation and stronger security hardening.
- Add a database schema SQL export for quick setup.

### suigetsu clothing web application ###

This project for my final year project in diploma level. I've evolved from an aspiring coder to the mind behind Suigetsu. 
Starting with basic coding languages, I embraced HTML, CSS, and JavaScript, laying the foundation for Suigetsu's sleek front-end.
Responsive design frameworks like Bootstrap made Suigetsu accessible across devices. 
Social integration was achieved through APIs, letting users share their finds effortlessly.
