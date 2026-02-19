# Production Config

Backend:
- CORS: origen explícito (no "*") si hay auth sensible.
- Manejo de errores: no exponer stack trace en prod.
- Timeouts: configurar si la plataforma lo requiere.
- Rate limiting en endpoints críticos (auth).

Frontend:
- Base URL de API por env.
- Build con variables correctas.
