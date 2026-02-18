# Contrato de API (base)

## Convención de respuesta
- Éxito: { ok: true, data: <payload> }
- Error: { ok: false, error: { code, message, details? } }

## Errores
- 400: validación
- 401: no autenticado
- 403: no autorizado
- 404: recurso inexistente
- 409: conflicto
- 500: error inesperado

## Versionado
- /api/v1 como default para proyectos que evolucionan
