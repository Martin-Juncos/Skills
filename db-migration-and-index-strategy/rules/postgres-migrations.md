# PostgreSQL Migrations (Sequelize)

Buenas prácticas:
- Una migración por cambio lógico
- Naming con timestamp: YYYYMMDDHHmmss_descripcion
- Incluir both: up y down (cuando sea viable)
- No editar migraciones ya ejecutadas en entornos compartidos
- Ejecutar migraciones en CI/staging antes de prod

Evitar:
- operaciones pesadas en horario pico
- locks prolongados por ALTER TABLE sin plan
