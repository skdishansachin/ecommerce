# Laravel E-Commerce Project

A modern e-commerce application built with **Laravel 11**, featuring a complete product catalog, user authentication, Stripe payments, and an admin panel with robust management tools and role-based access control.

## Features

### User

* **Product Catalog**: Browse products with categories, collections, and search functionality
* **Cart & Checkout**: Add products to cart, update quantities, remove items, and complete checkout
* **Stripe Payments**: Secure payments with Stripe API and webhook handling for payment status updates
* **Order Management**: View order history, order details, and status updates
* **Authentication**: User registration, login, password reset

### Admin

* **Product & Collections Management**: Full CRUD for products and collections with media uploads
* **User & Customer Management**: View and manage registered users and customers
* **Shipping Methods**: Dynamic shipping pricing configuration
* **RBAC**: Role-based access control for fine-grained permission management
* **Admin Authentication**: Secure admin login

## Tech Stack

* **PHP 8.2**, **Laravel 11**
* **Stripe API** for payments
* **Spatie Packages**:

  * MediaLibrary (file uploads)
  * Permission (RBAC)
  * Sluggable (SEO-friendly URLs)
* **Testing & Dev Tools**: PHPUnit, Laravel Telescope, Faker, Laravel Pint

## Installation

```bash
git clone https://github.com/skdishansachin/ecommerce
cd ecommerce
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
npm i
```

For local development with SQLite:

```bash
touch database/database.sqlite
php artisan migrate
```

## Development

* Start server:

```bash
php artisan serve
```

* Run tests:

```bash
php artisan test
```

* Code formatting:

```bash
./vendor/bin/pint
```
