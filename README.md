# MARKETA — Supermarket Management System

A complete **MERN Stack** supermarket management system with **ES Modules (type: module)** and **MVC architecture**.

---

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- MongoDB (local or Atlas)

### 1. Setup Backend
```bash
cd backend
npm install
# Edit .env and set your MONGO_URI
npm run dev
```
Server runs at: `http://localhost:5000`

### 2. Setup Frontend
```bash
cd frontend
npm install
npm run dev
```
App runs at: `http://localhost:5173`

---

## 🔐 First Login

1. Go to `http://localhost:5173`
2. Click **Register** tab
3. Register the **first account** — it auto-becomes **Admin** (approved instantly)
4. Any subsequent registrations require Admin approval from the **Admin Panel**

---

## 📁 Project Structure

```
marketa/
├── backend/              # Express + Mongoose (ES Modules)
│   ├── config/           # MongoDB connection
│   ├── controllers/      # Business logic (MVC)
│   ├── middlewares/      # Auth, error, upload
│   ├── models/           # Mongoose schemas
│   ├── routes/           # Express routers
│   ├── utils/            # Helpers
│   ├── uploads/          # Product images (auto-created)
│   ├── .env              # Environment config
│   └── server.js         # Entry point
│
└── frontend/             # React 18 + Vite
    └── src/
        ├── api/          # Axios instance
        ├── context/      # Auth context
        ├── components/   # Layout + UI components
        └── pages/        # All page components
```

---

## 🧩 Modules

| Module | Route |
|--------|-------|
| Dashboard | `/` |
| Products | `/products` |
| Categories | `/categories` |
| Suppliers | `/suppliers` |
| Customers | `/customers` |
| Purchases | `/purchases` |
| Sales (POS) | `/sales` |
| Inventory | `/inventory` |
| Reports | `/reports` |
| Notifications | `/notifications` |
| Settings | `/settings` |
| Admin Panel | `/admin` (admin only) |

---

## ⚙️ Environment Variables

`backend/.env`:
```
PORT=5000
MONGO_URI=mongodb://localhost:27017/marketa
JWT_SECRET=your_secret_key
JWT_EXPIRE=7d
NODE_ENV=development
```
