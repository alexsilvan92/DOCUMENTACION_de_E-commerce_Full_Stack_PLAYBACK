# 🛒 PLAYBACK

> **MVP de E-commerce Full Stack**
> Proyecto final orientado a demostrar dominio técnico y visión de producto real.

---

## 🎯 Objetivo del proyecto

Construir una aplicación web de **e-commerce moderna, escalable y realista**, diseñada para demostrar competencias **full stack completas**:

- Frontend moderno
- Backend robusto
- Base de datos relacional
- Autenticación avanzada
- Control de roles
- Pagos simulados
- Comunicación por email
- Despliegue en producción

> ⚠️ El objetivo **no es un CRUD**, sino un **producto defendible como negocio real**.

📄 Documentación
- [Features](docs/FEATURE.md)
- [Architecture](docs/ARCHITECTURE.md)
- [Roadmap](docs/ROADMAP.md)

---

## 🏗️ Arquitectura técnica

### 🖥️ Frontend

| Tecnología   | Uso                      |
| ------------ | ------------------------ |
| React        | SPA principal            |
| React Router | Rutas protegidas por rol |
| Context API  | Estado global            |
| Tailwind CSS | UI moderna y responsive  |
| i18n         | Internacionalización     |
| Dark Mode    | Mejora UX                |

---

### ⚙️ Backend

| Tecnología    | Uso                   |
| ------------- | --------------------- |
| Flask         | Framework backend     |
| API REST      | Arquitectura          |
| JWT           | Autenticación         |
| Refresh Token | Sesiones persistentes |
| RBAC          | Control de acceso     |
| SQLAlchemy    | ORM                   |

> Incluye validaciones, middlewares de permisos y manejo centralizado de errores.

---

### 🗄️ Base de datos

| Elemento          | Descripción             |
| ----------------- | ----------------------- |
| PostgreSQL        | Base de datos principal |
| Modelo relacional | Normalizado             |
| Relaciones        | 1:N y N:M               |
| Soft delete       | Entidades críticas      |

---

### 🚀 Deploy

| Servicio | Plataforma |
| -------- | ---------- |
| Frontend | Vercel     |
| Backend  | ?????      |
| Database | ?????      |

---

## 👥 Roles y permisos (RBAC)

| Rol              | Descripción                  |
| ---------------- | ---------------------------- |
| 👑 Administrador | Control global del sistema   |
| 🧑‍💼 Vendedor      | Gestión de catálogo y ventas |
| 🧑 Usuario       | Compra de productos          |

---

### 👑 Administrador

**Responsabilidades principales**:

- Gestión de usuarios y vendedores
- Moderación de productos
- Supervisión de pedidos
- Cambio de estados
- Acceso a métricas globales

---

### 🧑‍💼 Vendedor

**Gestión de negocio propio**:

- CRUD de productos
- Gestión de stock
- Subida de imágenes
- Visualización de pedidos propios
- Estadísticas de ventas

---

### 🧑 Usuario (cliente)

**Experiencia de compra**:

- Registro y login
- Navegación por catálogo
- Carrito y pedidos
- Historial de compras
- Favoritos y reseñas

---

## 🔐 Autenticación y seguridad

- Email + contraseña
- **OAuth 2.0 (Google Sign-In)**
- JWT + Refresh Tokens
- Hash seguro de contraseñas
- Middleware por rol

---

## 🧱 Funcionalidades por módulos

### 🛍️ Catálogo

| Módulo     | Funcionalidades                 |
| ---------- | ------------------------------- |
| Productos  | Precio, stock, imágenes, estado |
| Categorías | CRUD + relación N:M             |
| Búsqueda   | Texto + filtros                 |

---

### 🛒 Compra

| Módulo  | Funcionalidades            |
| ------- | -------------------------- |
| Carrito | Persistente por usuario    |
| Pedidos | Estados y precio histórico |
| Pagos   | Tarjeta / Bizum (simulado) |
| Envíos  | Dirección, tracking        |

---

### ⭐ Interacción

| Módulo    | Funcionalidades       |
| --------- | --------------------- |
| Favoritos | Guardado de productos |
| Reseñas   | Solo compradores      |
| UI/UX     | Dark mode, responsive |
| Idiomas   | ES / EN               |

---

## 📊 Dashboards

> Cada rol dispone de un **panel personalizado**, orientado a negocio.

---

### 👑 Admin Dashboard

**KPIs globales**:

| Métrica            |
| ------------------ |
| Usuarios por rol   |
| Ventas totales     |
| Ventas por periodo |
| Total pedidos      |

**Gestión**:

- Pedidos (tabla + estados)
- Productos (aprobación / bloqueo)
- Usuarios (roles y bloqueos)

**Gráficas**:

- Ventas mensuales
- Pedidos por estado
- Nuevos usuarios

---

### 🧑‍💼 Vendedor Dashboard

**Ventas**:

| Métrica          |
| ---------------- |
| Ventas totales   |
| Ventas mensuales |
| Comparativa      |

**Gestión**:

- Productos activos
- Stock bajo
- Pedidos propios

**Gráficas**:

- Ventas por producto
- Evolución mensual

---

### 🧑 Usuario Dashboard

- Pedidos recientes
- Estado de envíos
- Favoritos
- Reseñas pendientes
- Perfil y direcciones

---

## 📧 Notificaciones y comunicación

> Sistema de notificaciones por **email basado en eventos**.

### 🧑 Usuario

- Confirmaciones
- Estados de envío
- Favoritos en oferta
- Atención al cliente

---

### 🧑‍💼 Vendedor

- Nuevos pedidos
- Stock bajo
- Reseñas
- Reclamaciones

---

### 👑 Administrador

- Tickets abiertos
- Reclamaciones
- Reportes
- Resúmenes del sistema

---

### 🎫 Sistema de tickets

| Estado     | Descripción   |
| ---------- | ------------- |
| Abierto    | Ticket creado |
| En proceso | En atención   |
| Resuelto   | Cerrado       |

Incluye historial y comunicación por email.

---

## 🧪 Testing y calidad

- Validaciones backend
- Manejo centralizado de errores
- Seed de datos
- Colección Postman

---

## 🏁 Valor del proyecto

✔ Arquitectura profesional  
✔ Flujo real de negocio  
✔ Escalable y defendible  
✔ Enfoque full stack completo
