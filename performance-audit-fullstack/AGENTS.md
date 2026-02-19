# Reglas de ejecución (performance-audit-fullstack)

## Principios

- Medir primero, optimizar después.
- Hipótesis + prueba por cada sospecha.
- Priorizar quick wins y cambios reversibles.
- No sacrificar consistencia de datos por performance sin análisis.

## Defaults

- Empezar por el cuello de botella más probable: DB + endpoints críticos.
- Registrar latencia por endpoint (p95) y tiempos de query.
- Frontend: revisar bundle y re-renders en pantallas críticas.
