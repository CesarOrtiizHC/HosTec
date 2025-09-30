# 🖥️ HosTec - Tienda en Línea

Proyecto desarrollado con **React + Vite** en el frontend y **Supabase** como backend (base de datos, autenticación y almacenamiento).  
El sistema permite gestionar productos, usuarios, carritos de compra y pagos.

---

## Estructura de Carpetas

```bash
hos-tec/
│
├── public/                # Archivos estáticos (imágenes, favicon, etc.)
│
├── src/                   # Código fuente principal
│   ├── components/        # Componentes reutilizables
│   │   ├── Header.tsx     # Encabezado con login/logout
│   │   ├── Footer.tsx     # Pie de página
│   │   └── AuthContext.tsx # Manejo global de la sesión de usuario
│   │
│   ├── pages/             # Páginas del sistema
│   │   ├── Home.tsx       # Página principal con productos
│   │   ├── Productos.tsx  # Catálogo de productos
│   │   ├── Carrito.tsx    # Carrito de compras + pago con PayPal
│   │   ├── Login.tsx      # Inicio de sesión (correo/contraseña y OAuth)
│   │   ├── Registro.tsx   # Registro de nuevos usuarios
│   │   └── AdminFactura.tsx # Panel de facturación
│   │
│   ├── styles/            # Estilos CSS por página o componente
│   │   ├── Home.css
│   │   ├── Productos.css
│   │   ├── Carrito.css
│   │   ├── login.css
│   │   └── AdminFactura.css
│   │
│   ├── supabaseClient.ts  # Configuración de conexión con Supabase
│   ├── main.tsx           # Punto de entrada de la app React
│   └── App.tsx            # Configuración de rutas
│
├── package.json           # Dependencias y scripts
├── tsconfig.json          # Configuración de TypeScript
└── vite.config.ts         # Configuración de Vite
