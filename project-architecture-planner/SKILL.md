---
name: project-architecture-planner
description: Diseña la arquitectura inicial y estándares de un proyecto fullstack profesional (React/Node/DB), definiendo estructura de repo, capas, contratos, convenciones, checklist y plan de ejecución. Úsala al iniciar un proyecto nuevo, al re-arquitectar uno existente, o cuando el usuario pida “estructura”, “arquitectura”, “scaffold”, “setup inicial”, “cómo organizar el repo”, “buenas prácticas del proyecto”, “convenciones”, “estándares”, “MVP plan”. No usar para implementar features aisladas sin contexto.
metadata:
  short-description: Arquitectura + estándares + plan inicial fullstack
  version: "1.0.0"
  risk: low
---

# Project Architecture Planner

## Objetivo
Producir un **diseño de arquitectura inicial** (práctico y aplicable) para proyectos fullstack, incluyendo:
- Decisiones explícitas de stack y patrones.
- Estructura de carpetas (monorepo o repos separados).
- Contratos y convenciones (Git, naming, linting, tests).
- Modelo de datos inicial (alto nivel).
- Contratos de API (alto nivel).
- Checklist de calidad y seguridad.
- Plan de ejecución por etapas.

## Cuándo activarse
Activa esta skill si el usuario:
- Inicia un proyecto (“arrancamos de cero”, “setup”, “estructura del repo”).
- Pide arquitectura (“capas”, “patrones”, “DDD”, “MVC”, “service layer”).
- Quiere un kit profesional (“estándares”, “convenciones”, “workflow GitHub”).
- Pide un plan de implementación (“roadmap”, “MVP”, “fases”).

## Cuándo NO activarse
No la uses si:
- La solicitud es un cambio pequeño (un componente, un endpoint puntual) y no afecta arquitectura.
- El usuario solo quiere “código rápido” sin definición de contexto (en ese caso primero solicitar contexto mínimo dentro del output).

## Entrada mínima (si no está disponible, inferir preguntas dentro del output)
Si el usuario no dio detalles, asumí valores sensatos y marcá supuestos.
- Tipo de producto (ej.: e-commerce, dashboard, CRUD, landing+API).
- Frontend (React + router + estado).
- Backend (Node/Express).
- DB (Postgres o Mongo).
- Auth (sí/no, JWT).
- Deploy (local / Render / Vercel / Docker).
- Equipo (solo / equipo) para definir workflow.

## Salida obligatoria (formato)
Entregar SIEMPRE estas secciones, en este orden:

1. **Resumen ejecutivo (10–12 líneas)**
2. **Decisiones de arquitectura**
   - Monorepo vs multi-repo
   - Capas y responsabilidades
   - Estándares de código
3. **Estructura de carpetas propuesta**
   - Árbol de directorios
4. **Contrato de API (alto nivel)**
   - endpoints principales + convenciones de respuesta/errores
5. **Modelo de datos (alto nivel)**
   - entidades + relaciones + índices sugeridos
6. **Git & GitHub workflow**
   - ramas, commits, PR, issues, CI mínimo
7. **Seguridad y calidad (checklist)**
8. **Plan de ejecución por fases (MVP → v1)**
   - tareas concretas con orden recomendado
9. **Riesgos y decisiones pendientes**
   - lista breve y accionable

## Estándares de entrega
- Sin relleno: cada decisión debe tener justificación concreta.
- Evitar “depende” sin resolver: si depende, ofrecer 2 opciones con criterio para elegir.
- Mantener consistencia terminológica: nombre de capas, rutas, convenciones.
- No inventar requisitos. Si faltan datos, declarar supuestos.

## Plantillas rápidas (para usar internamente)
- Respuesta API estándar: `{ ok, data, error }`
- Estructura backend: `routes/ controllers/ services/ repositories/ middlewares/ validators/`
- Estructura frontend: `pages/ features/ components/ hooks/ services(api)/ store/ styles/`
