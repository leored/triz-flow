---
description: Ejecuta una sesión completa de análisis TRIZ sobre un reto existente
---

Ejecuta una sesión de análisis TRIZ sobre el reto "$ARGUMENTS".

## Pasos

1. Determina el directorio del reto:
   - Si `$ARGUMENTS` está vacío, busca el único directorio en `challenges/` o pide al usuario que especifique.
   - Si hay argumento, busca `challenges/{argumento}/`.

2. Verifica que existe `challenges/{nombre}/00-challenge.md` y que tiene contenido más allá de la plantilla vacía. Si no, pide al usuario que lo complete primero.

3. Invoca al agente `@facilitador` pasándole:
   - La ruta del challenge: `challenges/{nombre}/`
   - Instrucción de ejecutar la sesión completa

El facilitador se encargará de:
- Leer el reto y los expertos
- Elegir la secuencia de rondas según el tipo de problema
- Invocar cada lente TRIZ en orden
- Guardar resultados por ronda en `02-analysis/session-NN/`
- Generar la síntesis final en `03-synthesis/session-NN.md`
