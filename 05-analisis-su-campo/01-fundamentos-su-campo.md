# Fundamentos del Análisis Sustancia-Campo (Su-Campo)

El **Análisis Sustancia-Campo** (en ruso: вепольный анализ, *vepolnyi analiz*; abreviado **Vepol** o **Su-Campo**) es una herramienta de TRIZ que permite modelar cualquier sistema técnico como una interacción mínima entre **sustancias** y **campos**, con el fin de diagnosticar problemas y dirigir la búsqueda de soluciones de forma sistemática.

## Origen histórico

El Análisis Su-Campo fue desarrollado por **Genrich Altshuller** a partir de **1973** como parte de la evolución de TRIZ. Altshuller observó que las soluciones inventivas en patentes seguían patrones recurrentes que podían describirse como transformaciones en modelos de sustancias y campos. Esta observación condujo a dos contribuciones fundamentales:

1. **El modelo Su-Campo** (1973): una notación mínima para representar la estructura funcional de un sistema técnico.
2. **Las 76 Soluciones Estándar** (1975-1985, con colaboradores como Shulyak, Zlotin y Zusman): un catálogo de transformaciones modelo que resuelven clases de problemas Su-Campo.

> Ver: [76 Soluciones Estándar](../06-soluciones-estandar/00-indice-soluciones.md)

El Su-Campo complementa la Matriz de Contradicciones y los 40 Principios Inventivos. Mientras la Matriz trabaja con parámetros de ingeniería en conflicto, el Su-Campo trabaja con la **estructura funcional** del sistema y sus interacciones.

> Ver: [Matriz de Contradicciones](../04-matriz-contradicciones/00-como-usar-la-matriz.md) · [40 Principios Inventivos](../02-principios-inventivos/00-indice-principios.md)

## Los tres elementos del modelo Su-Campo

Todo sistema técnico funcional puede representarse con un modelo mínimo de **tres elementos**:

```
        F (Campo / Interacción)
       / \
      /   \
     /     \
   S1 ───── S2
```

| Elemento | Nombre | Rol | Definición |
|----------|--------|-----|------------|
| **S1** | Sustancia-objeto | Receptor de la acción | El objeto sobre el que se actúa; es el elemento que debe ser procesado, movido, detectado, modificado o controlado |
| **S2** | Sustancia-herramienta | Ejecutor de la acción | El elemento que actúa sobre S1; es la herramienta, dispositivo o agente que realiza la función |
| **F** | Campo (interacción) | Mediador energético | La energía o interacción que permite a S2 actuar sobre S1; describe el *tipo* de acción |

### Concepto de "sustancia" en Su-Campo

En el contexto del Análisis Su-Campo, **sustancia** no se limita a un material químico. Una sustancia es cualquier **objeto material** que participa en la interacción:

- Una pieza mecánica
- Un líquido o gas
- Un organismo biológico
- Una herramienta, máquina o dispositivo
- Una partícula, fibra o grano
- Un campo magnético materializado (como un ferrofluido)

Lo esencial es que S1 y S2 son **entidades materiales distinguibles** que participan en la función.

### Concepto de "campo" en Su-Campo

El **campo** (F, del ruso *поле*, "pole") representa la **forma de interacción** o la **energía** que media entre las sustancias. Altshuller adoptó el término "campo" en sentido amplio, más allá de la definición estricta de la física.

## Tipos de campos

TRIZ reconoce los siguientes tipos principales de campos, ordenados aproximadamente por nivel de controlabilidad creciente:

| Campo | Abreviatura | Descripción | Ejemplos de aplicación |
|-------|-------------|-------------|----------------------|
| **Gravitacional** | F_grav | Interacción debida a la gravedad | Caída libre, sedimentación, peso propio |
| **Mecánico** | F_mec | Fuerzas de contacto, presión, fricción, vibración, ondas acústicas | Prensado, pulido, ultrasonidos, centrifugación |
| **Térmico** | F_term | Transferencia de calor (conducción, convección, radiación) | Calentamiento, enfriamiento, dilatación térmica |
| **Químico** | F_quim | Reacciones químicas, interacciones moleculares | Oxidación, catálisis, disolución, polimerización |
| **Eléctrico** | F_elec | Campos electrostáticos, corrientes eléctricas | Electrodeposición, electrostática, electroforesis |
| **Magnético** | F_mag | Campos magnéticos permanentes o generados por corriente | Separación magnética, sujeción, MRI |
| **Electromagnético** | F_em | Ondas electromagnéticas (luz, microondas, rayos X, etc.) | Láser, fotopolimerización, detección óptica |
| **Nuclear** | F_nuc | Interacciones nucleares, radiactividad | Radiografía industrial, esterilización por radiación |

### Jerarquía de controlabilidad de campos

Una de las tendencias evolutivas de los sistemas técnicos es la transición hacia campos más **controlables**:

```
Menos controlable ──────────────────────────── Más controlable

Gravitacional → Mecánico → Térmico → Químico → Eléctrico → Magnético → Electromagnético
```

Esta tendencia es relevante al aplicar la **Regla 3 de transformación** (cambiar el tipo de campo) y las **Leyes de evolución** de sistemas técnicos.

> Ver: [Leyes de Evolución](../08-leyes-evolucion/00-vision-general.md)

## El modelo mínimo completo (triángulo Su-Campo)

La unidad funcional mínima en TRIZ es el **triángulo Su-Campo completo**: un modelo donde los tres elementos (S1, S2, F) están presentes y la interacción es funcional.

```
        F
       / \
      /   \          Modelo mínimo completo:
     /     \         S2 actúa sobre S1 a través del campo F
    /       \
  S1 ─────── S2
```

