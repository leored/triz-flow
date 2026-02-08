# Modelos Básicos Su-Campo

El Análisis Su-Campo clasifica los problemas técnicos según el estado del modelo sustancia-campo. Existen **cuatro tipos básicos de modelos**, cada uno con un diagnóstico claro y una dirección de solución asociada a una clase específica de las 76 Soluciones Estándar.

> Prerrequisito: [Fundamentos del Análisis Su-Campo](01-fundamentos-su-campo.md)

## Visión general de los cuatro modelos

```
┌──────────────────────────────────────────────────────────────────┐
│                    MODELOS BÁSICOS SU-CAMPO                      │
├──────────────┬──────────────┬──────────────┬─────────────────────┤
│  1. Completo │ 2. Incompleto│ 3. Dañino    │ 4. Insuficiente     │
│              │              │              │                     │
│      F       │    (F?)      │      F       │       F             │
│     / \      │      \       │     /↯\      │      / \            │
│    /   \     │       \      │    / ↯  \    │     / ~~>\          │
│   /     \    │        \     │   /  ↯   \   │    /      \         │
│  S1 ─── S2  │  S1    (S2?) │  S1 ←↯── S2  │  S1 ───── S2       │
│              │              │              │                     │
│  Funcional   │  Falta algo  │  Hay daño    │  Efecto débil       │
│  (sin        │  Completar   │  Neutralizar │  Intensificar       │
│  problema)   │  el modelo   │  el daño     │  la interacción     │
└──────────────┴──────────────┴──────────────┴─────────────────────┘
```

> Para la notación textual completa, ver: [Notación y diagramas Su-Campo](04-notacion-diagramas.md)

---

## Modelo 1: Completo y funcional

### Diagrama

```
        F
       / \
      /   \
     / → → \         S2 actúa sobre S1 a través del campo F.
    /       \         La interacción es adecuada.
  S1 ─────── S2      No hay problema Su-Campo.
```

### Descripción

Los tres elementos (S1, S2, F) están presentes y la interacción entre ellos produce el efecto deseado de forma satisfactoria. El sistema cumple su función principal sin deficiencias ni efectos dañinos relevantes.

### Qué necesita ocurrir

Nada desde el punto de vista Su-Campo. Si hay un problema en el sistema, no es un problema de modelo Su-Campo o debe reformularse identificando otra interacción dentro del sistema que sí sea deficiente.

### Ejemplo

**Sistema**: un imán (S2) sujeta una placa de acero (S1) mediante campo magnético (F_mag).

```
      F_mag
       / \
      /   \
     / → → \
    /       \
  S1 ─────── S2
 (placa     (imán)
  de acero)
```

La placa queda firmemente sujeta. No hay insuficiencia ni daño. El modelo está completo y funcional.

---

## Modelo 2: Incompleto

### Diagrama

```
Caso A: Falta S2                  Caso B: Falta F

     (F?)                              (F?)
       \                              /    \
        \                            /      \
         \                          /        \
  S1      (S2?)                   S1 ──────── S2

  Existe el objeto S1,            Existen S1 y S2 pero
  pero no hay herramienta         no hay interacción
  ni campo definido.              (campo) entre ellas.
```

### Descripción

Al modelo le falta uno o más elementos. Los casos más frecuentes son:

- **Falta S2**: se necesita realizar una acción sobre S1, pero no existe una herramienta identificada que ejecute la acción.
- **Falta F**: existen S1 y S2, pero no hay un campo (energía/interacción) que conecte a la herramienta con el objeto.
- **Falta S2 y F**: solo existe el objeto S1 y la necesidad funcional; todo lo demás debe introducirse.

Un modelo incompleto no es un sistema que funciona mal; es un sistema que **no funciona en absoluto** respecto a la función analizada.

### Qué necesita ocurrir

**Completar el modelo** añadiendo el elemento o elementos faltantes para formar un triángulo Su-Campo funcional.

### Ejemplo

**Problema**: "Necesitamos detectar microfisuras internas en piezas de cerámica, pero actualmente no tenemos forma de hacerlo."

```
Modelo actual (incompleto):

  S1 = pieza de cerámica con microfisuras
  S2 = ¿?
  F  = ¿?

Solo existe S1 (el objeto). Falta la herramienta y el campo.
```

**Solución** (completar el modelo): introducir un transductor ultrasónico (S2) y campo mecánico de ultrasonidos (F_mec), que se propagan por S1 y se reflejan en las fisuras.

```
Modelo completado:

      F_mec (ultrasonidos)
       / \
      /   \
     / → → \
    /       \
  S1 ─────── S2
 (cerámica)  (transductor ultrasónico)
```

### Dirección: Soluciones Estándar

→ **Clase 1**: Construcción y destrucción de modelos Su-Campo (especialmente subclase 1.1: Síntesis de modelos Su-Campo).

