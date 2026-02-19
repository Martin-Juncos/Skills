---
name: observability-baseline
description: Define una base profesional de observabilidad (logging, correlación, métricas, health checks y reporte de errores) para proyectos fullstack, especialmente Node/Express. Úsala al preparar producción, cuando falte visibilidad de fallas o al estandarizar logs y monitoreo.
metadata:
  short-description: Observabilidad mínima profesional
  version: "1.0.0"
  risk: medium
---

# Observability Baseline

## 🎯 Objetivo

Implementar una base de observabilidad que permita:

- Diagnosticar fallas rápido
- Medir latencia y tasas de error
- Detectar caídas (health)
- Investigar incidentes (correlación)
- Evitar exposición de información sensible

Produce:

- Estrategia de logging (backend + frontend)
- Correlación requestId
- Métricas mínimas recomendadas
- Endpoints de health y readiness
- Recomendaciones de error reporting
- Checklist de producción

---

## 🧠 Cuándo activarse

Activar cuando el usuario:

- Va a desplegar o ya está en producción
- No encuentra causas de errores (logs pobres)
- Quiere estandarizar logging
- Pide monitoreo, health check, métricas
- Tiene incidentes y necesita trazabilidad

---

## 📥 Entrada esperada

- Entorno objetivo (local/CI/prod)
- Stack (Express/React)
- Plataforma (si se conoce)
- Requisitos (retención logs, alertas)
- Si se usa reverse proxy/load balancer (si se conoce)

Si falta info: asumir stack Express + React, deploy estándar.

---

## 📤 Salida obligatoria (orden estricto)

1️⃣ Resumen del baseline propuesto  
2️⃣ Logging backend (qué, cómo, niveles)  
3️⃣ Correlación requestId (flujo y campos)  
4️⃣ Logging frontend (mínimo útil)  
5️⃣ Métricas mínimas (qué medir y por qué)  
6️⃣ Health/Readiness checks (diseño)  
7️⃣ Error reporting (estrategia)  
8️⃣ Checklist de seguridad en logs (anti-leaks)  
9️⃣ Plan de adopción incremental (pasos)  
🔟 Riesgos y decisiones pendientes  

---

## 📌 Reglas obligatorias

- No recomendar logging de secretos (tokens, passwords, cookies).
- Las propuestas deben ser implementables sin herramientas complejas.
- Si se sugiere una herramienta, debe ser opcional.
- Diferenciar health vs readiness.
- Siempre incluir un plan incremental (adoptar por etapas).
