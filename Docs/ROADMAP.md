# 🛒 PLAYBACK – Project Roadmap

> **Full Stack E-commerce MVP**
> Roadmap técnico y de producto para ejecución en 5 semanas con metodología Scrumban.

---

## 🧭 Visión general

**Objetivo final:** entregar un e-commerce funcional, escalable y defendible como producto real, con roles, flujos completos de compra y dashboards orientados a negocio.

* Duración total: **5 semanas**
* Equipo: **3 desarrolladores**
* Metodología: **Scrum + Kanban (Scrumban)**
* Sprint length: **1 semana**

---

## 🗓️ Roadmap por Sprints

### 🚀 Sprint 0 – Setup & Foundations (Semana 1)

**Goal:** Proyecto desplegado y listo para desarrollo continuo

**Entregables clave:**

* Repositorios configurados
* Deploy inicial
* Arquitectura base definida

**Features:**

* Setup backend Flask + SQLAlchemy
* Setup frontend React + Tailwind
* PostgreSQL configurado
* Variables de entorno
* CI básico
* README inicial

---

### 🔐 Sprint 1 – Authentication & RBAC (Semana 2)

**Goal:** Usuarios autenticados y control de acceso por rol

**Features:**

* Registro y login (email/password)
* JWT + Refresh Token
* OAuth 2.0 (Google Sign-In)
* RBAC (admin, vendor, user)
* Rutas protegidas frontend

---

### 🛍️ Sprint 2 – Catalog & Products (Semana 3)

**Goal:** Marketplace navegable con productos reales

**Features:**

* CRUD productos (vendor)
* Categorías N:M
* Búsqueda y filtros
* Favoritos
* Subida de imágenes

---

### 🛒 Sprint 3 – Orders & Checkout (Semana 4)

**Goal:** Flujo de compra completo y funcional

**Features:**

* Carrito persistente
* Creación de pedidos
* Estados de pedido
* Pagos simulados
* Envíos y tracking
* Emails transaccionales

---

### 📊 Sprint 4 – Dashboards & Polish (Semana 5)

**Goal:** Producto listo para demo y defensa

**Features:**

* Admin dashboard (KPIs globales)
* Vendor dashboard (ventas y stock)
* User dashboard (pedidos y perfil)
* Sistema de tickets
* UX/UI polish
* Bugfixing

---

## 🧩 GitHub Issues por Sprint

# 🛒 PLAYBACK – GitHub Issues (Global Numbering)

---

## 🚀 Sprint 0 – Setup & Foundations

### 1. 🏗️ Backend project scaffolding
- **Labels:** feature, backend, tech-debt
- **Area:** Backend
- **Type:** Feature
- **Historia de usuario:**
  - Como desarrollador backend,
  - quiero tener el proyecto Flask + SQLAlchemy configurado,
  - para poder empezar a desarrollar la API de forma organizada.
- **Criterios de aceptación:**
  - [ ] 1.1  Estructura de carpetas (app/, models/, routes/)
  - [ ] 1.2 app.py inicial funcionando
  - [ ] 1.3 requirements.txt definido
  - [ ] 1.4 Entorno virtual creado y activado

---

### 2. 🎨 Frontend project scaffolding
- **Labels:** feature, frontend, tech-debt
- **Area:** Frontend
- **Type:** Feature
- **Historia de usuario:**
  - Como desarrollador frontend,
  - quiero tener el proyecto React + Tailwind configurado,
  - para poder construir la interfaz de forma escalable.
- **Criterios de aceptación:**
  - [ ] 2.1  Proyecto React creado
  - [ ] 2.2 Tailwind configurado
  - [ ] 2.3 Estructura base de componentes
  - [ ] 2.4 App renderizando correctamente

---

### 3. 🗄️ Database schema v1
- **Labels:** feature, database
- **Area:** DB
- **Type:** Feature
- **Historia de usuario:**
  - Como desarrollador,
  - quiero definir el esquema inicial de la base de datos,
  - para soportar usuarios, roles y productos.
