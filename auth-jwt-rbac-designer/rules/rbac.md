# RBAC

Definir:

- Roles (ej: admin, user, moderator)
- Permisos por recurso/acción (ej: products:create, orders:read)
- Matriz de acceso: rol → permisos

No mezclar autorización en controllers: usar middleware authorize.
