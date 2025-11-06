# 🧾 POS System Frontend (Vite + React + Redux Toolkit)

This is the **frontend** of a comprehensive **Point of Sale (POS) Management System**, built with **React**, **Vite**, and **Redux Toolkit**.  
It provides a responsive, scalable, and modern interface for different user roles — including **Super Admin**, **Store Admin**, **Branch Manager**, and **Cashier** — to manage sales, inventory, employees, customers, and analytics.

---

## 🚀 Tech Stack

**Frontend Framework:** React + Vite  
**State Management:** Redux Toolkit  
**Routing:** React Router DOM  
**Styling:** Tailwind CSS + ShadCN UI  
**Data Fetching:** Axios  
**Charting:** Recharts  
**Icons:** Lucide React  
**Deployment:** Vercel / Render  
**Other Tools:** ESLint, Prettier

---

## 🧩 Features

### 👑 Super Admin

- Manage stores and branches
- Handle subscription plans and commissions
- Access analytics and reports
- Export and backup data
- Manage users and system settings

### 🏬 Store Admin

- Manage products, employees, and categories
- Configure store-wide settings (notifications, payment options, security)
- View detailed sales dashboards and reports
- Receive low-stock and inactive branch alerts

### 🧑‍💼 Branch Manager

- Track branch-level sales, payments, and refunds
- Manage employees and customers
- Analyze branch performance
- Access shift reports and daily summaries

### 💰 Cashier

- Process sales and returns
- Handle refunds and payments
- Manage customer loyalty points
- Print receipts and daily shift reports

### 🌐 Common Modules

- Authentication (Login, Signup, Reset Password)
- Onboarding for new stores
- Modern landing page with feature sections, testimonials, and pricing
- Responsive UI for all devices

---

## 🏗️ Folder Structure (Simplified)

```

pos-frontend-vite/
├── public/ # Static assets (SVGs, logos, previews)
├── src/
│ ├── Redux Toolkit/ # Centralized app state (slices + thunks)
│ ├── components/ # Reusable UI components (ShadCN UI)
│ ├── pages/ # Role-based page components
│ ├── context/ # React context for sidebar/theme
│ ├── routes/ # Route protection per user role
│ ├── utils/ # Utility functions (API, date, icons)
│ ├── App.jsx # Root component
│ └── main.jsx # Entry point
├── index.html
├── README.md
├── eslint.config.js
└── package.json

```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/SatinderSinghSall/Satinder-POS-MS--FRONTEND-Codebase.git
cd pos-frontend-vite
```

### 2️⃣ Install dependencies

```bash
npm install
```

### 3️⃣ Start the development server

```bash
npm run dev
```

### 4️⃣ Build for production

```bash
npm run build
```

### 5️⃣ Preview production build

```bash
npm run preview
```

---

## 🔌 Environment Variables

Create a `.env` file in the root directory and include:

```bash
VITE_API_BASE_URL=http://localhost:8080/api
VITE_CLOUDINARY_UPLOAD_URL=your_cloudinary_url
VITE_CLOUDINARY_PRESET=your_preset_name
```

---

## 📊 Key Integrations

- **Cloudinary** for image uploads
- **Redux Thunks** for async API calls
- **Recharts** for sales and analytics visualization
- **Toast Notifications** for user feedback
- **Role-based Routing & Access Control**

---

## 🧠 Developer Notes

- Modular Redux slices per feature (e.g., productSlice, orderSlice)
- Fully type-safe and scalable state architecture
- Clear folder separation by user roles
- Minimal re-renders with memoized components
- Reusable UI components built on ShadCN and Tailwind

---

## 📸 Preview (COMING SOON)

| Page         | Screenshot                                    |
| ------------ | --------------------------------------------- |
| Landing Page | ![Landing](./public/landing-page-preview.svg) |
| POS Mockup   | ![POS](./public/pos-mockup.svg)               |
| Dashboard    | ![Dashboard](./public/header-preview.svg)     |

---

## 🧑‍💻 Author

**Satinder Singh Sall**
📍 MCA Student, KiiT University, Odisha, India
💼 Passionate about Full Stack Development, Cloud Computing, and Modern Web Apps
🔗 [LinkedIn](https://www.linkedin.com/in/satinder-singh-sall-b62049204/) | [GitHub](https://github.com/SatinderSinghSall/) | [Portfolio] (https://satinder-portfolio.vercel.app/)

---

## 🪪 License

This project is licensed under the **MIT License** — feel free to modify and distribute with attribution.

---

### ⭐ If you find this project useful, please star the repo and share your feedback!
