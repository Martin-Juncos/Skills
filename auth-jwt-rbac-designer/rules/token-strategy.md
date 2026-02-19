# Token Strategy

Recomendación base:

- Access token: 10–20 min
- Refresh token: 7–30 días (según riesgo)
- Claims mínimos: sub (userId), roles, iat, exp
- Almacenamiento:
  - Preferido: refresh en cookie httpOnly; access en memoria
  - Alternativa: ambos en cookies httpOnly (según arquitectura)

Evitar exponer tokens a XSS.
