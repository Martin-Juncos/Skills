# Metrics (mínimo profesional)

Medir:
- Latencia por endpoint (p50/p95 si se puede, o promedio)
- Tasa de errores (4xx, 5xx)
- Requests totales por endpoint
- Fallas de dependencias (DB, servicios externos)

Si no hay stack de métricas:
- empezar registrando durationMs en logs JSON
- luego agregar métricas reales si se requiere
