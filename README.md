# Chirper - A Laravel Practice Project

![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)

## About

Chirper is a simple social media platform built with Laravel that demonstrates the framework's core features and best practices. The application showcases modern Laravel development techniques including:

- **Authentication and authorization**: Secure user access and resource protection.
- **Database migrations and Eloquent ORM**: Efficient database schema management and fluent querying.
- **Form validation and request handling**: Robust data integrity and user input processing.
- **Blade templating engine**: Dynamic and reusable UI components.
- **Tailwind CSS**: Modern utility-first styling.

---

## Tech Stack

This project was developed using the following environment:

* **Backend:** Laravel 11 / PHP 8.2+
* **Frontend:** Blade Templates & Tailwind CSS
* **Database:** MySQL (via XAMPP)
* **Package Managers:** Composer (PHP) & NPM (JavaScript)

---

## Prerequisites

Before you begin, ensure you have the following installed:

* **XAMPP** (with Apache and MySQL running).
* **Composer** (Global installation).
* **Node.js & NPM** (For compiling assets).
* **Git** (Optional, to clone the repo).

---

## Installation Guide

Follow these steps to get your local development environment running:

### 1. Clone the repository
```bash
git clone [https://github.com/your-username/chirper.git](https://github.com/your-username/chirper.git)
cd chirper
```

### 2. Install PHP dependencies
```bash
composer install
```

### 3. Install and compile Frontend assets
```bash
npm install
npm run build
```

### 4. Environment Configuration
Copy the example environment file and generate a unique application key:
```bash
cp .env.example .env
php artisan key:generate
```

### 5. Database Setup
1. Open **phpMyAdmin** via XAMPP and create a new database named `chirper`.
2. Edit your `.env` file and update the database credentials:
   ```env
   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=chirper
   DB_USERNAME=root
   DB_PASSWORD=
   ```

### 6. Run Migrations
Run the following command to create the necessary tables:
```bash
php artisan migrate
```

### 7. Start the Server
Finally, start the Laravel development server:
```bash
php artisan serve
```
The application will be available at: `http://127.0.0.1:8000`

---

## License

This project is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

---

## Credits

* **Developer:** [Your Name](https://github.com/your-username)
* **Inspiration:** [Laravel Boot Camp](https://bootcamp.laravel.com/) - The official hands-on introduction to Laravel.
* **Framework:** [Laravel](https://laravel.com)