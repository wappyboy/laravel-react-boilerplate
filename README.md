# 🚀 Laravel + React Monolith Boilerplate

A reusable full-stack starter kit that combines **Laravel**, **React (via Vite + Inertia)**, and **Sanctum authentication** into a unified monolith structure. Ideal for rapid development of modern web apps without managing separate backend and frontend repos.

---

## 🧱 Tech Stack

- **Laravel** – Backend framework
- **React** – Frontend SPA (via Vite + Inertia.js)
- **Laravel Sanctum** – Session-based authentication
- **Vite** – Lightning-fast asset bundler
- **PHPUnit** – Feature testing

---

## 📁 Project Structure

```
boiler-plate/
├── app/                      # Laravel backend logic (controllers, models, etc.)
├── bootstrap/                # Application bootstrap files
├── config/                   # Laravel configuration files
├── database/                 # Migrations, seeders, factories
├── public/                   # Public assets (index.php, built JS/CSS)
├── resources/
│   ├── js/                   # Frontend (React + Inertia)
│   │   ├── Pages/            # React pages (Inertia-rendered)
│   │   ├── Components/       # Reusable React components
│   │   └── app.jsx           # Root entry point for React
│   └── views/                # Blade fallback views (optional)
├── routes/
│   ├── web.php               # Web routes using Inertia
│   └── api.php               # Optional API routes (if needed)
├── tests/                    # Feature and unit tests (PHPUnit)
├── vite.config.js            # Vite configuration (React + Laravel)
├── package.json              # NPM packages and frontend build scripts
├── artisan                   # Laravel CLI
├── .env                      # Environment variables
├── .gitignore                # Git ignored files
└── composer.json             # PHP dependencies and autoloading
```

---

## ⚙️ Setup Instructions

### 1. Clone the Repo

```bash
git clone https://github.com/YOUR_USERNAME/laravel-react-boilerplate.git my-app
cd my-app
```

### 2. Install PHP Dependencies

```bash
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
```

### 3. Install Node Modules and Start Vite

```bash
npm install
npm run dev
```

### 4. Run Laravel Server

```bash
php artisan serve
```

Open your browser and go to: [http://localhost:8000](http://localhost:8000)

---

## 🔐 Authentication

This boilerplate includes:

- Login & Registration
- Auth-protected Dashboard
- Sanctum-powered session authentication

Example of protected route using Inertia:

```php
use Inertia\Inertia;

Route::middleware(['auth'])->group(function () {
    Route::get('/dashboard', fn () => Inertia::render('Dashboard'));
});
```

---

## 📦 Build for Production

```bash
npm run build
```

This will compile all assets for production.

---

## 🧪 Running Tests

```bash
php artisan test
```

All feature tests are located in `tests/Feature`.

---

## 🚀 Deployment

Make sure to:

- Run `npm run build`
- Set up environment variables in `.env`
- Configure your server (Laravel Forge, Heroku, or shared hosting)

---

## 📝 License

This project is open-source under the [MIT License](LICENSE).

---

## 🙌 Author

Created by **Ralph Eco**  
[[GitHub](https://github.com/wappyboy)
