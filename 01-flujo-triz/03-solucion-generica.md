# Etapa 3: Solución Genérica

## Objetivo

Aplicar las herramientas TRIZ al modelo genérico formulado en la [Etapa 2](02-problema-generico.md) para obtener **principios, patrones o direcciones de solución** abstractas.

## Herramienta según el modelo

### A. Si formulaste una contradicción técnica → Matriz de Contradicciones

**Procedimiento**:

1. Localizar el **parámetro que mejora** en las filas de la [Matriz de Contradicciones](../04-matriz-contradicciones/00-como-usar-la-matriz.md).
2. Localizar el **parámetro que empeora** en las columnas.
3. En la celda de cruce, leer los **números de principios inventivos** sugeridos (típicamente 2-4 principios).
4. Consultar cada principio en la [referencia de 40 Principios](../02-principios-inventivos/00-indice-principios.md).

**Ejemplo** (barco):
```
Mejora: #13 Estabilidad del objeto
Empeora: #25 Pérdida de tiempo
Celda: 35, 28, 34, 4
→ Principio 35: Cambio de parámetros físicos/químicos
→ Principio 28: Reemplazo del sistema mecánico
→ Principio 34: Descarte y recuperación
→ Principio 4: Asimetría
```

### B. Si formulaste una contradicción física → Principios de separación

**Procedimiento**:

1. Aplicar los cuatro principios de separación y evaluar si alguno resuelve la CF:

| Separación | Pregunta clave | Ejemplo (pintura líquida/sólida) |
|-----------|---------------|--------------------------------|
| **En el tiempo** | ¿Puede ser A ahora y no-A después (o viceversa)? | La pintura es líquida al aplicarla y se solidifica después (ya es así, pero ¿se puede acelerar?) |
| **En el espacio** | ¿Puede ser A en un lugar y no-A en otro? | Líquida en el contenedor, sólida al contacto con el metal |
| **Entre todo y partes** | ¿Pueden las partes ser A y el todo no-A? | Micropartículas sólidas suspendidas en líquido (pintura en polvo electrostática) |
| **Bajo condición** | ¿Puede ser A bajo una condición y no-A bajo otra? | Líquida a alta temperatura, sólida a temperatura ambiente (recubrimiento termoplástico) |

2. Cada separación que funcione genera una dirección de solución.

### C. Si formulaste un modelo Su-Campo → 76 Soluciones Estándar

**Procedimiento**:

1. Clasificar el modelo Su-Campo:
   - **Incompleto** (falta S2 o F) → Clase 1: completar el modelo
   - **Dañino** (interacción no deseada) → Clase 1: destruir o neutralizar
   - **Insuficiente** (interacción débil) → Clase 2: mejorar el modelo
   - **Problema de detección/medición** → Clase 4

2. Ir a la clase correspondiente en las [76 Soluciones Estándar](../06-soluciones-estandar/00-indice-soluciones.md).
3. Revisar las soluciones de esa clase y seleccionar las aplicables.

### D. Si el problema es complejo → ARIZ-85C

Cuando las herramientas anteriores no generan soluciones satisfactorias, escalar al [algoritmo ARIZ-85C](../07-ariz/00-que-es-ariz.md), que integra todas las herramientas en un proceso de 9 partes.

## Trabajar con múltiples principios

La Matriz y las 76 Soluciones rara vez dan una única respuesta. Lo normal es obtener 3-6 direcciones de solución. Para cada una:

1. **Leer la definición completa** del principio o solución (con subprincipios y ejemplos).
2. **Registrar las ideas** que sugiere para el problema específico, sin filtrar.
3. **No descartar prematuramente**: un principio que parece irrelevante puede inspirar una solución inesperada.

## Combinación de herramientas

No es necesario elegir una sola herramienta. Es frecuente y recomendable:

- Formular el problema como CT *y* como CF, y comparar las soluciones.
- Formular como modelo Su-Campo y buscar en las 76 Soluciones *además* de usar la Matriz.
- Usar las Leyes de Evolución para verificar que la solución está alineada con la tendencia evolutiva del sistema.

## Registro de resultados

Para cada dirección de solución genérica, documentar:

```
Herramienta usada: [Matriz / Separación / 76 Soluciones / ARIZ]
Principio/Solución: [Número y nombre]
Idea generada: [Descripción breve de la idea en el contexto del problema]
Viabilidad inicial: [Alta / Media / Baja / Por evaluar]
```

---

**Navegación**: [← Etapa 2: Problema genérico](02-problema-generico.md) · [Etapa 4: Solución específica →](04-solucion-especifica.md)
