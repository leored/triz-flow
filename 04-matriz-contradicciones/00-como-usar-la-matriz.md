# Cómo usar la Matriz de Contradicciones

## Qué es la Matriz de Contradicciones

La Matriz de Contradicciones de TRIZ es una tabla de 39 × 39 que relaciona **parámetros que mejoran** (filas) con **parámetros que empeoran** (columnas). En cada celda de intersección se indican los **principios inventivos** que, según el análisis estadístico de patentes, han resuelto con mayor frecuencia ese tipo de contradicción técnica.

La matriz fue desarrollada por **Genrich Altshuller** y su equipo a partir del análisis de más de 40 000 patentes de invención. Al estudiar cada patente, identificaron qué contradicción técnica se había resuelto y qué principio inventivo se había empleado. Las combinaciones más recurrentes se volcaron en esta tabla, que sirve como mapa de orientación para el inventor.

## Los 39 parámetros de ingeniería

Altshuller definió 39 parámetros genéricos que describen las características de cualquier sistema técnico. Algunos ejemplos:

| #  | Parámetro |
|----|-----------|
| 01 | Peso del objeto móvil |
| 02 | Peso del objeto estacionario |
| 03 | Longitud del objeto móvil |
| 04 | Longitud del objeto estacionario |
| 05 | Área del objeto móvil |
| …  | *(ver la lista completa en cada archivo de la matriz)* |
| 39 | Productividad |

Cada parámetro puede actuar como *parámetro que mejora* (fila) o como *parámetro que empeora* (columna), dependiendo de la contradicción que se analice.

## Paso a paso para usar la Matriz

### 1. Formular la contradicción técnica

Defina con claridad qué quiere mejorar en su sistema y qué empeora como consecuencia no deseada. Por ejemplo: "quiero aumentar la resistencia de una pieza (parámetro 14 — Resistencia), pero al hacerlo aumenta su peso (parámetro 01 — Peso del objeto móvil)".

### 2. Identificar el parámetro que mejora

Busque en la lista de 39 parámetros aquel que mejor describa la característica que desea mejorar. Este será su **fila** en la matriz. En el ejemplo: parámetro 14 (Resistencia).

### 3. Identificar el parámetro que empeora

Busque el parámetro que describe la característica que se degrada como efecto secundario. Este será su **columna**. En el ejemplo: parámetro 01 (Peso del objeto móvil).

### 4. Localizar la celda de intersección

Vaya al archivo de la matriz que contenga su parámetro de mejora y busque la tabla correspondiente. En la columna "Parámetro que empeora" localice el parámetro identificado en el paso 3. La celda contigua contiene los números de los principios sugeridos.

### 5. Leer los principios sugeridos

Cada celda contiene típicamente entre 2 y 4 números que corresponden a los 40 principios inventivos. En nuestro ejemplo, la intersección fila 14 × columna 01 podría indicar algo como `1, 8, 40, 15`.

### 6. Estudiar cada principio y generar ideas

Consulte la descripción de cada principio sugerido en el [Índice de principios inventivos](../02-principios-inventivos/00-indice-principios.md). Para cada principio:

- Lea la descripción general y los sub-principios.
- Revise los ejemplos.
- Pregúntese: *¿Cómo podría aplicar este principio a mi problema concreto?*
- Anote todas las ideas, incluso las que parezcan impracticables en un primer momento.

## Formato de la documentación de la Matriz

En esta documentación, la matriz completa se ha dividido en **5 archivos** organizados por rangos de parámetros de mejora:

| Archivo | Parámetros de mejora |
|---------|---------------------|
| [01-matriz-mejora-01-08.md](01-matriz-mejora-01-08.md) | 01 – 08 |
| [02-matriz-mejora-09-16.md](02-matriz-mejora-09-16.md) | 09 – 16 |
| [03-matriz-mejora-17-24.md](03-matriz-mejora-17-24.md) | 17 – 24 |
| [04-matriz-mejora-25-31.md](04-matriz-mejora-25-31.md) | 25 – 31 |
| [05-matriz-mejora-32-39.md](05-matriz-mejora-32-39.md) | 32 – 39 |

