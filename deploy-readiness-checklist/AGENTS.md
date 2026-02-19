# Reglas de ejecución (deploy-readiness-checklist)

## Principios

- Priorizar items P0 (bloqueantes).
- Cada item debe tener verificación clara (cómo comprobar).
- No depender de una plataforma específica si no se menciona.
- Separar FE y BE siempre.

## Defaults

- Health check endpoint en backend.
- Logs estructurados sin datos sensibles.
- CORS configurado explícitamente.
- Variables de entorno documentadas.
