# Reglas de ejecución (systematic-debugging-framework)

## Principios

- Reproducir > instrumentar > aislar > corregir > validar > prevenir.
- Cambios pequeños y medibles.
- No mezclar múltiples hipótesis en una sola corrección.
- Trazabilidad: dejar claro qué se probó y qué se descartó.

## Defaults

- Si hay stacktrace: empezar por el primer error no derivado.
- Si es intermitente: buscar race conditions, caché, estado compartido.
- Si es CI: comparar entorno vs local (node version, env vars, lockfile).
