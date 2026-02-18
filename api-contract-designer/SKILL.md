---
name: api-contract-designer
description: Diseña contratos de API REST profesionales para proyectos fullstack con Node/Express. Úsala cuando el usuario necesite definir endpoints, estructura de request/response, manejo de errores, versionado o integración frontend-backend antes de implementar código.
metadata:
  short-description: Diseño profesional de contratos REST
  version: "1.0.0"
  risk: low
---

# API Contract Designer

## 🎯 Objetivo

Definir contratos de API claros y consistentes antes de implementar endpoints.

Esta skill produce:

- Lista estructurada de endpoints
- Métodos HTTP correctos
- Estructura de request y response
- Códigos de estado
- Manejo de errores
- Convención de versionado
- Consideraciones de seguridad

---

## 🧠 Cuándo activarse

Activar si el usuario:

- Pide diseñar endpoints
- Pregunta cómo estructurar una API
- Necesita definir integración frontend-backend
- Quiere definir contrato antes de programar
- Está diseñando backend desde cero

---

## 📥 Entrada esperada

- Tipo de recurso (usuarios, productos, pedidos, etc.)
- Operaciones necesarias (CRUD, filtros, login, etc.)
- Si requiere autenticación
- Rol de usuarios si aplica

Si falta información, declarar supuestos.

---

## 📤 Salida obligatoria (orden estricto)

1️⃣ **Resumen del recurso**
2️⃣ **Lista de endpoints**
3️⃣ **Formato de request**
4️⃣ **Formato de response**
5️⃣ **Códigos de estado**
6️⃣ **Manejo de errores**
7️⃣ **Reglas de validación**
8️⃣ **Consideraciones de seguridad**
9️⃣ **Ejemplo completo de flujo (ej: crear → obtener → actualizar)**

---

## 📌 Estándares obligatorios

### Convención de respuesta

Éxito:


{ ok: true, data: ... }


Error:



{ ok: false, error: { code, message, details? } }


---

## Reglas

- No escribir implementación.
- Ser consistente entre endpoints.
- Usar REST real (no mezclar verbos en URL).
- Mantener nombres claros y predecibles.

