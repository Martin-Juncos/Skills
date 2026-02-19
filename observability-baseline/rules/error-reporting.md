# Error Reporting

Mínimo:
- Capturar errores 5xx con requestId y contexto
- No exponer stack trace en producción
- Respuesta de error estándar:
  { ok: false, error: { code, message, requestId } }

Opcional (si se desea):
- integrar un error tracker (ej: Sentry) para prod
