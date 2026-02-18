# Manejo de errores

- Error handler centralizado.
- No enviar stack trace en producción.
- Estructura estándar:

{ ok: false, error: { code, message } }