> Ver: [76 Soluciones Estándar — Clase 1](../06-soluciones-estandar/00-indice-soluciones.md)

---

## Modelo 3: Completo con interacción dañina

### Diagrama

```
        F
       /↯\
      / ↯  \
     / ↯  ↯ \       S2 actúa sobre S1 a través de F,
    /  ↯  ↯   \     pero la interacción produce un
  S1 ←←↯↯←←── S2    EFECTO DAÑINO sobre S1.
```

Notación alternativa más sencilla:

```
        F
       / \
      /   \
     / ⤳⤳⤳ \        ⤳ = interacción dañina
    /       \
  S1 ─────── S2
```

### Descripción

Los tres elementos están presentes, pero el campo F produce un **efecto no deseado** (dañino, perjudicial) sobre S1 además de, o en lugar de, el efecto útil. Los casos típicos son:

- F produce un efecto útil **y** un efecto dañino simultáneamente.
- F produce **solo** un efecto dañino (la acción es enteramente nociva).
- La interacción entre S1 y S2 genera un efecto secundario no deseado.

### Qué necesita ocurrir

**Neutralizar o eliminar la interacción dañina** sin perder la función útil del sistema. Las estrategias típicas incluyen:

- Introducir una sustancia intermedia S3 que absorba o bloquee el efecto dañino.
- Introducir un campo compensatorio F2 que contrarreste F.
- Modificar S1 o S2 para que sean menos susceptibles al daño.

### Ejemplo

**Problema**: "La soldadura por arco (S2) une piezas metálicas (S1) mediante calor (F_term), pero el calor excesivo deforma la pieza."

```
      F_term (calor)
       /↯\
      / ↯  \
     / ↯  ↯ \       El calor une las piezas (útil)
    /  ↯  ↯   \     PERO también las deforma (dañino).
  S1 ←←↯↯←←── S2
 (pieza       (arco de
  metálica)    soldadura)
```

**Solución** (introducir S3): añadir un disipador de calor (S3) adyacente a la zona de soldadura que absorba el exceso térmico.

```
      F_term
       / \
      /   \
     / → → \
    /       \
  S1 ─── S3 ─── S2
 (pieza) (disipador) (arco)

 S3 absorbe el calor excedente,
 protegiendo a S1 de la deformación.
```

### Dirección: Soluciones Estándar

→ **Clase 1**: Construcción y destrucción de modelos Su-Campo (especialmente subclase 1.2: Destrucción de modelos Su-Campo).

> Ver: [76 Soluciones Estándar — Clase 1](../06-soluciones-estandar/00-indice-soluciones.md)

---

## Modelo 4: Completo con interacción insuficiente

### Diagrama

```
        F
       / \
      /   \
     / ~~> \         S2 actúa sobre S1 a través de F,
    /       \        pero el efecto es INSUFICIENTE
  S1 ─────── S2      (demasiado débil, lento, impreciso).
```

### Descripción

Los tres elementos están presentes y la interacción no es dañina, pero el **efecto producido es insuficiente**: demasiado débil, demasiado lento, impreciso, incompleto o inestable. El sistema funciona, pero no al nivel requerido.

### Qué necesita ocurrir

**Intensificar o mejorar la interacción** existente. Las estrategias típicas incluyen:

- Modificar S2 (mejorar la herramienta, hacerla más efectiva).
- Cambiar F (usar un campo más potente o de otro tipo).
- Introducir S3 (sustancia intermedia que potencie la interacción).
- Introducir F2 (campo adicional que refuerce al primero).
- Cambiar el modelo a un sistema bi- o poli-modelo (encadenar, duplicar).

### Ejemplo

**Problema**: "El mezclador mecánico (S2) agita el líquido viscoso (S1) con campo mecánico (F_mec), pero la mezcla queda heterogénea."

```
      F_mec
       / \
      /   \
     / ~~> \         La agitación mecánica es
    /       \        INSUFICIENTE para homogeneizar
  S1 ─────── S2      el líquido viscoso.
 (líquido   (mezclador)
  viscoso)
```

**Solución** (cambiar F): reemplazar o complementar el campo mecánico con campo ultrasónico (F_mec_ultra), que genera cavitación y mezcla a nivel microscópico.

```
      F_mec + F_mec_ultra
       / \
      /   \
     / → → \         Ahora la combinación de campos
    /       \        logra una mezcla homogénea.
  S1 ─────── S2'
 (líquido   (mezclador con
  viscoso)   ultrasonido)
```

### Dirección: Soluciones Estándar

→ **Clase 2**: Evolución de modelos Su-Campo (especialmente subclases 2.1 a 2.4 para intensificación).

> Ver: [76 Soluciones Estándar — Clase 2](../06-soluciones-estandar/00-indice-soluciones.md)

---

