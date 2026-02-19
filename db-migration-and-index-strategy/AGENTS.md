# Reglas de ejecución (db-migration-and-index-strategy)

## Principios

- Cambios de esquema deben ser seguros y trazables.
- Índices deben responder a patrones de consulta.
- Evitar downtime cuando sea posible.
- No proponer cambios destructivos sin plan de transición.

## Defaults

- Postgres: migraciones versionadas (Sequelize CLI o herramienta equivalente).
- Mongo: cambios de schema controlados por código + migraciones ad-hoc si aplica.
- Índices: empezar por claves de búsqueda y campos de join/filtro/orden.
