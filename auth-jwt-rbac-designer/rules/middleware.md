# Middleware Responsibilities

auth middleware:
- verifica token
- adjunta user a req.user
- maneja errores 401

authorize middleware:
- verifica rol/permisos
- devuelve 403 si no corresponde
