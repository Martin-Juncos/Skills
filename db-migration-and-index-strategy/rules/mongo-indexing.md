# Mongo Indexing

Índices típicos:
- { email: 1 } unique (si aplica)
- Índices en campos de búsqueda frecuentes
- Índices compuestos para filtros combinados
- TTL index si hay expiración de documentos (sessions, tokens)

Validación:
- revisar query planner y métricas de slow queries
- evitar demasiados índices: afectan escritura
