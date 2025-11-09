<p align="center"><a href="https://laravel.com" target="_blank">

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="./Home1.png" alt="Build Status"></a>



## Home Delivery

Nuestra plataforma de mensajería combina la eficiencia tradicional con la innovación tecnológica al ofrecer un servicio de entregas rápidas y seguras que ahora incorpora el uso de drones. A través de una red logística inteligente, garantizamos la entrega de paquetes en tiempo récord, incluso en zonas de difícil acceso, optimizando cada trayecto con tecnología de geolocalización avanzada. Ya sea por tierra o aire, nuestro compromiso es brindar soluciones de envío modernas, sostenibles y confiables para particulares y empresas.

# 🛒 E-commerce Laravel – Plataforma multi-negocio

Aplicación web de e-commerce desarrollada con **Laravel** que permite conectar a clientes con negocios aliados a través de una plataforma de pedidos y domicilios. El sistema implementa **roles de usuario** (cliente, dueño de negocio y administrador), gestión de catálogos por negocio y un panel dedicado **“Mi negocio”** para los comercios con convenio.

---

## 🚀 Características principales

- 👥 **Múltiples roles de usuario**
  - **Cliente**: navega el catálogo, realiza pedidos y consulta su historial.
  - **Dueño de negocio con convenio**: administra su propio catálogo, ve estadísticas y gestiona domicilios desde la sección **“Mi negocio”**.
  - **Administrador**: gestiona usuarios, negocios, productos globales y parámetros del sistema.

- 🏪 **Módulo “Mi negocio” para dueños**
  - Registro de negocio (nombre, categoría, datos básicos).
  - Gestión de productos propios (crear, editar, eliminar).
  - Visualización de catálogo público del negocio.
  - Vista interna tipo tablero para revisar pedidos y domicilios.

- 🧾 **Catálogo y productos**
  - Catálogo filtrable y navegable para clientes.
  - Asociación de productos a un negocio (multi-negocio).
  - Posibilidad de vista de catálogo específica por negocio.

- 🚚 **Módulo de domicilios** (estructura base)
  - Registro y seguimiento básico de pedidos.
  - Integración lógica para estados de pedido (pendiente, en camino, entregado, etc.).

- 🔐 **Gestión de roles y navegación dinámica**
  - El **navbar cambia según el rol** del usuario autenticado.
  - Acceso a **“Mi negocio”** sólo para dueños de negocio con convenio.
  - Rutas protegidas mediante middlewares de autenticación y permisos.

- 🎨 **Front-end personalizable**
  - Vistas Blade organizadas (por ejemplo: `catalogo_dueño.blade.php`).
  - Estilos con **Tailwind CSS** (y/o Bootstrap, según configuración del proyecto).
  - Interactividad ligera con **Alpine.js** en componentes clave.

> ⚠️ Nota: Algunas funcionalidades pueden estar en desarrollo o planificadas según la rama o etapa del proyecto.

---

## 🧱 Stack tecnológico

- **Backend:** Laravel (PHP)
- **Frontend:** Blade, Tailwind CSS / Bootstrap, Alpine.js
- **Base de datos:** MySQL / MariaDB
- **Servidor local:** XAMPP / Laravel Sail / similar
- **Control de versiones:** Git + GitHub

---


