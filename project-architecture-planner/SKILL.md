---
name: project-architecture-planner
description: Diseña la arquitectura inicial y estándares de un proyecto fullstack profesional (React/Node/DB), definiendo estructura de repo, capas, contratos, convenciones, checklist, trade-offs y plan de ejecución. Úsala al iniciar un proyecto nuevo, al re-arquitectar uno existente, o cuando el usuario pida “estructura”, “arquitectura”, “scaffold”, “setup inicial”, “cómo organizar el repo”, “buenas prácticas”, “convenciones”, “estándares”, “MVP plan”.
metadata:
  short-description: Arquitectura + estándares + trade-offs + plan inicial
  version: "1.1.0"
  risk: low
---

# Project Architecture Planner

## Objetivo
Producir un diseño de arquitectura inicial (práctico y aplicable), incluyendo:
- Descubrimiento de contexto (preguntas/variables críticas).
- Decisiones explícitas y justificadas (trade-offs).
- Estructura de carpetas (monorepo o multi-repo).
- Contratos y convenciones (Git, naming, linting, tests).
- Modelo de datos inicial (alto nivel).
- Contrato de API (alto nivel).
- Checklist de calidad y seguridad.
- Plan de ejecución por fases (MVP → v1).
- (Opcional) C4 Context textual y/o Mermaid.

## Cuándo activarse
Activa esta skill si el usuario:
- Inicia un proyecto (“arrancamos de cero”, “setup”, “estructura del repo”).
- Pide arquitectura (“capas”, “patrones”, “DDD”, “MVC”, “service layer”, “clean”).
- Quiere un kit profesional (“estándares”, “convenciones”, “workflow GitHub”).
- Pide un plan de implementación (“roadmap”, “MVP”, “fases”).
- Tiene un repo caótico y quiere orden estructural.

## Cuándo NO activarse
No la uses si:
- La solicitud es un cambio pequeño y aislado que no afecta arquitectura.
- El usuario solo pide “un snippet” sin impacto transversal.

## Entrada mínima (si no está disponible, declarar supuestos)
Si el usuario no dio detalles, asumir valores sensatos y declarar supuestos:

- Tipo de producto (CRUD, e-commerce, dashboard, landing+API).
- Frontend (React + router + estado).
- Backend (Node/Express).
- DB (PostgreSQL o MongoDB).
- Auth (sí/no, JWT).
- Deploy (local / Render / Vercel / Docker).
- Equipo (solo / equipo) y horizonte (MVP vs producto).

## Modo de trabajo (obligatorio)
1) Descubrimiento de contexto (rápido, enfocado).
2) Propuesta de arquitectura mínima viable.
3) Análisis de trade-offs de decisiones claves.
4) Estándares + estructura + contratos.
5) Plan por fases.

Si falta info:
- No bloquear: declarar supuestos y ofrecer 2 opciones cuando el impacto sea alto.

## Salida obligatoria (formato y orden)
Entregar SIEMPRE estas secciones, en este orden:

1. Resumen ejecutivo (10–12 líneas)
2. Descubrimiento de contexto (preguntas + supuestos declarados)
3. Decisiones de arquitectura (con criterio)
   - Monorepo vs multi-repo
   - Capas y responsabilidades
   - Patrones (cuáles sí / cuáles no) con umbrales de adopción
4. Estructura de carpetas propuesta
   - Árbol de directorios
5. Contrato de API (alto nivel)
   - endpoints principales + convención de respuestas/errores
6. Modelo de datos (alto nivel)
   - entidades + relaciones + índices sugeridos
7. Git & GitHub workflow
   - ramas, commits, PR, issues, CI mínimo
8. Trade-offs y ADR (decisiones relevantes)
   - 2 a 5 ADR “cortos” (en formato)
9. Seguridad y calidad (checklist)
10. Plan de ejecución por fases (MVP → v1)
11. (Opcional) C4 Context (textual / Mermaid)
12. Riesgos y decisiones pendientes

## Estándares de entrega
- Cada decisión debe tener justificación concreta (requisitos/constraints).
- Evitar “depende” sin resolver: si depende, ofrecer 2 opciones con criterio.
- Mantener consistencia terminológica: capas, rutas, naming, convenciones.
- No inventar requisitos: si faltan datos, declarar supuestos.
- Preferir simplicidad: agregar complejidad solo cuando existan señales claras.

## Plantillas rápidas (internas)
- Respuesta API estándar:
  - Éxito: { ok: true, data: <payload> }
  - Error: { ok: false, error: { code, message, details?, requestId? } }

- Backend (Express):
  routes/ controllers/ services/ repositories/ middlewares/ validators/ config/ utils/

- Frontend (React):
  app/ pages/ features/ components/ hooks/ services(api)/ store/ styles/
