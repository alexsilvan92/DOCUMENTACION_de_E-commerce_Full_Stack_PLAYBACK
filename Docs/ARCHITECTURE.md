# 🏗️ PLAYBACK — Architecture

Este documento define la **arquitectura técnica del sistema**, explicando cómo se conectan frontend, backend y base de datos, y por qué se toman estas decisiones.

---

## 🧠 Visión general

Arquitectura **cliente–servidor desacoplada**, basada en API REST y control de acceso por roles.

```
[ Browser ]
     ↓
[ React SPA ]
     ↓  JWT
[ Flask API ]
     ↓
[ PostgreSQL ]
```

---

## 🖥️ Frontend Architecture

### Stack

* React
* React Router
* Context API
* Tailwind CSS
* i18n

### Estructura

* Components (UI reutilizable)
* Pages (vistas por ruta)
* Contexts (auth, user, cart)
* Services (API calls)
* Guards (protección por rol)

### Seguridad

* Tokens almacenados de forma segura
* Rutas protegidas por rol
* Manejo de expiración de sesión

---

## ⚙️ Backend Architecture

### Stack

* Flask
* Flask‑JWT‑Extended
* SQLAlchemy
* Marshmallow / validaciones

### Capas

* Routes / Controllers
* Services (lógica de negocio)
* Models (ORM)
* Schemas / Validators
* Middlewares (auth, roles)

### Autenticación

* JWT Access Token
* Refresh Token
* OAuth 2.0 (Google)

---

## 🗄️ Database Architecture

### Motor

* PostgreSQL

### Principios

* Modelo relacional normalizado
* Relaciones 1:N y N:M
* Soft delete en entidades críticas

### Entidades principales

* User
* Role
* Product
* Category
* Order
* OrderItem
* Payment
* Shipment
* Review
* Favorite
* Ticket

---

## 🔐 Seguridad

* Hash de contraseñas
* Control de acceso por rol (RBAC)
* Validación de inputs
* Protección de endpoints críticos

---

## 📧 Sistema de notificaciones

* Envío de emails asincrónico
* Plantillas HTML
* Eventos de dominio (order_created, stock_low, etc.)

---

## 🚀 Deploy Architecture

### Frontend

* Vercel

### Backend

* API desplegada en servicio cloud

### Database

* PostgreSQL gestionado

### Variables de entorno

* Secrets
* Tokens
* Credenciales externas

---

## 📈 Escalabilidad

* Separación de responsabilidades
* Backend desacoplado
* Fácil extensión a microservicios

---

## 🧪 Observabilidad y calidad

* Logging centralizado
* Manejo de errores global
* Tests de endpoints
* Postman collection