### Principio fundamental

> **Para que un sistema técnico funcione, debe contener al menos un modelo Su-Campo completo (S1, S2, F). Si falta alguno de los tres elementos, el sistema es incompleto y no funcional.**

Este principio tiene consecuencias directas para la resolución de problemas:

- Si el modelo está **incompleto** → hay que completarlo (añadir el elemento faltante).
- Si el modelo está **completo pero dañino** → hay que modificar o neutralizar la interacción.
- Si el modelo está **completo pero insuficiente** → hay que mejorar la interacción.

> Ver: [Modelos básicos Su-Campo](02-modelos-basicos.md)

## Cómo construir un modelo Su-Campo desde un problema

El proceso de modelado Su-Campo transforma una descripción verbal de un problema técnico en un diagrama estructurado que revela qué falta o qué falla.

### Paso 1: Identificar la función principal

Determinar cuál es la **acción útil** que el sistema debe realizar.

```
Ejemplo: "Necesitamos limpiar piezas metálicas de aceite residual."
Función: Eliminar aceite de la superficie de piezas metálicas.
```

### Paso 2: Identificar S1 (sustancia-objeto)

Preguntar: **¿Sobre qué objeto se ejerce la acción?**

```
S1 = pieza metálica con aceite residual
```

### Paso 3: Identificar S2 (sustancia-herramienta)

Preguntar: **¿Qué elemento realiza la acción sobre S1?**

```
S2 = ¿? (si no existe, el modelo está incompleto)
S2 = disolvente (si ya se usa uno actualmente)
S2 = onda ultrasónica + líquido (si se usa limpieza ultrasónica)
```

### Paso 4: Identificar F (campo / interacción)

Preguntar: **¿Qué tipo de energía o interacción permite que S2 actúe sobre S1?**

```
F = campo químico (disolución)
F = campo mecánico (vibración ultrasónica)
F = campo térmico (si se usa calor para volatilizar el aceite)
```

### Paso 5: Diagnosticar el modelo

Evaluar qué tipo de modelo resulta:

| Diagnóstico | Condición | Acción |
|------------|-----------|--------|
| Modelo **incompleto** | Falta S2 o F | Completar el modelo |
| Modelo **dañino** | F causa efecto nocivo sobre S1 | Neutralizar el daño |
| Modelo **insuficiente** | F es demasiado débil | Intensificar o cambiar F |
| Modelo **completo y funcional** | Todo correcto | No hay problema Su-Campo |

### Ejemplo completo de modelado

**Problema**: "La pintura se aplica sobre la superficie metálica con rodillo, pero la capa queda irregular."

**Paso 1** — Función: depositar pintura uniformemente sobre superficie metálica.

**Paso 2** — S1 = superficie metálica (objeto que recibe la pintura).

**Paso 3** — S2 = rodillo con pintura (herramienta que aplica la pintura).

**Paso 4** — F = campo mecánico (presión y movimiento del rodillo).

**Paso 5** — Diagnóstico: el modelo está **completo pero con interacción insuficiente** (la capa queda irregular, es decir, el efecto mecánico no logra uniformidad).

```
        F_mec
       / \
      /   \          F_mec actúa de S2 a S1
     / ~~> \         pero el efecto es INSUFICIENTE
    /       \        (~~> = interacción insuficiente)
  S1 ─────── S2
  (superficie) (rodillo)
```

**Dirección de solución**: según las reglas de transformación Su-Campo, se puede:

- Modificar S2 (usar un rodillo texturizado, electrostático, etc.)
- Cambiar F (pasar de campo mecánico a campo eléctrico → pintura electrostática)
- Introducir S3 (una sustancia intermedia, como un agente nivelador en la pintura)

> Ver: [Reglas de transformación](03-transformaciones.md) · [76 Soluciones Estándar](../06-soluciones-estandar/00-indice-soluciones.md)

## Relación del Su-Campo con otras herramientas TRIZ

```
    Problema técnico
          │
    ┌─────┴──────┐
    ▼             ▼
Contradicción   Modelo
  técnica      Su-Campo
    │             │
    ▼             ▼
  Matriz →    76 Soluciones
  40 Principios  Estándar
    │             │
    └─────┬───────┘
          ▼
       ARIZ-85C
    (integra ambos)
```

El Análisis Su-Campo es especialmente útil cuando:

- El problema no se expresa fácilmente como una contradicción entre dos parámetros.
- Se necesita **mejorar, modificar o controlar** una interacción existente.
- Hay un **efecto dañino** que debe eliminarse sin perder la función útil.
- Se busca una forma más **sistemática** de explorar alternativas que la Matriz de Contradicciones.

> Ver: [Conceptos clave de TRIZ](../00-fundamentos/03-conceptos-clave.md) · [ARIZ-85C](../07-ariz/00-que-es-ariz.md)

## Resumen

| Concepto | Definición |
|----------|-----------|
| **Sustancia (S)** | Cualquier objeto material que participa en la interacción |
| **Campo (F)** | La forma de energía o interacción entre sustancias |
| **Modelo Su-Campo** | Representación mínima de un sistema como triángulo S1-S2-F |
| **Modelo completo** | Los tres elementos presentes, interacción funcional |
| **Modelo incompleto** | Falta S2 o F; el sistema no funciona |
| **Modelo dañino** | F causa efecto nocivo sobre S1 |
| **Modelo insuficiente** | F es demasiado débil para cumplir la función |

---

**Navegación**: [← Soluciones estándar](../06-soluciones-estandar/00-indice-soluciones.md) · [Modelos básicos →](02-modelos-basicos.md)
