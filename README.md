# FinEase

FinEase is a personal finance management web application designed to help users
manage their income, expenses, budgets, and savings goals in one place. Users
can record and manage transactions, set monthly budgets, and monitor their
financial activities through clear summaries, charts, and reports.

The project focuses on building a secure, responsive, and user-friendly
financial management experience while handling authentication, protected API
access, database operations, error handling, and reliable deployment.

## 🚀 Technologies Used

### Programming Language

- JavaScript

### Frontend

- React
- Vite
- Tailwind CSS
- DaisyUI
- React Router
- Axios
- Firebase Authentication
- Recharts
- Lucide React
- React Icons
- SweetAlert2
- React Toastify

### Backend

- Node.js
- Express.js
- MongoDB
- MongoDB Atlas
- Firebase Admin SDK
- CORS
- dotenv

### Deployment & Development

- Vercel
- Git & GitHub
- Firebase
- npm
- Surge
- Netlify

## ✨ Features

- 🔐 Firebase authentication with email/password and Google sign-in
- 👤 User profile management
- 💰 Create, read, update, and delete financial transactions
- 🗑️ Delete multiple transactions at once
- 🔎 Filter transactions by category, type, amount, and date
- ↕️ Sort transactions by different criteria
- 📊 Financial summaries and interactive charts
- 💵 Income and expense tracking
- 🎯 Savings and budgeting management
- 📅 Proper transaction date handling
- 📱 Responsive design for different screen sizes
- 🔒 Protected routes and authenticated API requests
- 🛡️ Server-side Firebase token verification
- 🗄️ Secure user-specific MongoDB queries
- ⚠️ Proper HTTP error handling
- 🔄 Automatic retry with exponential backoff and jitter for temporary
  server/network failures
- 🌐 Configurable CORS for development and production environments

## 🧩 Problems Solved

While developing FinEase, several real-world application problems were
addressed:

### Authentication & API Security

Implemented Firebase Authentication on the client side and Firebase Admin token
verification on the server side to protect private API routes. Database queries
also verify the authenticated user's email so users can only access their own
financial data.

### Transaction Management

Built complete CRUD functionality for transactions, including individual and
bulk deletion, transaction updating, filtering, sorting, and selection
management.

### Reliable Error Handling

Implemented handling for common API and server errors such as `400`, `401`,
`403`, `404`, `413`, and `500` responses, along with appropriate frontend error
states.

### Network & Server Recovery

Implemented retry logic using exponential backoff and jitter for temporary
server or network failures. This helps prevent repeated requests from being sent
at the same time when a server becomes temporarily unavailable.

### Date Handling

Implemented reliable transaction date parsing and validation to prevent invalid
calendar dates and avoid timezone-related date inconsistencies.

### Database Security

MongoDB queries are scoped to the authenticated user's identity, preventing
users from accessing or modifying transactions belonging to other users.

### Responsive User Interface

Designed transaction tables, forms, charts, navigation, modals, and other
components to work across desktop, tablet, and mobile screen sizes.

### Production Deployment

Configured the Express backend for Vercel deployment and resolved a production
dependency compatibility issue involving Firebase Admin, `jwks-rsa`, and `jose`.

### CORS Configuration

Implemented environment-based CORS configuration so production deployments can
allow only trusted frontend origins while local development can use the local
development origin.

## 📁 Project Structure

```text
FinEase
├── client
│   ├── src
│   │   ├── components
│   │   ├── pages
│   │   ├── contexts
│   │   ├── hooks
│   │   ├── routes
│   │   └── ...
│   └── ...
│
└── server
    ├── index.js
    ├── package.json
    ├── .env
    └── ...

🎯 Project Goal
The goal of FinEase is to provide a simple and practical platform for managing personal finances while demonstrating modern full-stack web development practices, including authentication, secure API design, database management, responsive UI development, error recovery, and production deployment.
```

🌐 Live Application: [(https://finease-finance-management.web.app/)]

👨‍💻 Author: Developed as a full-stack personal finance management project using
modern web technologies.