- **Criterios de aceptación:**
  - [ ] 3.1 Modelo User
  - [ ] 3.2 Modelo Role
  - [ ] 3.3 Relaciones definidas
  - [ ] 3.4 Migraciones listas

---

### 4. ⚙️ Environment configuration
- **Labels:** tech-debt, devops
- **Area:** DevOps
- **Type:** Tech Debt
- **Historia de usuario:**
  - Como desarrollador,
  - quiero configurar variables de entorno,
  - para separar configuración de código.
- **Criterios de aceptación:**
  - [ ] 4.1 .env.example creado
  - [ ] 4.2 Variables cargadas correctamente
  - [ ] 4.3 Secrets fuera del repo

---

### 5. 🚀 Initial deploy
- **Labels:** feature, devops
- **Area:** DevOps
- **Type:** Feature
- **Historia de usuario:**
  - Como desarrollador,
  - quiero desplegar el proyecto base,
  - para validar el flujo de deploy continuo.
- **Criterios de aceptación:**
  - [ ] 5.1 Backend desplegado
  - [ ] 5.2 Frontend desplegado
  - [ ] 5.3 App accesible públicamente

---

## 🔐 Sprint 1 – Authentication & RBAC

### 6. 📝 User registration endpoint
- **Labels:** feature, backend, auth
- **Area:** Backend
- **Type:** Feature
- **Historia de usuario:**
  - Como visitante,
  - quiero registrarme con email y password,
  - para acceder a la plataforma.
- **Criterios de aceptación:**
  - [ ] 6.1 Endpoint POST /register
  - [ ] 6.2 Password hasheado
  - [ ] 6.3 Email único validado

---

### 7. 🔑 Login + JWT authentication
- **Labels:** feature, backend, auth
- **Area:** Backend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 7.1 Endpoint /login
  - [ ] 7.2 JWT generado
  - [ ] 7.3 Token válido en requests

---

### 8. ♻️ Refresh token flow
- **Labels:** feature, backend, auth
- **Area:** Backend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 8.1 Refresh token persistido
  - [ ] 8.2 Renovación automática
  - [ ] 8.3 Revocación segura

---

### 9. 🔐 Google OAuth integration
- **Labels:** feature, backend, auth
- **Area:** Backend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 9.1 OAuth configurado
  - [ ] 9.2 Login con Google
  - [ ] 9.3 Usuario creado si no existe

---

### 10. 🛂 Role-based access control (RBAC)
- **Labels:** feature, backend, auth
- **Area:** Backend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 10.1 Roles definidos
  - [ ] 10.2 Middleware por rol
  - [ ] 10.3 Accesos protegidos

---

### 11. 🧭 Protected routes (frontend)
- **Labels:** feature, frontend, auth
- **Area:** Frontend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 11.1 Guards por rol
  - [ ] 11.2 Redirecciones correctas
  - [ ] 11.3 Persistencia de sesión

---

## 🛍️ Sprint 2 – Catalog & Products

### 12. 📦 Product model and endpoints
- **Labels:** feature, backend
- **Area:** Backend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 12.1 Modelo Product
  - [ ] 12.2 CRUD endpoints
  - [ ] 12.3 Validaciones

---

### 13. 🏷️ Category model (N:M)
- **Labels:** feature, backend, database
- **Area:** DB
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 13.1 Modelo Category
  - [ ] 13.2 Relación N:M
  - [ ] 13.3 CRUD categorías

---

### 14. 🛠️ Product CRUD (vendor)
- **Labels:** feature, backend
- **Area:** Backend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 14.1 Permisos vendor
  - [ ] 14.2 Gestión de stock
  - [ ] 14.3 Persistencia correcta

---

### 15. 🖼️ Product listing UI
- **Labels:** feature, frontend
- **Area:** Frontend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 15.1 Grid/listado
  - [ ] 15.2 Datos correctos
  - [ ] 15.3 Responsive

---

### 16. 🔍 Search and filters
- **Labels:** feature, frontend
- **Area:** Frontend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 16.1 Búsqueda texto
  - [ ] 16.2 Filtros categoría/precio
  - [ ] 16.3 UX clara

