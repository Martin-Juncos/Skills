# Logging & Instrumentation

Backend:
- log de requestId, método, ruta, status, tiempo
- log de errores con contexto (sin secretos)

Frontend:
- log de estado de la request (start/success/error)
- capturar response status y payload sanitizado

CI/Deploy:
- log de variables presentes (sin valores)
- versions: node, npm, lockfile
