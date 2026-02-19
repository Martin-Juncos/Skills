# Mongo Migrations (Mongoose)

Mongo es schema-flexible, pero en producción necesitás disciplina:

- Schema versioning a nivel documento (opcional)
- Migraciones por script cuando cambian estructuras críticas
- Backward compatibility: tolerar campos viejos y nuevos por un periodo
- Evitar cambios masivos sin batch y monitoreo

Regla:
- Migraciones en Mongo suelen ser “data migrations” más que “schema migrations”.
