# Context Discovery (guía breve)

Objetivo: captar variables que cambian decisiones.

## Jerarquía de preguntas (orden recomendado)
1) Escala
- Usuarios esperados: 10 / 1k / 100k / 1M+
- Volumen de datos: MB / GB / TB
- Tráfico: req/min o req/s, picos

2) Equipo
- Solo / equipo
- Tamaño y seniority
- Ritmo de entrega y QA

3) Horizonte / timeline
- MVP (semanas) vs producto (meses/años)
- Riesgo de pivote

4) Dominio
- CRUD puro vs reglas de negocio complejas
- Tiempo real (sí/no)
- Integraciones externas (pagos, auth, envíos, etc.)

5) Restricciones
- Presupuesto
- Infra (Render/Vercel/Docker/K8s)
- Requisitos de compliance (si aplica)
- Preferencias tecnológicas

## Clasificación rápida (heurística)
- MVP: simplicidad + velocidad + monolito/modular básico
- Producto SaaS (equipo medio): modular monolith + boundaries + tests
- Escala alta/equipo grande: distribución selectiva (solo si se justifica)
