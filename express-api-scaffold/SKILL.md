---
name: express-api-scaffold
description: Genera la estructura profesional de un endpoint o módulo en Express siguiendo arquitectura por capas (routes → controllers → services → repositories → validators). Úsala cuando el usuario quiera implementar un recurso backend ya definido en el contrato de API.
metadata:
  short-description: Scaffold profesional de backend Express
  version: "1.0.0"
  risk: low
---

# Express API Scaffold

## 🎯 Objetivo

Generar la estructura profesional de backend para un recurso específico.

Incluye:

- route
- controller
- service
- repository
- validator
- manejo de errores
- integración opcional de JWT
- ejemplo de endpoint completo

---

## 🧠 Cuándo activarse

Activar cuando el usuario:

- Pide crear un endpoint en Express
- Quiere estructurar un recurso backend
- Necesita implementar un contrato ya definido
- Quiere aplicar arquitectura por capas

---

## 📥 Entrada esperada

- Nombre del recurso (ej: users, products)
- Operaciones requeridas (CRUD o específicas)
- DB utilizada (Postgres o Mongo)
- Si requiere autenticación
- Si usa Sequelize o Mongoose

Si falta información, declarar supuestos.

---

## 📤 Salida obligatoria (orden estricto)

1️⃣ Resumen del recurso  
2️⃣ Estructura de archivos generada  
3️⃣ Código base de:
   - Route
   - Controller
   - Service
   - Repository
   - Validator
4️⃣ Manejo centralizado de errores  
5️⃣ Integración opcional de middleware JWT  
6️⃣ Consideraciones de seguridad  
7️⃣ Checklist de calidad  

---

## 📌 Reglas obligatorias

- Separar responsabilidades correctamente.
- No mezclar lógica de acceso a datos en controllers.
- No validar dentro del controller.
- No acceder directamente a DB desde route.
- Mantener coherencia con el contrato de API.
