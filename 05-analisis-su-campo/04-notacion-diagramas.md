# Notación Textual para Diagramas Su-Campo

Este documento define un sistema de **notación textual consistente** para representar diagramas Su-Campo en formato Markdown. Dado que esta documentación es exclusivamente texto plano, se necesitan convenciones claras para representar sustancias, campos, interacciones y transformaciones sin gráficos.

> Prerrequisito: [Fundamentos Su-Campo](01-fundamentos-su-campo.md) · [Modelos básicos](02-modelos-basicos.md)

## Símbolos para sustancias

| Símbolo | Significado | Uso |
|---------|-------------|-----|
| `S1` | Sustancia-objeto | El objeto sobre el que se actúa |
| `S2` | Sustancia-herramienta | El agente que realiza la acción |
| `S3` | Tercera sustancia (intermediaria) | Sustancia añadida para modificar la interacción |
| `S1'` | S1 modificada | S1 después de una transformación |
| `S2'` | S2 modificada | S2 después de una modificación |
| `S1a, S1b` | Variantes de S1 | En bi-sistemas o poli-sistemas |
| `S2a, S2b` | Variantes de S2 | En bi-sistemas o poli-sistemas |

### Etiquetado descriptivo

Para mayor claridad, las sustancias pueden etiquetarse con su identidad real entre paréntesis:

```
S1 (pieza de acero)
S2 (herramienta de corte)
S3 (fluido refrigerante)
```

## Símbolos para campos

| Símbolo | Significado |
|---------|-------------|
| `F` | Campo genérico (tipo no especificado) |
| `F1, F2` | Primer y segundo campo (cuando hay múltiples) |
| `F_mec` | Campo mecánico (presión, fricción, vibración, ultrasonido) |
| `F_term` | Campo térmico (calor, frío) |
| `F_quim` | Campo químico (reacciones, disolución, catálisis) |
| `F_elec` | Campo eléctrico (electrostática, corriente) |
| `F_mag` | Campo magnético |
| `F_em` | Campo electromagnético (luz, láser, microondas, rayos X) |
| `F_grav` | Campo gravitacional |
| `F_nuc` | Campo nuclear |

### Campos compuestos

Cuando dos campos actúan simultáneamente se separan con `+`:

```
F_mec + F_term    (campo mecánico combinado con térmico)
F_elec + F_mag    (campo electromagnético descompuesto)
```

## Flechas e interacciones

Este es el núcleo del sistema de notación. Las flechas representan el tipo y calidad de la interacción entre los elementos del modelo Su-Campo.

### Tabla de flechas

| Flecha | Significado | Contexto de uso |
|--------|-------------|-----------------|
| `-->` o `→` | Acción normal (funcional) | Interacción útil y suficiente |
| `~~>` | Acción insuficiente | Interacción útil pero demasiado débil |
| `==>` o `═══>` | Acción fuerte / intensificada | Interacción reforzada o potenciada |
| `⤳` o `-/->` | Acción dañina | Interacción que causa efecto nocivo |
| `- - ->` o `...>` | Acción deseada pero ausente | Interacción que falta y debe crearse |
| `<-->` | Acción bidireccional | S1 y S2 interactúan mutuamente |
| `--X-->` | Acción bloqueada | Interacción impedida por una barrera |

### Uso en línea

En texto corriente, las interacciones se escriben en línea:

```
F --> S1          El campo F actúa sobre S1 (acción normal)
S2 --> S1         S2 actúa sobre S1 (acción directa)
F ~~> S1          El campo F actúa insuficientemente sobre S1
F ⤳ S1           El campo F causa daño sobre S1
F ...> S1         Se desea que F actúe sobre S1 pero aún no lo hace
```

## Notación triangular para el modelo completo

El modelo Su-Campo completo se representa como un triángulo en texto:

### Forma estándar (bloque de código)

```
        F
       / \
      /   \
     / --> \
    /       \
  S1 ─────── S2
```

### Forma compacta (una línea)

```
[S1] <--F--> [S2]
```

