# fullstack-project-orchestrator

Skill “director técnico” para coordinar el flujo profesional de construcción de proyectos fullstack usando el kit de skills.

Esta skill **no implementa código** ni define arquitectura en detalle por sí sola: su función es **clasificar el proyecto**, **estimar complejidad**, detectar restricciones, y **activar el orden correcto de skills** (y omitir las innecesarias) con justificación.

---

## Qué produce

- Clasificación del proyecto (tipo de producto)
- Estimación de complejidad (baja / media / alta)
- Restricciones y supuestos detectados
- Flujo recomendado: orden de ejecución de skills
- Justificación del orden y dependencias
- Skills omitidas y por qué
- Riesgos de alterar el orden
- Próximo paso inmediato (qué skill ejecutar ahora)

---

## Cuándo usarla

- Al iniciar un proyecto desde cero
- Al re-arquitectar un proyecto existente
- Cuando el equipo no tiene claro “por dónde empezar”
- Para alinear trabajo técnico con roadmap y prioridades
- Para evitar sobre-ingeniería en MVPs

---

## Skills que orquesta (kit)

Orden base (puede variar según el proyecto):

1. `project-architecture-planner`
2. `roadmap-and-writing-plans`
3. `api-contract-designer`
4. `express-api-scaffold`
5. `auth-jwt-rbac-designer` (si aplica)
6. `react-feature-scaffold`
7. `quality-baseline-setup`
8. `deploy-readiness-checklist`
9. `observability-baseline`
10. `performance-audit-fullstack`
11. `documentation-and-onboarding`
12. `feature-brainstorming-framework`
13. `doc-coauthoring-structured`

> Nota: el orquestador puede omitir o reordenar skills según tipo de proyecto, riesgo y escala.

---

## Ejemplos de prompts

- “Vamos a iniciar un e-commerce con React + Express + Postgres. Orquestá el flujo del kit.”
- “Tengo un MVP CRUD interno para una escuela. ¿Qué skills aplico y en qué orden?”
- “Quiero un SaaS multiusuario con roles y pagos. Elegí el flujo y justificalo.”
- “Tengo un repo caótico. Definí un plan de re-arquitectura y qué skills ejecutar.”

---

## Resultado esperado

Una salida clara y accionable que indique:

- **Qué hacer primero**
- **Qué sigue después**
- **Qué se omite**
- **Por qué**

y que permita ejecutar las skills del kit en un flujo consistente.

---

## No hace

- No genera implementación completa.
- No escribe código final.
- No reemplaza a las skills especializadas (solo coordina).
