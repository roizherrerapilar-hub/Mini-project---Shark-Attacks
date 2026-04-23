# 🦈 Shark Attack Analysis — Diving School Location Strategy

## Objetivo
Identificar los 3 destinos más seguros del mundo para abrir una escuela de buceo,
analizando el histórico de ataques de tiburón a nivel global.
La selección se basa en la tasa de fatalidad por país y la estacionalidad de los ataques,
con el fin de minimizar el riesgo para los futuros estudiantes. 

## Dataset

- **Fuente:** Global Shark Attack File (GSAF) — registro histórico real de ataques de tiburón a nivel mundial
- **Registros originales:** 78.395 filas × 15 columnas
- **Registros tras limpieza:** ~4.017 filas útiles para el análisis
- **Cobertura temporal:** Histórico global hasta 2026

### Variables principales utilizadas

| Variable | Tipo | Descripción |

| `country` | Categórica | País donde ocurrió el ataque |
| `state` | Categórica | Estado o región |
| `location` | Categórica | Lugar específico del ataque |
| `activity` | Categórica | Actividad que realizaba la víctima |
| `age` | Numérica | Edad de la víctima |
| `injury` | Texto | Descripción de la herida |
| `species` | Categórica | Especie de tiburón involucrada |
| `fatal` | Booleana | Si el ataque fue mortal (derivada de `injury`) |
| `age_range` | Categórica | Rango de edad (`<18`, `18-25`, `26-35`...) |