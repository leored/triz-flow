---
description: Crea un perfil de experto de dominio para el reto activo
---

Crea un perfil de experto de dominio basándote en la descripción: "$ARGUMENTS".

## Pasos

1. Identifica el reto activo:
   - Si solo hay un directorio en `challenges/`, úsalo.
   - Si hay varios, pregunta al usuario cuál.

2. A partir de la descripción del usuario, genera un perfil de experto usando la plantilla `templates/expert.md`. Rellena los campos de forma creativa pero realista:
   - **Nombre**: un nombre ficticio apropiado
   - **Especialidad**: derivada de la descripción
   - **Experiencia**: años y contexto mencionados, o razonables
   - **Trayectoria**: 3-4 hitos profesionales relevantes
   - **Dominios de conocimiento**: 4-6 áreas concretas
   - **Enfoque ante problemas**: cómo aborda problemas técnicos desde su expertise
   - **Sesgos y puntos ciegos**: limitaciones honestas de su perspectiva

3. Sanitiza el nombre del experto para el nombre de archivo (minúsculas, guiones).

4. Guarda en `challenges/{reto}/01-expertos/{nombre-sanitizado}.md`.

5. Muestra al usuario el perfil creado y sugiere crear más expertos de dominios diferentes para enriquecer el análisis cruzado — las mejores soluciones TRIZ vienen de otros campos.
