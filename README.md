# devflow-server
🛒 E-Commerce Backend
📌 Descripción

E-Commerce Backend es la API que soporta un sistema de tienda online completo. Provee autenticación segura, gestión de usuarios, productos, pedidos y pagos. Está diseñado para ser escalable, mantenible y fácil de integrar con cualquier frontend.

👉 Repositorio Frontend: https://github.com/NahuelAnselmo/devflow-client#

🚀 Características Principales

Autenticación con JWT + Bcrypt.

CRUD completo para usuarios y productos.

Gestión de pedidos (crear, modificar, cancelar).

Validación con Joi para datos seguros.

Manejo de errores centralizado con códigos de estado HTTP.

Logs de requests con Morgan.

CORS habilitado para conectar con el frontend.

🛠️ Tecnologías

Node.js + Express (API REST).

MongoDB + Mongoose (base de datos NoSQL).

JWT + Bcrypt (autenticación).

Joi (validación de datos).

Postman / Thunder Client (testeo de API).

📂 Estructura del Proyecto
📦 ecommerce-backend
 ┣ 📂 src
 ┃ ┣ 📂 config      # Configuración (db, env)
 ┃ ┣ 📂 controllers # Lógica de negocio
 ┃ ┣ 📂 middlewares # Middlewares (auth, validaciones)
 ┃ ┣ 📂 models      # Modelos de Mongoose
 ┃ ┣ 📂 routes      # Definición de endpoints
 ┃ ┗ 📂 utils       # Helpers y utilidades
 ┣ 📜 .env.example  # Variables de entorno de ejemplo
 ┣ 📜 package.json
 ┗ 📜 README.md

⚙️ Requisitos Previos

Antes de instalar y ejecutar el proyecto, asegúrate de tener:

Node.js (v16 o superior).

MongoDB (local o MongoDB Atlas).

Git instalado.

Editor recomendado: Visual Studio Code.

📥 Instalación

Clonar el repositorio:

git clone https://github.com/NahuelAnselmo/devflow-server.git
cd TU_REPO_BACK


Instalar dependencias:

npm install


Crear archivo .env en la raíz del proyecto con estas variables:

PORT=3000
MONGODB_URI=mongodb+srv://<usuario>:<password>@cluster0.mongodb.net/ecommerce
JWT_SECRET=tuClaveSecreta


Iniciar el servidor en modo desarrollo:

npm run dev

📡 Endpoints principales
👤 Usuarios

POST /api/users/register → Crear usuario.

POST /api/users/login → Login y token.

GET /api/users/:id → Obtener perfil.

PUT /api/users/:id → Editar usuario.

DELETE /api/users/:id → Eliminar usuario.

🛍️ Productos

GET /api/products → Listar productos.

POST /api/products → Crear producto.

PUT /api/products/:id → Editar producto.

DELETE /api/products/:id → Eliminar producto.

📦 Pedidos

POST /api/orders → Crear pedido.

GET /api/orders/:id → Obtener detalle.

PUT /api/orders/:id → Modificar pedido.

DELETE /api/orders/:id → Cancelar pedido.

🧪 Testing

Podés usar Postman o Thunder Client (extensión de VSCode) para probar los endpoints.

🚀 Despliegue

El proyecto puede desplegarse fácilmente en:

Render / Railway (backend).

MongoDB Atlas (base de datos).

📜 Licencia

Este proyecto está bajo licencia MIT.

👥 Equipo

Desarrollado por:

Nahuel Anselmo