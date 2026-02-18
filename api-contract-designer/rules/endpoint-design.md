# Endpoint Design

- Usar sustantivos en plural: /users
- No usar verbos en la URL
- Usar parámetros de query para filtros
- Usar parámetros de ruta para identificadores

Ejemplo:
GET /api/v1/products?category=tech
GET /api/v1/products/:id
