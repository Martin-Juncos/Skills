---
name: systematic-debugging-framework
description: Aplica un framework sistemático de debugging para proyectos fullstack (React/Node/DB/CI/Deploy). Úsala cuando haya errores, fallas de build, CI roto, bugs en runtime, problemas de integración, CORS, auth, DB o comportamientos intermitentes.
metadata:
  short-description: Debugging profesional paso a paso
  version: "1.0.0"
  risk: low
---

# Systematic Debugging Framework

## 🎯 Objetivo

Resolver problemas técnicos con un proceso reproducible, trazable y eficiente.

Produce:

- Triage (clasificación y severidad)
- Hipótesis priorizadas
- Pasos de reproducción
- Plan de instrumentación (logs/mediciones)
- Aislamiento de causa raíz
- Fix propuesto + validación
- Prevención (test/regla/checklist)

---

## 🧠 Cuándo activarse

Activar cuando el usuario:

- Reporta un error o bug
- Tiene fallas de CI/build
- Problemas de deploy/producción
- Errores de CORS, auth, DB
- Comportamientos inconsistentes o intermitentes
- Performance degradada

---

## 📥 Entrada esperada

Ideal:
- Mensaje de error exacto
- Stacktrace / logs
- Contexto (qué cambió, cuándo empezó)
- Entorno (local/CI/prod)
- Pasos para reproducir

Si falta info, pedirla dentro del output (sin bloquear el avance).

---

## 📤 Salida obligatoria (orden estricto)

1️⃣ Resumen del problema (con supuestos si falta info)  
2️⃣ Triage: severidad + impacto + alcance  
3️⃣ Reproducción mínima (pasos + datos)  
4️⃣ Hipótesis (3–7) priorizadas por probabilidad/impacto  
5️⃣ Pruebas para confirmar/descartar (por hipótesis)  
6️⃣ Instrumentación recomendada (logs, flags, métricas)  
7️⃣ Aislamiento (qué componente descartar primero y por qué)  
8️⃣ Fix propuesto (acción concreta)  
9️⃣ Validación del fix (cómo verificar)  
🔟 Prevención (test, lint rule, checklist, doc)  

---

## 📌 Reglas obligatorias
