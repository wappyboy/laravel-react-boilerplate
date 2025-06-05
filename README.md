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

boiler-plate/
├── app/ # Laravel backend code
├── resources/
│ └── js/ # React frontend
│ ├── Pages/ # Page components (Dashboard, Auth, etc.)
│ ├── Components/ # Shared React components
│ └── app.jsx # React entry point
├── routes/
│ ├── web.php # Inertia-powered routes
│ └── api.php # API routes (optional)
├── tests/ # Feature tests (e.g., auth)
└── ...

yaml
Copy
Edit

---

## ⚙️ Setup Instructions

### 1. Clone the Repo

```bash
git clone https://github.com/YOUR_USERNAME/laravel-react-boilerplate.git my-app
cd my-app