Se lee: "S2 actúa sobre S1 mediante el campo F."

### Forma de tabla

| Componente | Identidad | Rol |
|------------|-----------|-----|
| S1 | (nombre del objeto) | Objeto |
| S2 | (nombre de la herramienta) | Herramienta |
| F | (tipo de campo) | Interacción |

## Notación para cada tipo de modelo

### Modelo completo y funcional

```
        F
       / \
      /   \
     / --> \          Todos los elementos presentes.
    /       \         Interacción adecuada.
  S1 ─────── S2

  Forma compacta:  [S1] <--F--> [S2]    (✓ funcional)
```

### Modelo incompleto (falta S2)

```
  S1        ?         S2 no existe.
                      F no existe.
  Forma compacta:  [S1]  ...  [?]  ...  (?)

  Se necesita: introducir S2 y F.
```

### Modelo incompleto (falta F)

```
        ?
       / \
      /   \
     / ... \          S1 y S2 existen pero
    /       \         no hay campo que los conecte.
  S1 ─────── S2

  Forma compacta:  [S1] <--?--> [S2]    (falta F)
```

### Modelo con interacción dañina

```
        F
       /↯\
      / ↯  \
     / ⤳⤳⤳ \        F produce efecto dañino sobre S1.
    /       \
  S1 ←↯↯↯── S2

  Forma compacta:  [S1] <⤳⤳F⤳⤳> [S2]   (✗ dañino)
```

Alternativa ASCII pura:

```
        F
       / \
      /   \
     /-/-> \         -/-> indica interacción dañina
    /       \
  S1 ─────── S2

  Forma compacta:  [S1] <-/- F -/-> [S2]   (✗ dañino)
```

### Modelo con interacción insuficiente

```
        F
       / \
      /   \
     / ~~> \         F actúa sobre S1 pero
    /       \        el efecto es insuficiente.
  S1 ─────── S2

  Forma compacta:  [S1] <~~F~~> [S2]    (~ insuficiente)
```

## Notación para transformaciones

Las transformaciones (reglas de cambio) se representan con una flecha de transformación `==>` o `⟹` entre el modelo anterior y el modelo resultante.

### Formato general

```
ANTES                    ==>              DESPUÉS

    F                                         F
   / \                                       / \
  / ~~> \                                   / --> \
 S1 ── S2                                 S1 ──── S2'

[S1] <~~F~~> [S2]       ==>      [S1] <--F--> [S2']
(insuficiente)                    (modificar S2)
```

### Regla 1: Completar modelo

```
[S1] ... [?] ... (?)     ==>     [S1] <--F--> [S2]
(incompleto)                     (completo)
```

### Regla 2: Modificar S2

```
[S1] <~~F~~> [S2]       ==>     [S1] <--F--> [S2']
(insuficiente)                   (S2 modificada)
```

### Regla 3: Cambiar campo

```
[S1] <~~F~~> [S2]       ==>     [S1] <--F'--> [S2]
(F inadecuado)                   (nuevo tipo de campo)
```

### Regla 4: Introducir S3

```
[S1] <⤳⤳F⤳⤳> [S2]      ==>     [S1] <--F--> [S3] <--F--> [S2]
(dañino)                         (S3 como barrera o mediador)
```

### Regla 5: Introducir F2

```
[S1] <⤳⤳F⤳⤳> [S2]      ==>     [S1] <--F--> [S2]
(dañino)                                ↑
                                   F2 --┘  (campo compensatorio)
```

### Regla 6: Encadenar modelos

```
[S1] <~~F~~> [S2]       ==>     [S1] <--F1--> [S2]  →  [S1'] <--F2--> [S3]
(insuficiente)                   (cadena de dos modelos)
```

### Regla 7: Bi-sistema

```
[S1] <~~F~~> [S2]       ==>     [S1a] <--F--> [S2a]  +  [S1b] <--F--> [S2b]
(insuficiente)                   (bi-sistema homogéneo)
```

## Notación para modelos complejos

### Modelo con doble efecto (útil + dañino)

