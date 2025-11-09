# 🛒 E-commerce Laravel: Home Delivery – Plataforma multi-negocio

Aplicación web de e-commerce desarrollada con **Laravel** que permite conectar a clientes con negocios aliados a través de una plataforma de pedidos y domicilios. El sistema implementa **roles de usuario** (cliente, dueño de negocio y administrador), gestión de catálogos por negocio y un panel dedicado **“Mi negocio”** para los comercios con convenio.

---

## 🚀 Características principales

- 👥 **Roles dinámicos de usuario**
  - **Cliente:** navega el catálogo y realiza pedidos.
  - **Dueño de negocio:** gestiona su negocio, catálogo y pedidos desde “Mi negocio”.
  - **Administrador:** controla usuarios, negocios y productos globales.

- 🏪 **Panel “Mi negocio”**
  - Registro y edición de información del negocio.
  - Administración de productos (crear, editar, eliminar).
  - Vista pública del catálogo del negocio.

- 📦 **Catálogo interactivo**
  - Productos organizados por negocio o categoría.
  - Filtros, vistas por tipo y secciones dinámicas.

- 🚚 **Módulo de domicilios**
  - Control básico de pedidos (pendiente, en camino, entregado).
  - Asociación con el negocio y usuario correspondiente.

- 🔐 **Navegación personalizada**
  - El **navbar cambia según el rol** del usuario autenticado.
  - Rutas protegidas mediante **middlewares de autenticación**.

---

## ⚙️ Tecnologías utilizadas

| Componente | Descripción |
|-------------|-------------|
| 🧱 **Laravel 10+** | Framework principal (MVC, migraciones, seeders) |
| 🐘 **PHP 8.1+** | Lenguaje de servidor |
| 🗄️ **MySQL / MariaDB** | Base de datos relacional |
| 🎨 **Tailwind CSS / Bootstrap** | Estilos y diseño responsivo |
| ⚡ **Alpine.js** | Interactividad ligera en el frontend |
| 🔑 **Auth Scaffolding (Breeze / Fortify)** | Registro y autenticación de usuarios |
| 🧩 **Blade Templates** | Motor de vistas de Laravel |

---

## 🖼️ Vista general

**Interfaz de catálogo para clientes:**

![Vista catálogo cliente](assets/catalogo_cliente.png)

**Panel “Mi negocio” para dueños:**

![Panel dueño](assets/catalogo_dueño.png)

**Formulario de registro con roles:**

![Registro usuario](assets/registro_roles.png)

> 📸 Las imágenes se encuentran en la carpeta `assets/` del repositorio.

---
