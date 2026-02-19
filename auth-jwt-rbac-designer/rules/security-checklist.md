# Security Checklist (priorizado)

1) Validación de input (schema)
2) Hash de passwords (bcrypt)
3) Rate limiting en auth endpoints
4) Protección de secretos (.env, rotación)
5) Cookies seguras si aplica (httpOnly, secure, sameSite)
6) Logging de eventos de auth (sin datos sensibles)
7) Revocación/rotación de refresh tokens (si aplica)
8) Headers de seguridad (helmet)
