# 🖥️ HosTec - Tienda de Accesorios para Computadoras

HosTec es un proyecto web de comercio electrónico desarrollado en **React + Vite (Frontend)** y **Node.js + Express (Backend)**, con **Supabase** como base de datos y autenticación.  

---

## 🚀 Tecnologías utilizadas
- **Frontend**
  - React + Vite
  - TypeScript
  - React Router
  - CSS personalizado
- **Backend**
  - Node.js
  - Express
  - Supabase SDK
- **Base de Datos**
  - Supabase (PostgreSQL)

---

📌 Funcionalidades

🔐 Autenticación: Login con correo/contraseña desde tabla usuarios.

🛒 Carrito de compras: Agregar, eliminar y pagar productos.

📦 Gestión de productos: Listado dinámico desde Supabase.

💳 Pagos: Integración con PayPal (opcional).

📧 EmailJS: Envío de correos desde formularios (opcional).



---

📡 Endpoints del Backend

🔐 Autenticación (/api/auth)

POST /api/auth/register → Registrar usuario.

{
  "nombre": "Juan",
  "correo": "juan@example.com",
  "contraseña": "123456"
}

POST /api/auth/login → Iniciar sesión.

{
  "correo": "juan@example.com",
  "contraseña": "123456"
}



---

📦 Productos (/api/products)

GET /api/products → Listar todos los productos.

GET /api/products/:id → Obtener un producto por ID.

POST /api/products → Agregar producto (solo admin).

{
  "name": "Teclado Mecánico",
  "price": 899,
  "stock": 20,
  "image_url": "https://misimagenes.com/teclado.jpg"
}



---

🛒 Carrito (/api/cart)

GET /api/cart/:user_id → Obtener carrito de un usuario.

POST /api/cart → Agregar producto al carrito.

{
  "user_id": "98bd9e6b-2b86-4fb0-85e6-d5e191e9fcbc",
  "product_id": 2,
  "cantidad": 1
}

DELETE /api/cart/:id → Eliminar un producto del carrito.



---

🔮 Mejoras futuras

Autenticación con Google y Facebook.

Implementar facturación automática.

Dashboard para administrador.

Integración con API de envíos (DHL o FedEx).