Cuando un mismo modelo produce un efecto útil y un efecto dañino simultáneamente:

```
        F
       / \
      / → \    efecto útil
     / ⤳⤳⤳ \  efecto dañino (simultáneo)
    /       \
  S1 ─────── S2

  Forma compacta:  [S1] <--F(útil)/-/->F(dañino)--> [S2]
```

### Modelo con medición / detección

Los modelos Su-Campo de detección tienen la particularidad de que la "acción" es obtener información sobre S1:

```
        F_detección
       / \
      /   \
     / info \        S2 detecta una propiedad de S1
    /       \        a través del campo F.
  S1 ─────── S2
 (objeto)   (sensor/detector)

  Forma compacta:  [S1] --F_info--> [S2_detector]
```

### Cadena de tres modelos

```
    F1                F2                F3
   / \               / \               / \
  / → \             / → \             / → \
 S1 ── S2    →    S1' ── S3    →    S1'' ── S4
 (etapa 1)        (etapa 2)         (etapa 3)

Compacta:
[S1] --F1--> [S2] → [S1'] --F2--> [S3] → [S1''] --F3--> [S4]
```

### Poli-sistema con n elementos

```
     F        F        F              F
    / \      / \      / \            / \
  S1a-S2   S1b-S2   S1c-S2  ...   S1n-S2

Compacta:  n × { [S1_i] <--F--> [S2] }   donde i = a, b, c, ..., n
```

## Cómo leer un diagrama Su-Campo textual

### Procedimiento de lectura

1. **Identificar las sustancias**: buscar todos los símbolos `S1`, `S2`, `S3`... y leer sus etiquetas entre paréntesis.
2. **Identificar los campos**: buscar `F`, `F1`, `F2`... con sus subíndices de tipo.
3. **Leer las flechas**: determinar el tipo de interacción según la flecha utilizada (ver tabla de flechas arriba).
4. **Determinar el tipo de modelo**: según las flechas, clasificar como completo, incompleto, dañino o insuficiente.
5. **Si hay `==>` (transformación)**: leer el modelo ANTES (izquierda) y DESPUÉS (derecha) para entender qué regla se aplicó.

### Ejemplo de lectura paso a paso

Dado el siguiente diagrama:

```
ANTES:                           DESPUÉS:

      F_mec                           F_elec
       / \                             / \
      /   \                           /   \
     / ~~> \           ==>           / --> \
    /       \                       /       \
  S1 ─────── S2                   S1 ─────── S2'
 (pintura)  (rodillo)            (pintura)  (pistola
                                             electrostática)
```

**Lectura**:

1. **S1** = pintura (objeto a depositar).
2. **S2** = rodillo (herramienta original); **S2'** = pistola electrostática (herramienta modificada).
3. **F_mec** = campo mecánico (antes); **F_elec** = campo eléctrico (después).
4. **Flecha `~~>`** = interacción insuficiente (antes); **Flecha `-->`** = interacción funcional (después).
5. **Tipo de modelo**: antes era insuficiente; después es completo y funcional.
6. **Transformación**: se aplicó **Regla 3** (cambiar tipo de campo: mecánico → eléctrico) junto con **Regla 2** (modificar S2: rodillo → pistola).

## Cómo escribir un diagrama Su-Campo textual

### Procedimiento de escritura

1. **Definir S1**: escribir el objeto del problema y asignarlo como S1.
2. **Definir S2**: identificar la herramienta o agente que actúa sobre S1.
3. **Definir F**: identificar el tipo de campo o energía de la interacción.
4. **Elegir la flecha correcta** según el tipo de interacción:
   - Funcional: `-->`
   - Insuficiente: `~~>`
   - Dañina: `⤳` o `-/->`
   - Ausente: `...>`
5. **Dibujar el triángulo** usando el formato estándar.
6. **Etiquetar** las sustancias con su identidad real entre paréntesis.
7. **Clasificar el modelo** y anotar el diagnóstico.

### Plantilla copiable

