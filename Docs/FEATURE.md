# ✨ PLAYBACK — Feature Specification

Este documento describe **todas las funcionalidades del producto**, organizadas por módulos y pensadas como **features reales de negocio**, no solo tareas técnicas.

---

## 🧑‍💻 Autenticación y usuarios

### Registro y login

* Registro con email y contraseña
* Login con email y contraseña
* OAuth 2.0 con Google (Google Sign‑In)
* Validación de email
* Hash seguro de contraseñas
* Manejo de sesiones con JWT + Refresh Token

### Gestión de usuarios

* Edición de perfil
* Gestión de direcciones
* Cambio de contraseña
* Desactivación de cuenta (soft delete)

---

## 👥 Roles y permisos (RBAC)

### Roles disponibles

* Administrador
* Vendedor
* Usuario (cliente)

### Control de acceso

* Rutas protegidas por rol (frontend)
* Middleware de permisos (backend)
* Acceso granular a endpoints

---

## 🛍️ Catálogo de productos

### Productos

* Creación, edición y eliminación de productos (vendedor)
* Aprobación y bloqueo de productos (admin)
* Estados del producto:

  * Activo
  * Pendiente
  * Bloqueado
* Gestión de stock
* Precio histórico
* Subida y gestión de imágenes

### Categorías

* CRUD completo (admin)
* Relación N:M con productos

### Búsqueda y filtrado

* Búsqueda por texto
* Filtros por precio
* Filtros por categoría

---

## 🛒 Carrito y compra

### Carrito

* Añadir productos
* Modificar cantidades
* Eliminar productos
* Carrito persistente por usuario

### Pedidos

* Creación de pedido desde carrito
* Estados del pedido:

  * Pendiente
  * Pagado
  * Enviado
  * Entregado
  * Cancelado
* Historial de pedidos

### Pagos (simulados)

* Métodos disponibles:

  * Tarjeta
  * Bizum
* Relación 1:1 con pedido
* Registro de estado de pago

### Envíos

* Dirección del usuario
* Empresa de transporte
* Número de tracking
* Estado del envío

---

## ⭐ Interacción del usuario

### Favoritos

* Añadir / eliminar productos
* Listado personal

### Reseñas

* Valoración 1–5 estrellas
* Comentarios
* Solo usuarios que hayan comprado

---

## 📊 Dashboards

### Admin Dashboard

* KPIs globales
* Gestión de pedidos
* Gestión de productos
* Gestión de usuarios
* Gráficas de negocio

### Vendedor Dashboard

* Ventas totales y mensuales
* Productos más vendidos
* Gestión de stock
* Pedidos propios

### Usuario Dashboard

* Pedidos recientes
* Estado de envíos
* Favoritos
* Reseñas pendientes
* Perfil

---

## 📧 Notificaciones por email

### Usuarios

* Confirmación de registro
* Confirmación y estados de pedido
* Información de envío
* Favoritos en oferta
* Respuestas de atención al cliente

### Vendedores

* Nuevo pedido
* Stock bajo
* Reseñas nuevas
* Reclamaciones

### Administrador

* Tickets abiertos
* Reclamaciones
* Reportes
* Resúmenes periódicos

---

## 🎫 Atención al cliente

* Creación de tickets
* Estados del ticket:

  * Abierto
  * En proceso
  * Resuelto
* Comunicación por email
* Historial de mensajes

---

## 🎨 UI / UX

* Diseño responsive
* Dark Mode
* Internacionalización (ES / EN)

---

## 🧪 Calidad y testing

* Validaciones backend
* Manejo centralizado de errores
* Seed de datos
* Colección Postman
