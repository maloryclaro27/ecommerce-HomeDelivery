# 🚚 Home Delivery E-commerce System  
[![Laravel](https://img.shields.io/badge/Framework-Laravel-red?logo=laravel)](https://laravel.com/)
[![MySQL](https://img.shields.io/badge/Database-MySQL-blue?logo=mysql)](https://www.mysql.com/)
[![PHP](https://img.shields.io/badge/PHP-8.2+-purple?logo=php)](https://www.php.net/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

Plataforma integral de **e-commerce y entregas inteligentes** desarrollada con **Laravel**, que conecta usuarios, negocios y administradores dentro de un ecosistema de pedidos en tiempo real, entregas programadas y seguimiento mediante **geolocalización dinámica**.

---

## 🧭 Descripción general

**Home Delivery** permite a los clientes realizar pedidos en línea, programar entregas y rastrear el estado del envío en tiempo real desde un mapa interactivo.  
El sistema integra un **programa de fidelización con puntos acumulables (SkyGo Points)**, un **módulo de negocios asociados** y un **dashboard administrativo** que gestiona la flota de transportes (motos, drones, etc.) en operación.

---

## ⚙️ Tecnologías utilizadas

| Componente | Tecnología |
|-------------|-------------|
| **Backend** | Laravel 10 (PHP 8.2) |
| **Frontend** | Blade, Tailwind CSS, Alpine.js |
| **Base de datos** | MySQL / MariaDB |
| **Geolocalización** | API GPS + Leaflet.js (mapas interactivos) |
| **Autenticación** | Middleware de roles (cliente, negocio, administrador) |
| **Servicios internos** | Jobs, Cache y Session Management de Laravel |

---

## 🧩 Funcionalidades principales

### 👥 Roles y autenticación
- **Cliente:** puede registrarse, explorar productos, realizar pedidos y ver su estado en tiempo real.  
- **Dueño de negocio:** administra el catálogo, precios, productos y domicilios asociados a su tienda.  
- **Administrador:** controla toda la plataforma desde un **panel central** con métricas, flota y pedidos activos.

---

### 🛍️ Módulo de pedidos
- 🕐 **Pedidos en tiempo real:** actualización automática del estado (pendiente, preparado, en camino, entregado).  
- 🗓️ **Entregas programadas:** permite seleccionar día y hora de entrega.  
- 🛒 **Carrito inteligente:** guarda los productos por usuario, incluyendo cantidades y tipo de establecimiento.  
- 📦 **Historial de pedidos:** consulta y reordenamiento de compras pasadas.

---

### 🗺️ Geolocalización y seguimiento
- 📍 **Mapa interactivo:** seguimiento visual del pedido desde la tienda hasta la entrega.  
- 🚚 **Ubicación GPS en vivo:** los vehículos o drones transmiten su posición en tiempo real.  
- 🔎 **Vista de administrador:** muestra todos los transportes activos con información de estado, ubicación y tiempo estimado de llegada.

---

### ✈️ Sistema de entregas inteligentes
- 🤖 **Asignación automática o manual:** los pedidos se asignan al transporte más cercano o son gestionados por el administrador.  
- 🛰️ **Control de flota:** monitoreo en vivo de drones, motos o vehículos activos.  
- 🧭 **Optimización de rutas:** prioriza entregas según cercanía y carga de trabajo.

---

### 💰 Puntos de fidelización 
- Cada pedido genera puntos equivalentes a un porcentaje del total de la compra.  
- Los puntos pueden canjearse por descuentos o beneficios especiales.  
- Los usuarios pueden consultar su saldo y historial de puntos desde su perfil.

---

### 🏪 Negocios asociados
- **Catálogo segmentado:** restaurantes, droguerías, ropa y tecnología.  
- **Gestión de productos:** creación, edición o eliminación con descripción, precio e imagen.  
- **Sección “Mi negocio”:** dashboard exclusivo para dueños, con ventas, estadísticas y pedidos activos.

---

### 📊 Dashboard administrativo
- Vista central para el control de:
  - 📦 Pedidos en curso y programados  
  - 👥 Usuarios y roles  
  - 🚁 Drones y medios de transporte activos  
  - 📈 Métricas de rendimiento (tiempos, zonas, fidelización)  
- Permite controlar estados de flota y generar reportes en tiempo real.

---

## 🔒 Seguridad y rendimiento
- Autenticación segura con middleware de roles.  
- Cifrado de contraseñas mediante bcrypt.  
- Control de sesiones y caché con drivers nativos de Laravel.  
- Validaciones de formularios y sanitización de datos.

---

## 💾 Base de datos principal

Las tablas más importantes incluyen:

| Tabla | Descripción |
|-------|--------------|
| `usuarios` | Información del usuario y puntos de fidelización |
| `productos` | Catálogo de productos por negocio |
| `orders` / `order_items` | Pedidos y detalle de productos |
| `shipping_details` | Dirección, teléfono y método de pago |
| `restaurantes`, `droguerias`, `ropa`, `tecnologia` | Negocios asociados |
| `sessions`, `cache`, `jobs` | Infraestructura de Laravel |

---

## 🧠 Arquitectura general
El sistema sigue el patrón **MVC (Model-View-Controller)** de Laravel, con módulos desacoplados para autenticación, pedidos, geolocalización y logística.  
El panel administrativo integra **actualización en tiempo real con AJAX y sockets** para reflejar cambios instantáneos.

---

## 🧩 Próximas mejoras
- Integración con pasarelas de pago (PayU, MercadoPago).  
- Control de inventario por establecimiento.  
- Notificaciones push (Firebase).  
- Estadísticas gráficas para el panel del negocio.

---

## 🪪 Licencia
Este proyecto se distribuye bajo la licencia **MIT**.  
Puedes modificarlo y reutilizarlo libremente citando la fuente original.

---

### 📫 Contacto
**Desarrollado por:** Málory Claro Ojeda  
📧 claromalory@gmail.com  
🌐 Bucaramanga, Colombia


## 🖼️ Vista general

**Interfaz principal**

--- 

![Interfaz](/interfaz_principal.png)

---

![Interfaz](/interfaz_principal1.png)

---

![Interfaz](/interfaz_principal2.png)

---

![Interfaz](/interfaz_principal3.png)

---

**Formulario de registro con roles:**

![Registro usuario](/registro_roles.png)

---

**Catálogo para clientes:**

![catalogo_cliente](/catalogo_cliente.png)

---

**Listado de tiendas**

![catalogo_tiendas](/lista_tiendas.png)

---

**Listado de restaurantes con sistema de filtrado:**

![restaurantes](/restaurantes.png)

---

**Ejemplo de pedido con un restaurante:**

![rest](/productos.png)

---

**Vista del carrito:**

![carrito](/carrito.png)

---

**Resumen de compra:**

![resumen](/compra.png)

---

**Pasarela de pagos con reducción de total del pago por puntos de fidelización::**

![pasarela](/pago.png)

---

**Checkout de compra:**

![checkout](/pago1.png)

---

**Selección de medio de transporte:**

![transporte](/transporte.png)

---

**Sistema de geolocalización del pedido:**

![geolocalizacion](/geolocalizacion.png)

---

**Historial de pedidos:**

![historial](/historial.png)

---

**Checkout de compra:**

![pagoo](/pago1.png)

---

**Dashboard del administrador para el monitoreo de los medios de transporte:**

![drones](/drones.png)









