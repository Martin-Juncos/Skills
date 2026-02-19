---
name: db-migration-and-index-strategy
description: Diseña una estrategia profesional de migraciones e índices para PostgreSQL (Sequelize) y/o MongoDB (Mongoose). Úsala al iniciar un proyecto con persistencia, antes de producción o cuando haya problemas de performance/consultas lentas.
metadata:
  short-description: Migraciones + índices (Postgres/Mongo)
  version: "1.0.0"
  risk: medium
---

# DB Migration & Index Strategy

## 🎯 Objetivo

Definir una estrategia segura y mantenible para evolucionar el esquema y optimizar consultas.

Produce:

- Estrategia de migraciones (cómo, cuándo, dónde)
- Convención de versionado/naming de migraciones
- Checklist de seguridad de despliegue (rollout/rollback)
- Estrategia de índices basada en patrones de consulta
- Recomendaciones para entornos (dev/staging/prod)
- Plan incremental de adopción

---

## 🧠 Cuándo activarse

Activar cuando el usuario:

- Está empezando un proyecto con DB
- Va a desplegar a producción
- Necesita migraciones ordenadas
- Tiene queries lentas o problemas de performance
- Quiere definir índices correctos

---

## 📥 Entrada esperada

- DB: PostgreSQL o MongoDB (o ambas)
- ORM/ODM: Sequelize / Mongoose (si aplica)
- Entorno: solo dev / staging / prod
- Patrones de consulta principales (ej: buscar por email, filtrar productos, paginado)
- Volumen estimado (si se conoce)

Si falta info:
