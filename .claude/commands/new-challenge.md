---
description: Crea la estructura de un nuevo reto TRIZ en challenges/
---

Crea un nuevo reto TRIZ con el nombre "$ARGUMENTS".

## Pasos

1. Sanitiza el nombre: convierte a minúsculas, reemplaza espacios por guiones, elimina caracteres especiales. Guarda el resultado como `slug`.

2. Crea la siguiente estructura de directorios y archivos:

```
challenges/{slug}/
├── 00-challenge.md
├── 01-expertos/
├── 02-analysis/
└── 03-synthesis/
```

3. Para `00-challenge.md`, copia la plantilla de `templates/challenge.md` y rellena el título con el nombre original (sin sanitizar) que dio el usuario.

4. Confirma al usuario qué se creó y sugiérele los siguientes pasos:
   - Editar `00-challenge.md` para definir el problema técnico
   - Crear expertos con `/create-expert`
   - Ejecutar la sesión con `/run-session {slug}`
