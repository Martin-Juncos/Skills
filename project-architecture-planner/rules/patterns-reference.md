# Referencia rápida (patrones y cuándo usarlos)

Data Access
- Active Record: CRUD simple, prototipo rápido.
- Repository: abstracción útil si hay testing intenso o fuentes múltiples.
- Unit of Work: transacciones complejas (costo alto).

Domain Logic
- Transaction Script: lógica simple, CRUD con validaciones.
- Domain Model / DDD parcial: reglas complejas, entidades con comportamiento.

Distribución
- Monolito: MVP, equipo chico, foco en entrega.
- Modular Monolith: dominios claros, equipo 2-10, escalado aún acoplado.
- Microservicios: necesidad real de escalado diferenciado + alta complejidad operativa.

API
- REST: default.
- GraphQL: flexibilidad de queries (costo en caching/operación).
- WebSocket: tiempo real cuando el caso lo justifica.
