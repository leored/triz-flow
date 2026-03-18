# TRIZ Flow

Referencia completa del método TRIZ (Teoría para Resolver Problemas de Inventiva) en español, con un sistema de dinámicas interactivas para analizar problemas técnicos aplicando distintas "lentes TRIZ".

## Estructura del método (referencia)

- `00-fundamentos/` — Qué es TRIZ, historia, conceptos clave (contradicciones, RFI, recursos)
- `01-flujo-triz/` — Flujo de 4 etapas: problema específico → genérico → solución genérica → específica
- `02-principios-inventivos/` — Los 40 principios inventivos (un archivo por principio)
- `03-parametros-ingenieria/` — Los 39 parámetros de ingeniería
- `04-matriz-contradicciones/` — Matriz de contradicciones (parámetro a mejorar × parámetro que empeora → principios sugeridos)
- `05-analisis-su-campo/` — Análisis Sustancia-Campo (modelos S1-S2-F)
- `06-soluciones-estandar/` — Las 76 soluciones estándar (5 clases)
- `07-ariz/` — ARIZ-85C completo (algoritmo de 9 partes para problemas complejos)
- `08-leyes-evolucion/` — Las 8 leyes de evolución de sistemas técnicos
- `09-recursos/` — Bibliografía, glosario ES/EN/RU, guía rápida

## Dinámica interactiva

Un facilitador orquesta el análisis de problemas técnicos invocando lentes TRIZ especializadas en rondas secuenciales. Expertos de distintos dominios aportan perspectivas diversas — alineado con el principio TRIZ de que las soluciones vienen de otros campos.

### Comandos

- `/new-challenge <nombre>` — Crea estructura de reto en `challenges/{nombre}/`
- `/run-session [nombre]` — Ejecuta sesión completa de análisis TRIZ sobre un reto
- `/create-expert <descripción>` — Crea perfil de experto de dominio para el reto activo

### Agentes (lentes TRIZ)

- `@facilitador` (opus) — Orquestador. Lee el problema, elige secuencia de herramientas, invoca lentes, sintetiza. No opina.
- `@analista` (sonnet) — Analiza el sistema: funciones, componentes, contradicciones (CT/CF), recursos disponibles.
- `@principios` (opus) — Aplica los 40 principios inventivos. Consulta la Matriz de Contradicciones.
- `@su-campo` (sonnet) — Modela como Sustancia-Campo. Aplica las 76 soluciones estándar.
- `@evolucion` (sonnet) — Aplica las 8 leyes de evolución. Predice dirección de desarrollo.
- `@idealidad` (opus) — Define el RFI, explota recursos, empuja hacia la solución ideal.

### Secuencias (el facilitador elige según el tipo de problema)

| Tipo de problema | Secuencia |
|-----------------|-----------|
| Contradicción técnica clara | Analista → Principios → Idealidad |
| Contradicción física | Analista → Principios (separación) → Idealidad |
| Problema de interacción | Analista → Su-Campo → Idealidad |
| Exploración completa | Analista → Principios → Su-Campo → Evolución → Idealidad |
| Predicción tecnológica | Analista → Evolución → Idealidad |

### Estructura por reto

```
challenges/{nombre}/
├── 00-challenge.md          # Definición del problema técnico
├── 01-expertos/             # Perfiles de expertos de dominio
├── 02-analysis/
│   └── session-NN/
│       └── round-NN.md      # Una ronda por lente TRIZ
└── 03-synthesis/
    └── session-NN.md        # Síntesis final con soluciones
```

### Plantillas

- `templates/challenge.md` — Plantilla de definición de reto técnico
- `templates/expert.md` — Plantilla de perfil de experto de dominio