Cada archivo contiene encabezados de nivel 2 con el número y nombre del parámetro de mejora, seguido de una tabla de dos columnas:

- **Parámetro que empeora**: número y nombre del parámetro.
- **Principios sugeridos**: números de los principios inventivos recomendados, separados por comas, o "—" si no se encontró una recomendación fuerte en el análisis de patentes.

La diagonal (un parámetro contra sí mismo) se omite en cada tabla.

## Ejemplo resuelto

**Problema**: Se tiene un chasis de vehículo que debe ser más resistente a impactos (para mejorar la seguridad), pero al reforzarlo con más material el peso aumenta, lo que incrementa el consumo de combustible.

**Paso 1 — Contradicción técnica**:
- Mejorar: Resistencia (parámetro 14).
- Empeora: Peso del objeto móvil (parámetro 01).

**Paso 2 y 3** — Ya identificados arriba.

**Paso 4** — Abrir el archivo de la matriz correspondiente al parámetro de mejora 14 y buscar la fila del parámetro que empeora 01.

**Paso 5** — Supongamos que la celda indica los principios: `1, 8, 40, 15`.

**Paso 6 — Generar ideas**:

| Principio | Nombre | Idea generada |
|-----------|--------|---------------|
| 1 | Segmentación | Dividir el chasis en secciones modulares con diferentes grosores según la zona de impacto. |
| 8 | Contrapeso | Usar el propio peso del motor como elemento de absorción de impacto, redistribuyendo masas. |
| 40 | Materiales compuestos | Sustituir acero por fibra de carbono o materiales compuestos: mayor resistencia, menor peso. |
| 15 | Dinamismo | Diseñar zonas de deformación programada que cambien de rigidez en el momento del impacto. |

De estas ideas, la más prometedora puede desarrollarse y validarse con prototipos.

## Consejos prácticos

- **Pruebe ambas direcciones**: si la búsqueda con el par (mejora A, empeora B) no produce ideas satisfactorias, invierta la contradicción y busque (mejora B, empeora A). Los principios sugeridos pueden ser diferentes y complementarios.

- **Formule múltiples contradicciones**: un mismo problema puede describirse con distintos pares de parámetros. Explore varias formulaciones para obtener un conjunto más amplio de principios.

- **Celdas con "—"**: significan que en el análisis original de patentes no se encontró una recomendación estadísticamente fuerte para esa combinación. No significa que no haya solución; simplemente la matriz no ofrece orientación directa. En esos casos, intente reformular la contradicción con parámetros cercanos.

- **La matriz es un punto de partida**: no sustituye al pensamiento creativo del ingeniero. Los principios son direcciones de búsqueda, no recetas. La calidad de la solución depende de cómo se interpreten y adapten al contexto específico.

- **Combine principios**: a menudo las mejores soluciones surgen de la combinación de dos o más principios inventivos aplicados simultáneamente.

## Enlaces de referencia

- [Índice de los 40 principios inventivos](../02-principios-inventivos/00-indice-principios.md)
- [Matriz: Parámetros de mejora 01–08](01-matriz-mejora-01-08.md)
- [Matriz: Parámetros de mejora 09–16](02-matriz-mejora-09-16.md)
- [Matriz: Parámetros de mejora 17–24](03-matriz-mejora-17-24.md)
- [Matriz: Parámetros de mejora 25–32](04-matriz-mejora-25-31.md)
- [Matriz: Parámetros de mejora 33–39](05-matriz-mejora-32-39.md)

---

**Navegación**: [← Índice de principios](../02-principios-inventivos/00-indice-principios.md) · [Matriz: Parámetros 01-08 →](01-matriz-mejora-01-08.md)
