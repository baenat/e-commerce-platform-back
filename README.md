<div align="center">

# 🛒 E-commerce Platform

<img alt="E-commerce Platform" src="cart.png" width="120" />

**Una plataforma moderna de comercio electrónico construida con Node.js, Express y MongoDB**

![Node](https://img.shields.io/badge/Node%20js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![ExpressJs](https://img.shields.io/badge/Express%20js-000000?style=for-the-badge&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)

[📖 Documentación API](https://documenter.getpostman.com/view/15768378/2sA3kPqk2j) • [💻 Frontend](https://github.com/baenat/e-commerce-platform-front)

</div>

---

## 📋 Tabla de Contenidos

- [Descripción](#-descripción)
- [Características](#-características)
- [Tecnologías](#️-tecnologías)
- [Instalación](#-instalación)
- [Configuración](#️-configuración)
- [Uso](#-uso)
- [API Endpoints](#-api-endpoints)
- [Estructura del Proyecto](#-estructura-del-proyecto)
- [Contribuir](#-contribuir)

---

## 🎯 Descripción

E-commerce Platform es una API RESTful robusta y escalable para gestionar operaciones de comercio electrónico. Proporciona funcionalidades completas para la gestión de productos, carritos de compra y procesamiento de pedidos.

### ¿Por qué usar esta plataforma?

✨ **Escalable** - Arquitectura diseñada para crecer con tu negocio  
🚀 **Moderna** - Desarrollada con las últimas tecnologías  
📦 **Completa** - Todo lo necesario para un e-commerce funcional  
🔧 **Extensible** - Fácil de personalizar y ampliar

---

## ⚡ Características

- ✅ **Gestión Completa de Productos** (CRUD)
- 🛍️ **Sistema de Carrito de Compras**
<!-- - 📦 **Procesamiento de Órdenes** -->
<!-- - 🔍 **Búsqueda y Filtrado de Productos** -->
- 📊 **Base de Datos MongoDB**
<!-- - 🔒 **API REST Segura** -->
<!-- - 📝 **Documentación Completa** -->

---

## 🛠️ Tecnologías

| Tecnología | Propósito |
|------------|-----------|
| **Node.js** | Runtime de JavaScript |
| **Express** | Framework web |
| **TypeScript** | Tipado estático |
| **MongoDB** | Base de datos NoSQL |
| **NPM** | Gestor de paquetes |

---

## 🚀 Instalación

### Prerrequisitos

Antes de comenzar, asegúrate de tener instalado:

- **Node.js** ≥ 14.0.0 ([Descargar](https://nodejs.org/))
- **MongoDB** ≥ 4.4.0 ([Descargar](https://www.mongodb.com/try/download/community))
- **npm** o **yarn**

### Pasos de Instalación

1️⃣ **Clonar el repositorio**

```bash
git clone https://github.com/baenat/e-commerce-platform-back.git
cd e-commerce-platform-back
```

2️⃣ **Instalar dependencias**

```bash
npm install
```

3️⃣ **Configurar variables de entorno**

Crea un archivo `.env` en la raíz del proyecto:

```env
PORT=3000
MONGODB_URI=mongodb://localhost:3000/
APP_VERSION=development
```

---

## ⚙️ Configuración

### Variables de Entorno

| Variable | Descripción | Valor por Defecto |
|----------|-------------|-------------------|
| `PORT` | Puerto del servidor | `3000` |
| `MONGODB_URI` | URI de conexión a MongoDB | `mongodb://localhost:3000/` |
| `APP_VERSION` | Versión | `1` |

---

## 💻 Uso

### Modo Desarrollo

```bash
npm run dev
```

### Modo Producción

```bash
npm run build
npm start
```

El servidor estará disponible en: **`http://localhost:3000`**

### Verificar que funciona

```bash
curl http://localhost:3000/
```

**Respuesta esperada:**

```json
{
  "message": "Available Endpoints",
  "endpoints": {
    "products": "/api/v1/products",
    "orders": "/api/v1/orders"
  }
}
```

---

## 📡 API Endpoints

### 🏠 Ruta Principal

```http
GET /
```

Retorna la lista de endpoints disponibles.

### 📦 Productos

| Método | Endpoint | Descripción |
|--------|----------|-------------|
| `GET` | `/api/v1/products` | Lista todos los productos |
| `GET` | `/api/v1/products/:id` | Obtiene un producto específico |
| `POST` | `/api/v1/products` | Crea un nuevo producto |
| `PUT` | `/api/v1/products/:id` | Actualiza un producto |
| `DELETE` | `/api/v1/products/:id` | Elimina un producto |

### 📋 Órdenes

| Método | Endpoint | Descripción |
|--------|----------|-------------|
| `GET` | `/api/v1/orders` | Lista todas las órdenes |
| `GET` | `/api/v1/orders/:id` | Obtiene una orden específica |
| `POST` | `/api/v1/orders` | Crea una nueva orden |
| `PUT` | `/api/v1/orders/:id` | Actualiza una orden |
| `DELETE` | `/api/v1/orders/:id` | Elimina una orden |

### 📖 Documentación Completa

Para ejemplos detallados, esquemas de datos y pruebas de endpoints, consulta la [Documentación Completa de Postman](https://documenter.getpostman.com/view/15768378/2sA3kPqk2j).

---

## 📁 Estructura del Proyecto

```
e-commerce-platform-back/
├── src/
│   ├── controllers/     # Lógica de controladores
│   ├── database/        # Conexión MongoDB
│   ├── models/          # Modelos de MongoDB
│   ├── routes/          # Definición de rutas
│   ├── utils/           # Utils
│   └── index.ts         # Punto de entrada
├── .env                 # Variables de entorno
├── package.json
├── tsconfig.json
└── README.md
```

---

## 🤝 Contribuir

Las contribuciones son bienvenidas. Para cambios importantes:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

---

## 📄 Licencia

Este proyecto está bajo la Licencia MIT.

---

## 🔗 Enlaces Útiles

- [🌐 Frontend del Proyecto](https://github.com/baenat/e-commerce-platform-front)
- [📚 Documentación API (Postman)](https://documenter.getpostman.com/view/15768378/2sA3kPqk2j)
- [📖 Documentación de Express](https://expressjs.com/)
- [📖 Documentación de MongoDB](https://docs.mongodb.com/)

---

<div align="center">

**Desarrollado con ❤️ por [Baenat](https://github.com/baenat)**

⭐ Si te gusta este proyecto, ¡dale una estrella!

</div>
