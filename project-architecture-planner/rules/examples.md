# Ejemplos (cómo aterrizar decisiones)

Ejemplo 1 (MVP, solo dev)
- Monolito/modular simple
- ORM directo si CRUD es simple
- Postgres si hay órdenes/pagos

Ejemplo 2 (equipo 5-10)
- Modular monolith
- Separación por dominios
- Repository selectivo donde haya complejidad

Ejemplo 3 (escala alta)
- Distribución selectiva
- Observabilidad obligatoria
- Eventos solo donde haya tolerancia a consistencia eventual
