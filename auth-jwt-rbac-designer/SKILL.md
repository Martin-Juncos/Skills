---
name: auth-jwt-rbac-designer
description: Diseña autenticación JWT y autorización RBAC profesional para APIs en Node/Express y su integración con frontend React. Úsala cuando el usuario necesite login, protección de rutas, roles/permisos, manejo de tokens o hardening básico de auth.
metadata:
  short-description: Diseño JWT + RBAC profesional
  version: "1.0.0"
  risk: medium
---

# Auth JWT + RBAC Designer

## 🎯 Objetivo

Definir un diseño completo de autenticación y autorización basado en JWT y RBAC.

Produce:

- Flujo de autenticación (login/refresh/logout)
- Estrategia de tokens (access/refresh)
- Estructura de claims
- Modelo de roles/permisos (RBAC)
- Middlewares (auth, authorize)
- Contrato de endpoints de auth (alto nivel)
- Checklist de seguridad

---

## 🧠 Cuándo activarse

Activar cuando el usuario:

- Requiere login/registro
- Necesita proteger endpoints o rutas
- Menciona roles, permisos, admin/user
- Quiere JWT, refresh tokens, sesiones
- Pide seguridad base para API

---

## 📥 Entrada esperada

- Roles requeridos (si los conoce)
- Recursos a proteger
- Si hay refresh token (sí/no)
- Tipo de almacenamiento (cookies httpOnly vs localStorage)
- Tipo de app (SPA, SSR, mobile)

Si falta info: asumir SPA React + API Express, usar access+refresh.

---

## 📤 Salida obligatoria (orden estricto)

1️⃣ Resumen del enfoque (JWT + RBAC)  
2️⃣ Flujos: login → acceso → refresh → logout  
3️⃣ Estrategia de tokens (duración, almacenamiento, rotación)  
4️⃣ Claims recomendados (sub, roles, etc.)  
5️⃣ RBAC: roles, permisos, matriz de acceso  
6️⃣ Middlewares: auth + authorize (responsabilidades)  
7️⃣ Endpoints de auth (alto nivel)  
8️⃣ Integración en frontend (alto nivel)  
9️⃣ Checklist de seguridad (priorizado)  
🔟 Decisiones pendientes y riesgos  

---

## 📌 Reglas obligatorias

- No implementar código completo (solo diseño + pseudocódigo breve si hace falta).
- No recomendar guardar access token en localStorage si se elige enfoque con cookies; explicar tradeoffs.
- No exponer secretos, no hardcodear keys.
- Ser específico: duraciones, claims, endpoints, responsabilidades.
