# ShopVerse — Full-Stack E-Commerce Website

A responsive e-commerce website built with **HTML, CSS, Vanilla JavaScript, Node.js/Express**, with database support for **MongoDB** or **MySQL/SQL**.

## Features

- Responsive home page and product catalog
- Product search and category filtering
- Product detail page
- Shopping cart stored in browser localStorage
- User registration and login
- JWT authentication
- User account + order history
- Checkout and order creation
- Admin dashboard to add/delete products
- MongoDB support through Mongoose
- MySQL/SQL support through Sequelize
- Included SQL schema
- Demo seed data

## 1. Requirements

Install:
- Node.js 20+
- MongoDB (for Mongo mode) OR MySQL 8+ (for SQL mode)

## 2. Install

```bash
cd server
npm install
```

Copy `.env.example` to `.env` and edit it.

## 3. Run with MongoDB

`.env`:

```env
PORT=5000
DB_TYPE=mongodb
JWT_SECRET=replace_with_a_long_random_secret
MONGODB_URI=mongodb://127.0.0.1:27017/ecommerce_db
```

Then:

```bash
npm run seed
npm start
```

Open: http://localhost:5000

## 4. Run with MySQL / SQL

Create the database with `database/sql/schema.sql` or let Sequelize create the tables.

`.env`:

```env
PORT=5000
DB_TYPE=mysql
JWT_SECRET=replace_with_a_long_random_secret
MYSQL_HOST=127.0.0.1
MYSQL_PORT=3306
MYSQL_DB=ecommerce_db
MYSQL_USER=root
MYSQL_PASSWORD=your_password
```

Then:

```bash
npm run seed
npm start
```

## Demo Admin

- Email: `admin@example.com`
- Password: `Admin@12345`

Change the password before production use.

## Main Routes

Frontend:
- `/`
- `/products.html`
- `/product.html?id=...`
- `/cart.html`
- `/login.html`
- `/register.html`
- `/checkout.html`
- `/account.html`
- `/admin.html`

API:
- `GET /api/products`
- `GET /api/products/:id`
- `POST /api/auth/register`
- `POST /api/auth/login`
- `GET /api/auth/me`
- `POST /api/orders`
- `GET /api/orders`
- `POST /api/products` (admin)
- `DELETE /api/products/:id` (admin)

## Production notes

This starter does **not** include a real payment gateway, tax engine, email service, image upload service, or inventory reservation. Add Stripe/PayPal, server-side stock validation, rate limiting, CSRF strategy as appropriate, secure cookies, HTTPS, logging, and a managed database before production.

ScreenShot For Visualization:
01.
<img width="1892" height="842" alt="image" src="https://github.com/user-attachments/assets/f19541be-ddba-4307-89c7-aaf806480427" />
02.
<img width="1897" height="826" alt="image" src="https://github.com/user-attachments/assets/be23897f-fc55-4eb2-ac5b-c76686fd719e" />
03.
<img width="1896" height="543" alt="image" src="https://github.com/user-attachments/assets/0321f008-530f-4d36-9ace-db670718adfe" />
04.
<img width="1912" height="865" alt="image" src="https://github.com/user-attachments/assets/534f5cda-1417-4b9a-bd9d-5865a2e49766" />
05.
<img width="1916" height="860" alt="image" src="https://github.com/user-attachments/assets/b60e7c60-af3d-4ea1-9295-7bff9181c755" />
06.
<img width="1917" height="863" alt="image" src="https://github.com/user-attachments/assets/dea60eb5-c9c0-4d03-b017-1cd595c3b054" />
07.
<img width="1917" height="867" alt="image" src="https://github.com/user-attachments/assets/fcc83ebf-bce6-434c-befd-bcbabcc52f00" />






