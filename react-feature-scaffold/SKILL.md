---
name: react-feature-scaffold
description: Genera la estructura profesional de una feature en React alineada con arquitectura limpia y contrato de API. Úsala cuando el usuario quiera implementar una funcionalidad frontend conectada a backend.
metadata:
  short-description: Scaffold profesional de feature React
  version: "1.0.0"
  risk: low
---

# React Feature Scaffold

## 🎯 Objetivo

Generar la estructura organizada de una feature en React.

Incluye:

- Carpeta de feature
- Componentes principales
- Hooks personalizados
- Servicio de API
- Integración opcional con Redux
- Manejo de loading y errores
- Buenas prácticas de separación de responsabilidades

---

## 🧠 Cuándo activarse

Activar cuando el usuario:

- Pide crear una feature React
- Quiere integrar frontend con API
- Necesita organizar componentes correctamente
- Quiere aplicar arquitectura por features

---

## 📥 Entrada esperada

- Nombre de la feature (ej: products, users)
- Operaciones necesarias (listar, crear, editar, eliminar)
- Si usa Redux o estado local
- Si requiere autenticación
- Si usa Tailwind u otro sistema de estilos

Si falta información, declarar supuestos.

---

## 📤 Salida obligatoria (orden estricto)

1️⃣ Resumen de la feature  
2️⃣ Estructura de carpeta generada  
3️⃣ Código base de:
   - Página principal
   - Componentes
   - Hook personalizado
   - Servicio API
4️⃣ Manejo de loading y errores  
5️⃣ Integración opcional con Redux  
6️⃣ Buenas prácticas aplicadas  
7️⃣ Checklist de calidad  

---

## 📌 Reglas obligatorias

- No mezclar lógica de negocio en componentes de UI.
- Extraer llamadas HTTP a servicios separados.
- Usar hooks personalizados para lógica reutilizable.
- Mantener componentes pequeños y específicos.
- Mantener consistencia con contrato de API.
