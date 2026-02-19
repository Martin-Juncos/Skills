# Backend Performance (Node/Express)

Revisar:
- Latencia por endpoint (p95)
- N+1 en consultas / loops con I/O
- Pool de DB (config y saturación)
- Serialización costosa
- Middleware pesado (auth, parsing)
- Caching en endpoints de lectura

Medición:
- durationMs en logs por request
- timings por capa: controller/service/repo
