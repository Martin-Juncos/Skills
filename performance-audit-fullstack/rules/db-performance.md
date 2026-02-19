# DB Performance

Postgres:
- EXPLAIN (ANALYZE) en queries lentas
- índices alineados con WHERE/JOIN/ORDER BY
- paginado: preferir keyset pagination si aplica
- revisar locks y queries concurrentes

Mongo:
- query planner
- índices correctos
- evitar scans completos
- cuidado con índices excesivos (impacto en writes)
