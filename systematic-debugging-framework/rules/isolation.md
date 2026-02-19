# Isolation Strategy

Orden recomendado:
1) Confirmar repro
2) Aislar capa: FE vs BE vs DB vs red
3) Aislar módulo: auth, routing, build, config
4) Aislar cambio reciente (git bisect mental o real)
5) Reducir a un caso mínimo

Evitar tocar 5 archivos sin saber causa.
