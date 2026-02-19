# Selección de patrones (guía operativa)

Antes de elegir un patrón, responder:
1) ¿Qué problema específico resuelve?
2) ¿Cuál es la alternativa más simple viable?
3) ¿Se puede postergar y agregar luego?

Señales para patrones comunes:
- Repository: testabilidad fuerte, múltiples fuentes o queries complejas.
- DDD parcial: reglas de negocio relevantes y cambios frecuentes en lógica.
- Modular monolith: equipo pequeño/medio, dominios separados, despliegue único.
- Microservicios: solo con dominios muy claros + equipo grande + escalado diferenciado.
