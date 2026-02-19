# Environment & Secrets

Checklist mínima:
- Todas las variables sensibles en env (no en código).
- Separar env de dev y prod.
- Confirmar que el backend no loguea secretos.
- Rotación posible (documentar dónde cambiar).

Ejemplos comunes:
- DATABASE_URL / DB_HOST+DB_USER+DB_PASS
- JWT_SECRET
- FRONTEND_URL (CORS)
- NODE_ENV=production
