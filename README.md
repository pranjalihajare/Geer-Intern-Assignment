# Geer Intern Assignment

A full-stack e-commerce prototype inspired by [Geer.in](https://geer.in), built as an internship assignment.

## 🛠 Tech Stack

### Frontend:

* Next.js (App Router, TypeScript)
* Tailwind CSS

### Backend:

* Next.js API Routes (serverless functions)
* In-memory data storage (temporary during dev runtime)

## 🚀 How to Run the Project

 Setup frontend (with API included)

```bash
cd frontend
npm install
npm run dev
```

The app will run at `http://localhost:3000`

## 📁 Project Structure

```
geer-intern-assignment/
├── frontend/
│   ├── app/ (Next.js App Router pages)
│   ├── pages/api/products/ (GET, POST, DELETE APIs)
│   ├── lib/products.ts (shared in-memory data)
│   └── ...
└── README.md
```

## 🧪 Features

* View all products at `/products`
* Delete products via UI (hover to reveal × button)
* Search products by name

## ⚠️ Notes / Assumptions

* Products are stored in-memory, so they reset on every dev server restart.
* This is a development-only mock server (no persistent database).
* The frontend assumes the backend API is on the same origin (Next.js API routes).

## 🎯 Future Improvements (not implemented)

* Add persistent storage (e.g., SQLite, PostgreSQL, or lowdb)
* Add `/products/[id]` detail page
* Admin auth for managing products
