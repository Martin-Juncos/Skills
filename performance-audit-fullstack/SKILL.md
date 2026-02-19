---
name: performance-audit-fullstack
description: Realiza una auditoría profesional de performance fullstack (React/Node/DB) con mediciones, hipótesis, quick wins y plan de optimización. Úsala cuando el proyecto esté lento, haya latencia alta, problemas de carga, endpoints lentos o costos elevados.
metadata:
  short-description: Auditoría de performance end-to-end
  version: "1.0.0"
  risk: medium
---

# Performance Audit Fullstack

## 🎯 Objetivo

Detectar cuellos de botella y proponer mejoras verificables en:

- Frontend (render, bundle, network)
- Backend (latencia, I/O, pool, N+1)
- Base de datos (queries, índices, locks)
- Caching (estrategia y consistencia)

Produce:

- Diagnóstico por capa
- Plan de medición
- Hipótesis priorizadas
- Quick wins (alto impacto / bajo costo)
- Plan de optimización por fases
- Validación (cómo medir mejora)

---

## 🧠 Cuándo activarse

Activar cuando el usuario:

- Reporta lentitud en UI o API
- Tiene endpoints con latencia alta
- Tiene timeouts o saturación
- Quiere optimizar consultas
- Pide “performance”, “optimización”, “caching”

---

## 📥 Entrada esperada

Ideal:
- Síntomas (q
