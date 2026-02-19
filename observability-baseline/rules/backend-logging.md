# Backend Logging (Express)

Recomendación:
- Formato: JSON
- Campos mínimos:
  - timestamp
  - level
  - requestId
  - method
  - path
  - status
  - durationMs
  - userId (si existe, opcional y sanitizado)
  - errorCode (si aplica)

Niveles:
- info: requests exitosos (o sampling si hay alto tráfico)
- warn: validaciones, rate limit, casos esperables
- error: excepciones, 5xx, fallas externas
