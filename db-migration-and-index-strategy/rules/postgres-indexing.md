# PostgreSQL Indexing

Índices típicos:
- UNIQUE en email/username (si aplica)
- Índice en foreign keys usadas en joins
- Índice compuesto cuando se filtra por (A,B) frecuentemente
- Índice para ORDER BY si hay paginado por campo estable

Regla:
- Un índice es útil si coincide con WHERE/JOIN/ORDER BY reales.

Validación:
- EXPLAIN (ANALYZE) para confirmar mejoras.
