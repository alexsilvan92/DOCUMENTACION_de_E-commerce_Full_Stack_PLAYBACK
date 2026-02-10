# 🛒 PLAYBACK

> **Full Stack E-commerce MVP**  
> Final project aimed at demonstrating strong technical skills and real product vision.

---

## 🎯 Project Goal

Build a **modern, scalable, and realistic e-commerce web application**, designed to demonstrate **complete full stack competencies**:

- Modern frontend
- Robust backend
- Relational database
- Advanced authentication
- Role-based access control
- Simulated payments
- Email communication
- Production deployment

> ⚠️ The goal is **not a CRUD**, but a **product defensible as a real business**.

📄 Documentation
- [Features](docs/FEATURE.md)
- [Architecture](docs/ARCHITECTURE.md)
- [Roadmap](docs/ROADMAP.md)

---

## 🏗️ Technical Architecture

### 🖥️ Frontend

| Technology     | Usage                        |
| -------------- | ---------------------------- |
| React          | Main SPA                     |
| React Router   | Role-protected routes        |
| Context API    | Global state management      |
| Tailwind CSS   | Modern and responsive UI     |
| i18n           | Internationalization         |
| Dark Mode      | UX improvement               |

---

### ⚙️ Backend

| Technology      | Usage                       |
| --------------- | --------------------------- |
| Flask           | Backend framework           |
| REST API        | Architecture                |
| JWT             | Authentication              |
| Refresh Token   | Persistent sessions         |
| RBAC            | Access control              |
| SQLAlchemy      | ORM                         |

> Includes validations, permission middlewares, and centralized error handling.

---

### 🗄️ Database

| Element           | Description                 |
| ----------------- | --------------------------- |
| PostgreSQL        | Main database               |
| Relational model  | Normalized                  |
| Relationships    | 1:N and N:M                 |
| Soft delete       | Critical entities           |

---

### 🚀 Deployment

| Service   | Platform |
| --------- | -------- |
| Frontend  | Vercel   |
| Backend   | ?????    |
| Database  | ?????    |

---

## 👥 Roles and Permissions (RBAC)

| Role               | Description                   |
| ------------------ | ----------------------------- |
| 👑 Administrator   | Global system control         |
| 🧑‍💼 Seller        | Catalog and sales management |
| 🧑 User            | Product purchasing           |

---

### 👑 Administrator

**Main responsibilities**:

- User and seller management
- Product moderation
- Order supervision
- Status changes
- Access to global metrics

---

### 🧑‍💼 Seller

**Own business management**:

- Product CRUD
- Stock management
- Image uploads
- View own orders
- Sales statistics

---

### 🧑 User (Customer)

**Shopping experience**:

- Registration and login
- Catalog browsing
- Cart and orders
- Purchase history
- Favorites and reviews

---

## 🔐 Authentication and Security

- Email + password
- **OAuth 2.0 (Google Sign-In)**
- JWT + Refresh Tokens
- Secure password hashing
- Role-based middleware

---

## 🧱 Features by Module

### 🛍️ Catalog

| Module      | Features                        |
| ----------- | ------------------------------- |
| Products    | Price, stock, images, status    |
| Categories  | CRUD + N:M relationship         |
| Search      | Text + filters                  |

---

### 🛒 Purchase

| Module   | Features                     |
| -------- | ---------------------------- |
| Cart     | Persistent per user          |
| Orders   | States and price history     |
| Payments | Card / Bizum (simulated)     |
| Shipping | Address, tracking            |

---

### ⭐ Interaction

| Module     | Features                   |
| ---------- | -------------------------- |
| Favorites  | Product saving             |
| Reviews    | Buyers only                |
| UI/UX     | Dark mode, responsive      |
| Languages  | ES / EN                    |

---

## 📊 Dashboards

> Each role has a **custom business-oriented dashboard**.

---

### 👑 Admin Dashboard

**Global KPIs**:

| Metric              |
| ------------------- |
| Users by role       |
| Total sales         |
| Sales by period     |
| Total orders        |

**Management**:

- Orders (table + statuses)
- Products (approval / blocking)
- Users (roles and bans)

**Charts**:

- Monthly sales
- Orders by status
- New users

---

### 🧑‍💼 Seller Dashboard

**Sales**:

| Metric            |
| ----------------- |
| Total sales       |
| Monthly sales     |
| Comparison        |

**Management**:

- Active products
- Low stock
- Own orders

**Charts**:

- Sales by product
- Monthly evolution

---

### 🧑 User Dashboard

- Recent orders
- Shipping status
- Favorites
- Pending reviews
- Profile and addresses

---

## 📧 Notifications and Communication

> Event-based **email notification system**.

### 🧑 User

- Confirmations
- Shipping status updates
- Favorites on sale
- Customer support

---

### 🧑‍💼 Seller

- New orders
- Low stock alerts
- Reviews
- Claims

---

### 👑 Administrator

- Open tickets
- Claims
- Reports
- System summaries

---

### 🎫 Ticket System

| Status       | Description     |
| ------------ | --------------- |
| Open         | Ticket created  |
| In progress  | Being handled   |
| Resolved     | Closed          |

Includes history and email communication.

---

## 🧪 Testing and Quality

- Backend validations
- Centralized error handling
- Data seeding
- Postman collection

---

## 🏁 Project Value

✔ Professional architecture  
✔ Real business flow  
✔ Scalable and defensible  
✔ Complete full stack focus  
