# Inventario de Productos

Aplicación web empresarial para el módulo de registro de productos en un sistema de inventario.

## Estructura del proyecto

/project-root
├── /frontend
│   ├── index.html
│   ├── /css
│   ├── /js
│   └── /assets
├── /backend
│   ├── server.js
│   ├── /routes
│   ├── /controllers
│   ├── /models
│   ├── /config
│   └── /middlewares
├── package.json
└── README.md

## Instalación

1. Abre una terminal en la carpeta del proyecto.
2. Ejecuta:

```bash
npm install
```

## Ejecución

Inicia el servidor:

```bash
npm run dev
```

Luego abre tu navegador en:

```text
http://localhost:3000
```

## Qué incluye esta primera fase

- Formulario profesional para registrar productos.
- Validación en frontend y backend.
- Catálogo dinámico de productos en memoria.
- API RESTful con endpoints:
  - `GET /productos`
  - `POST /productos`
- Arquitectura preparada para conectar con base de datos relacional.

## Cómo conectar una base de datos en el futuro

1. Edita `backend/config/database.js` para usar el cliente y credenciales de MySQL o PostgreSQL.
2. Cambia `backend/models/productModel.js` para reemplazar el almacenamiento en memoria con consultas a la base de datos.
3. Mantén la separación entre controladores, modelos y rutas para minimizar cambios.

## Notas adicionales

- El frontend se sirve de manera estática desde Express.
- El backend valida siempre los datos recibidos antes de almacenar.
- El sistema está listo para evolución a un API más completo y persistencia real.