```
        F_(tipo)
       / \
      /   \
     / (flecha) \
    /             \
  S1 ──────────── S2
 (objeto)        (herramienta)

Diagnóstico: [completo | incompleto | dañino | insuficiente]
Dirección: Regla [1-7] → Clase [1-5] de Soluciones Estándar
```

## Ejemplo completo con notación

### Problema

"Un robot de soldadura (S2) suelda paneles de carrocería (S1) con calor de arco eléctrico (F_term + F_elec). La soldadura es buena, pero las salpicaduras de metal fundido dañan la superficie adyacente de la carrocería."

### Paso 1: Modelo actual

```
      F_term + F_elec
       /↯\
      / ↯  \
     / ↯  ↯ \
    /       \
  S1 ←↯↯↯── S2
 (panel de   (robot de
  carrocería) soldadura)

Diagnóstico: MODELO DAÑINO
  - Efecto útil: soldadura correcta de las juntas.
  - Efecto dañino: salpicaduras dañan la superficie adyacente.

Forma compacta:
  [S1 (panel)] <⤳⤳(F_term+F_elec)⤳⤳> [S2 (robot soldador)]
```

### Paso 2: Selección de regla

Según la tabla de decisión (ver [Modelos básicos](02-modelos-basicos.md)):

- Modelo dañino → **Regla 4** (introducir S3 como barrera) o **Regla 5** (introducir F2 compensatorio).

### Paso 3: Aplicar Regla 4 (introducir S3)

```
ANTES:                                DESPUÉS:

    F_term + F_elec                     F_term + F_elec
       /↯\                                  / \
      / ↯  \                               /   \
     / ⤳⤳⤳ \             ==>             / --> \
    /       \                           /    │    \
  S1 ─────── S2                       S1 ── S3 ── S2
                                     (panel)(pasta (robot)
                                            anti-
                                            salpicaduras)

Forma compacta:
  ANTES:   [S1] <⤳⤳F⤳⤳> [S2]
  DESPUÉS: [S1] <--F--> [S3 (pasta protectora)] <--F--> [S2]

  S3 = pasta anti-salpicaduras aplicada sobre la superficie
       adyacente a la zona de soldadura.
  La pasta absorbe las salpicaduras y se retira después.
```

### Paso 4: Verificación

```
Modelo resultante:

      F_term + F_elec
       / \
      /   \
     / --> \              ✓ Soldadura correcta (efecto útil conservado)
    /   │   \             ✓ Salpicaduras absorbidas por S3 (daño eliminado)
  S1 ── S3 ── S2
 (panel)(pasta)(robot)

Diagnóstico: MODELO COMPLETO Y FUNCIONAL
```

## Resumen de la notación

| Elemento | Notación | Ejemplo |
|----------|----------|---------|
| Sustancia-objeto | `S1` | `S1 (pieza metálica)` |
| Sustancia-herramienta | `S2` | `S2 (taladro)` |
| Sustancia intermedia | `S3` | `S3 (lubricante)` |
| Campo genérico | `F` | `F` |
| Campo tipado | `F_tipo` | `F_mec`, `F_term`, `F_elec` |
| Acción funcional | `-->` | `F --> S1` |
| Acción insuficiente | `~~>` | `F ~~> S1` |
| Acción dañina | `⤳` o `-/->` | `F ⤳ S1` |
| Acción ausente | `...>` | `F ...> S1` |
| Acción fuerte | `==>` | `F ==> S1` |
| Transformación | `==>` (entre modelos) | `ANTES ==> DESPUÉS` |
| Modelo completo | Triángulo `F / S1-S2` | Ver formato estándar |
| Modelo compacto | `[S1] <--F--> [S2]` | `[acero] <--F_mag--> [imán]` |

> Para aplicar estas notaciones en la resolución de problemas, ver: [Reglas de transformación](03-transformaciones.md) · [76 Soluciones Estándar](../06-soluciones-estandar/00-indice-soluciones.md)

---

**Navegación**: [← Transformaciones](03-transformaciones.md) · [76 Soluciones Estándar →](../06-soluciones-estandar/00-indice-soluciones.md)
