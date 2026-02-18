# Response Format

Siempre usar estructura consistente:

Éxito:
{ ok: true, data: payload }

Error:
{ ok: false, error: { code, message, details? } }

No devolver datos crudos sin estructura.
