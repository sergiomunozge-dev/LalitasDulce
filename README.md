# 🍰 LalitasDulce - E-commerce de Repostería Tradicional Chilena

Plataforma de comercio electrónico especializada en la venta de productos de repostería tradicional chilena e internacional. El sistema implementa una arquitectura de microservicios diseñada para ofrecer escalabilidad, seguridad avanzada y una experiencia de usuario fluida en dispositivos móviles.
🚀 Características Principales

    Autenticación Robusta: Registro con MFA, gestión de sesiones mediante JWT y cookies httpOnly.

    Catálogo Inteligente: Filtros dinámicos para productos según categorías y condiciones especiales (Veganos, Sin Azúcar, Sin Gluten).

    Gestión de Compras: Carrito en tiempo real y persistencia de historial de pedidos.

    Fidelización: Módulo de suscripciones y beneficios exclusivos para usuarios registrados.

    Multipasarela de Pago: Integración nativa con Flow, Mercado Pago y Stripe.

    Panel Administrativo: Control total de inventario, stock, precios y gestión de usuarios para administradores.

# 🛠️ Stack Tecnológico
## Backend (Arquitectura de Microservicios)

    Runtime: Node.js

    Framework: Express

    Seguridad: Bcrypt (Hasing), Jsonwebtoken (Cifrado), Cookie-parser (Mitigación XSS), Helmet (Cabeceras HTTP).

    Infraestructura: API Gateway con http-proxy-server, Rate Limit para mitigación de ataques DDoS.

    Base de Datos: MongoDB con Mongoose (ODM).

    Logs y Auditoría: Morgan (Desarrollo) y Pino (Producción en formato JSON).

## Frontend

    Librería Principal: React

    Enrutamiento: React Router Dom

    Estilos: CSS3 / Tailwind CSS (Enfoque Mobile First)

    Estado: Context API / Zustand

## Testing y Calidad

    Unit Testing: Jest

    Integration Testing: Supertest

# 📦 Instalación y Configuración
## Requisitos Previos

    Node.js (v18+)

    Instancia de MongoDB (Local o Atlas)

## Pasos

    Clonar el repositorio:
    Bash

    git clone https://github.com/usuario/lalitas-dulce.git

    Instalar dependencias del Gateway y Servicios:
    Bash

    npm install

    Configuración de Variables de Entorno (.env):
    Cree un archivo .env en cada microservicio siguiendo el formato:
    Fragmento de código

    PORT=3000
    MONGO_URI=tu_url_de_conexion
    JWT_SECRET=tu_clave_secreta
    STRIPE_KEY=tu_api_key

    Ejecutar en modo Desarrollo:
    Bash

    npm run dev

# 🏗️ Estructura del Proyecto

    /gateway: Punto de entrada único, manejo de CORS y Proxy.

    /services/auth: Microservicio de identidad y seguridad.

    /services/products: Gestión de catálogo y stock.

    /services/payments: Integración con pasarelas externas.

    /client: Aplicación frontend en React.

# 🧪 Ejecución de Pruebas

Para ejecutar la suite de pruebas unitarias y de integración:
Bash

npm test

📄 Licencia

Este proyecto es de uso privado. Todos los derechos reservados a LalitasDulce.