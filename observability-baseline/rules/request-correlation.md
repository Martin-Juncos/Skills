# Request Correlation (requestId)

Objetivo:
- Trazar una request extremo a extremo

Estrategia:
- Generar requestId si no viene (o respetar header upstream)
- Incluir en:
  - logs backend
  - header de respuesta (X-Request-Id)
  - payload de error (error.requestId) si aplica

Evitar requestId predecible si se expone públicamente.
