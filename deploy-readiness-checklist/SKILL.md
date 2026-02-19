---
name: deploy-readiness-checklist
description: Genera una checklist profesional y accionable para preparar un proyecto fullstack (React + Node/Express + DB) para despliegue. Úsala antes de publicar a producción o cuando el usuario pida “deploy”, “producción”, “release”, “preparar para subir”, “checklist de despliegue”.
metadata:
  short-description: Checklist de readiness para producción
  version: "1.0.0"
  risk: medium
---

# Deploy Readiness Checklist

## 🎯 Objetivo

Preparar el proyecto para producción con una checklist clara, priorizada y verificable.

Produce:

- Checklist de configuración (env, build, runtime)
- Requisitos mínimos de seguridad
- Verificaciones de calidad previas al deploy
- Recomendaciones de observabilidad
- Plan de rollback básico
- Riesgos típicos y cómo mitigarlos

---

## 🧠 Cuándo activarse

Activar cuando el usuario:

- Está por desplegar (Render, Vercel, Railway, etc.)
- Quiere checklist de producción
- Tiene errores típicos de deploy (env, build, CORS, DB)
- Pide “release” o “publicar”

---

## 📥 Entrada esperada

- Plataforma objetivo (si se conoce)
- Arquitectura (monorepo o separado)
- Backend (Express) y Frontend (React)
- DB (Postgres/Mongo) y proveedor
- Si hay auth (JWT/cookies)
- Variables de entorno actuales (si se comparten)

Si falta info: asumir deploy estándar separado FE/BE, con env vars y build.

---

## 📤 Salida obligatoria (orden estricto)

1️⃣ Resumen del escenario de despliegue (supuestos si faltan datos)  
2️⃣ Checklist priorizada (P0, P1, P2)  
3️⃣ Variables de entorno (listado recomendado por componente)  
4️⃣ Configuración de producción (CORS, logging, errores)  
5️⃣ Build & artifacts (qué se genera y cómo validar)  
6️⃣ DB readiness (migrations/índices/conexión)  
7️⃣ Observabilidad mínima (logs, health check)  
8️⃣ Seguridad mínima (headers, rate limit, secretos)  
9️⃣ Plan de rollback (simple)  
🔟 Errores comunes y diagnóstico rápido  

---

## 📌 Reglas obligatorias

- Checklist verificable: cada ítem debe indicar cómo confirmar.
- No asumir proveedor específico si no se indicó.
- No pedir herramientas complejas: baseline realista.
- No exponer secretos ni recomendar hardcode.
- Diferenciar claramente frontend vs backend.