---

### 17. ❤️ Favorites system
- **Labels:** feature, frontend, backend
- **Area:** Backend / Frontend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 17.1 Endpoint favoritos
  - [ ] 17.2 UI favoritos
  - [ ] 17.3 Persistencia DB

---

## 🛒 Sprint 3 – Orders & Checkout

### 18. 🛍️ Cart persistence
- **Labels:** feature, backend, frontend
- **Area:** Backend / Frontend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 18.1 Carrito por usuario
  - [ ] 18.2 Persistencia sesión
  - [ ] 18.3 Sync frontend

---

### 19. 📝 Order creation
- **Labels:** feature, backend
- **Area:** Backend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 19.1 Crear pedido
  - [ ] 19.2 Validar stock
  - [ ] 19.3 Guardar histórico

---

### 20. 🔄 Order state machine
- **Labels:** feature, backend
- **Area:** Backend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 20.1 Estados definidos
  - [ ] 20.2 Transiciones válidas
  - [ ] 20.3 Notificaciones

---

### 21. 💳 Simulated payment gateway
- **Labels:** feature, backend, payment
- **Area:** Backend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 21.1 Pago simulado OK
  - [ ] 21.2 Pago fallido
  - [ ] 21.3 Pedido actualizado

---

### 22. 🚚 Shipping and tracking
- **Labels:** feature, backend, frontend
- **Area:** Backend / Frontend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 22.1 Dirección envío
  - [ ] 22.2 Tracking visible
  - [ ] 22.3 Estado sincronizado

---

### 23. 📧 Transactional emails
- **Labels:** feature, backend, notifications
- **Area:** Backend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 23.1 Email confirmación
  - [ ] 23.2 Email cambio estado
  - [ ] 23.3 Templates HTML

---

## 📊 Sprint 4 – Dashboards & Polish

### 24. 📈 Admin dashboard KPIs
- **Labels:** feature, frontend, backend, dashboard
- **Area:** Backend / Frontend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 24.1 KPIs globales
  - [ ] 24.2 Gráficas
  - [ ] 24.3 Datos en tiempo real

---

### 25. 📊 Vendor dashboard analytics
- **Labels:** feature, frontend, backend, dashboard
- **Area:** Backend / Frontend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 25.1 Ventas por producto
  - [ ] 25.2 Stock bajo
  - [ ] 25.3 Visualización clara

---

### 26. 🧑‍💻 User dashboard
- **Labels:** feature, frontend, dashboard
- **Area:** Frontend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 26.1 Pedidos recientes
  - [ ] 26.2 Perfil editable
  - [ ] 26.3 Favoritos visibles

---

### 27. 🎫 Ticket system
- **Labels:** feature, frontend, backend, notifications
- **Area:** Backend / Frontend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 27.1 Crear ticket
  - [ ] 27.2 Estados ticket
  - [ ] 27.3 Emails asociados

---

### 28. ✨ UX improvements
- **Labels:** feature, frontend
- **Area:** Frontend
- **Type:** Feature
- **Criterios de aceptación:**
  - [ ] 28.1 UI consistente
  - [ ] 28.2 Feedback visual
  - [ ] 28.3 Dark mode pulido

---

### 29. 🐞 Final testing and fixes
- **Labels:** bug, frontend, backend
- **Area:** Backend / Frontend
- **Type:** Bug
- **Criterios de aceptación:**
  - [ ] 29.1 Bugs críticos resueltos
  - [ ] 29.2 Flujos completos OK
  - [ ] 29.3 Demo estable

---

## 📊 GitHub Projects – Kanban Board

1. **Backlog**
   Ideas, mejoras futuras, tareas no priorizadas

2. **Sprint To Do**
   Issues comprometidas en el sprint actual

3. **In Progress** (WIP limit: 3)
   Trabajo activo

4. **In Review** (WIP limit: 2)
   Pull Requests abiertos

5. **Done**
   Completado y deployado

---