## Tabla de decisión: Modelo → Clase de Soluciones Estándar

La siguiente tabla resume la relación directa entre el tipo de modelo diagnosticado y la clase de Soluciones Estándar que debe consultarse:

| Tipo de modelo | Diagnóstico | Clase de Solución Estándar | Estrategia general |
|----------------|-------------|----------------------------|-------------------|
| **Incompleto** | Falta S2 y/o F | **Clase 1.1**: Síntesis de modelos Su-Campo | Completar el modelo añadiendo los elementos faltantes |
| **Dañino** | F causa daño a S1 | **Clase 1.2**: Destrucción de modelos Su-Campo dañinos | Introducir S3, F2, o modificar S1/S2 para neutralizar |
| **Insuficiente** | F es débil | **Clase 2**: Evolución de modelos Su-Campo | Mejorar S2, cambiar F, añadir S3 o F2, encadenar modelos |
| **Completo (pero se necesita medición)** | Falta detección/medición | **Clase 4**: Detección y medición | Construir un modelo Su-Campo de detección |
| **Cualquiera (se necesita simplificar)** | Sistema excesivamente complejo | **Clase 5**: Normas de simplificación | Reducir elementos, usar recursos existentes |

### Clase 3: Transición a supersistema

La **Clase 3** de las Soluciones Estándar no corresponde a un tipo de modelo específico, sino a una **dirección evolutiva general**: la transición de un sistema individual a un **bi-sistema** o **poli-sistema**. Se aplica cuando las clases 1 y 2 han agotado sus posibilidades dentro del sistema actual.

> Ver: [76 Soluciones Estándar](../06-soluciones-estandar/00-indice-soluciones.md)

## Flujo de diagnóstico Su-Campo

El siguiente diagrama muestra el proceso de diagnóstico paso a paso:

```
                    ¿El modelo tiene S1, S2 y F?
                              │
                     ┌────────┴────────┐
                     │ NO              │ SÍ
                     ▼                 ▼
              MODELO INCOMPLETO    ¿La interacción F
              → Clase 1.1          es dañina?
              (completar)                │
                              ┌─────────┴─────────┐
                              │ SÍ                │ NO
                              ▼                   ▼
                       MODELO DAÑINO        ¿La interacción F
                       → Clase 1.2          es suficiente?
                       (neutralizar)              │
                                         ┌────────┴────────┐
                                         │ NO              │ SÍ
                                         ▼                 ▼
                                   MODELO               MODELO
                                   INSUFICIENTE         COMPLETO
                                   → Clase 2            (sin problema
                                   (intensificar)        Su-Campo)
```

## Múltiples modelos en un sistema

Un sistema técnico real rara vez contiene un solo modelo Su-Campo. La mayoría de los sistemas pueden descomponerse en **múltiples modelos** que representan diferentes funciones o interacciones:

```
Ejemplo: Sistema de pintura electrostática

Modelo 1 (carga):           Modelo 2 (transporte):     Modelo 3 (deposición):

    F_elec                      F_mec (aire)              F_elec
     / \                         / \                       / \
    /   \                       /   \                     /   \
  S1a    S2a                  S1b    S2b                S1c    S2c
(pintura)(electrodo)         (gotas) (compresor)       (gotas)(pieza a
                                                        cargadas) pintar)
```

Cuando un sistema presenta problemas, es fundamental **identificar cuál de los modelos** dentro del sistema es el deficiente y aplicar el análisis a ese modelo específico.

## Ejemplo integrador: diagnóstico completo

**Problema**: "En una imprenta offset, la tinta (S2) se transfiere al papel (S1) mediante presión mecánica (F_mec) a través de un rodillo. La impresión es buena en general, pero en zonas de alta cobertura la tinta traspasa al reverso del papel (efecto *show-through*)."

**Análisis**:

1. **Función útil**: transferir tinta al papel → modelo completo y funcional.
2. **Efecto dañino**: la tinta traspasa al reverso → modelo dañino superpuesto.

```
Modelo funcional (útil):          Modelo dañino (superpuesto):

    F_mec                              F_mec
     / \                                /↯\
    /   \                              / ↯  \
   / → → \                           /  ↯    \
  S1      S2                        S1_reverso  S2 (tinta)
 (papel   (tinta)                  (cara posterior
  cara                              del papel)
  frontal)
```

**Diagnóstico**: modelo con **interacción dañina** → Clase 1.2.

**Direcciones de solución**:

- Introducir S3: capa barrera en el papel (tratamiento superficial).
- Modificar S2: tinta de mayor viscosidad o secado rápido.
- Modificar F: reducir presión en zonas de alta cobertura (control variable).

> Ver: [Reglas de transformación](03-transformaciones.md)

---

**Navegación**: [← Fundamentos Su-Campo](01-fundamentos-su-campo.md) · [Transformaciones →](03-transformaciones.md)
