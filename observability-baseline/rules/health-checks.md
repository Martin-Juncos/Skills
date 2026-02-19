# Health & Readiness

/health:
- indica que el proceso está vivo
- responde 200 con { ok: true, uptime, version? }

/ready:
- indica que puede servir tráfico
- valida dependencias críticas (ej: DB conectada)
- si falla: 503

No incluir datos sensibles en estas respuestas.
