# Reglas de ejecución (auth-jwt-rbac-designer)

## Principios

- Seguridad primero, pero pragmática.
- Explicar tradeoffs sin extenderse de más.
- Definir valores concretos (TTL, claims, endpoints).
- Mantener consistencia con el contrato de API.

## Defaults recomendados

- Access token corto (minutos)
- Refresh token más largo (días)
- Rotación de refresh si hay riesgo elevado
- RBAC por roles con permisos por recurso/acción
