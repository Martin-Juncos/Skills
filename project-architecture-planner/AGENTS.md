# Reglas de ejecución (project-architecture-planner)

## Principios
- Priorizar decisiones explícitas por sobre generalidades.
- Proponer defaults profesionales si faltan datos y declararlos como supuestos.
- Mantener consistencia: nombres de carpetas, capas, endpoints y convenciones.

## Convenciones recomendadas (por defecto)
- API REST con Express.
- Validación de entrada (schema) antes de controllers.
- Separación de capas: controller → service → repository.
- Manejo de errores centralizado.
- Config por entorno mediante variables (sin hardcode).

## Git/GitHub (por defecto)
- Convencional: Conventional Commits.
- PR obligatorio para main.
- CI mínimo: lint + test + build (cuando aplique).

## Calidad mínima
- Linting + formatting definidos.
- Estructura de errores y respuestas consistente.
- Checklist de seguridad base (headers, rate limiting, validación, secretos).
