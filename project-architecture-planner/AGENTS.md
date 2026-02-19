# Reglas de ejecución (project-architecture-planner)

## Principios
- Contexto primero: no proponer arquitectura sin identificar escala, equipo, horizonte y restricciones.
- Decisiones explícitas: toda elección relevante debe tener trade-offs claros.
- Simplicidad deliberada: el patrón por defecto es el más simple que cumpla requisitos.
- Consistencia: nombres de carpetas, capas, rutas y convenciones deben “encajar” entre sí.

## Convenciones (defaults recomendados)
- API REST con Express.
- Validación de entrada (schema) antes de controllers.
- Separación: controller → service → repository (solo si aporta valor).
- Errores centralizados (middleware) y respuesta estándar.
- Config por entorno mediante variables (sin hardcode).

## Umbrales para introducir complejidad
- Repository/UoW: cuando hay múltiples fuentes de datos, testing intensivo o queries complejas.
- DDD parcial: cuando el dominio tiene reglas y casos de negocio no triviales.
- Microservicios: solo con límites claros + equipo grande + necesidades de escalado diferenciado.

## Git/GitHub (por defecto)
- Conventional Commits.
- PR obligatorio para main.
- CI mínimo: lint + test + build (cuando aplique).

## Calidad mínima
- Linting + formatting definidos.
- Contrato de errores consistente.
- Checklist de seguridad base (validación, secretos, headers, rate limiting).
