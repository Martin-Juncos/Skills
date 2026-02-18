# Reglas de ejecución (express-api-scaffold)

## Principios

- Arquitectura por capas obligatoria.
- Controllers solo coordinan.
- Services contienen lógica de negocio.
- Repository accede a base de datos.
- Validación antes de controller.
- Errores centralizados.

## Defaults

- Async/await.
- try/catch en controller.
- next(error) para errores.
- No exponer detalles internos.
