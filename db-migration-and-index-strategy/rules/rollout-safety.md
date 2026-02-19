# Rollout Safety (Producción)

Estrategia recomendada:
1) Desplegar código compatible con esquema viejo y nuevo
2) Ejecutar migración (no destructiva primero)
3) Verificar métricas y errores
4) Luego aplicar cambios destructivos solo si es necesario, con ventana controlada

Checklist:
- backup/restore probado (aunque sea básico)
- plan de rollback realista
- monitoreo activo durante el cambio
