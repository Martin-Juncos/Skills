# Reglas de ejecución (observability-baseline)

## Principios

- Observabilidad útil > volumen de logs.
- Trazabilidad: requestId en toda respuesta y logs del backend.
- Seguridad: nunca loguear secretos.
- Diseñar para producción sin depender de herramientas externas.

## Defaults

- Logs JSON en backend para fácil análisis.
- Niveles: debug, info, warn, error.
- Health check simple (/health) + readiness (/ready) si aplica.
- Métricas mínimas: latencia y tasa de errores por endpoint.
