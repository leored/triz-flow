# Reglas de Transformación Su-Campo

Las **reglas de transformación** son operaciones estándar que se aplican a los modelos Su-Campo para resolver los problemas diagnosticados (modelo incompleto, dañino o insuficiente). Estas reglas constituyen el puente entre el **diagnóstico** del modelo y las **76 Soluciones Estándar**.

> Prerrequisito: [Modelos básicos Su-Campo](02-modelos-basicos.md) · [Fundamentos Su-Campo](01-fundamentos-su-campo.md)

## Visión general de las siete reglas

| Regla | Nombre | Cuándo se aplica | Transformación |
|:-----:|--------|-------------------|---------------|
| 1 | Completar modelo incompleto | Falta S2 y/o F | Añadir los elementos faltantes |
| 2 | Modificar S2 | Interacción insuficiente o dañina | Cambiar propiedades de la herramienta |
| 3 | Modificar F | Insuficiente control o efectividad | Cambiar tipo de campo |
| 4 | Introducir S3 | Daño a S1, o insuficiencia | Interponer sustancia intermedia |
| 5 | Introducir F2 | Efecto dañino que debe neutralizarse | Añadir campo compensatorio |
| 6 | Encadenar modelos | Un solo modelo no resuelve | Conectar salida de un modelo con entrada de otro |
| 7 | Transición a bi/poli-sistema | Sistema individual agotado | Duplicar, combinar o heterogeneizar |

---

## Regla 1: Completar un modelo incompleto

### Principio

Si el modelo Su-Campo está incompleto (falta S2, F, o ambos), la solución es **añadir los elementos faltantes** para formar un triángulo Su-Campo funcional.

### Diagrama antes → después

```
ANTES (incompleto):                    DESPUÉS (completo):

  S1      (S2?)      (F?)                    F
                                            / \
  Solo existe el objeto.                   /   \
  No hay herramienta ni campo.            / → → \
                                         /       \
                                       S1 ─────── S2

                                       Se introducen S2 y F.
```

```
ANTES (falta F):                       DESPUÉS (completo):

  S1 ─────── S2      (F?)                    F
                                            / \
  Existen sustancias pero                  /   \
  no hay campo que las conecte.           / → → \
                                         /       \
                                       S1 ─────── S2

                                       Se introduce F.
```

### Explicación

Esta es la regla más fundamental. Muchos problemas técnicos se reducen a la ausencia de un mecanismo de acción. La clave es seleccionar el campo F y la herramienta S2 más apropiados según los recursos disponibles y los requisitos del sistema.

La selección del campo F debe considerar la **jerarquía de controlabilidad**:

```
Gravitacional → Mecánico → Térmico → Químico → Eléctrico → Magnético → Electromagnético
                                                            ↑
                                                     Preferir campos
                                                     más controlables
```

### Ejemplo

**Problema**: detectar fugas microscópicas en tuberías de gas.

- S1 = tubería con posible fuga.
- S2 = ¿? (no hay herramienta de detección).
- F = ¿?

**Solución**: introducir un gas trazador con compuesto fluorescente (S2) y una lámpara UV (F_em) que haga visible la fuga.

```
ANTES:                          DESPUÉS:

  S1 (tubería)                      F_em (luz UV)
                                     / \
  Sin forma de detectar             /   \
  la fuga.                         / → → \
                                  /       \
                                S1 ─────── S2
                               (tubería)  (gas trazador
                                           fluorescente)
```

### Soluciones Estándar asociadas

→ Clase 1.1 (Soluciones 1.1.1 a 1.1.8)

---

## Regla 2: Modificar S2 (sustancia-herramienta)

### Principio

Cuando la interacción es insuficiente o produce efectos no deseados, **modificar las propiedades de S2** puede mejorar o corregir la acción sobre S1, sin cambiar el tipo de campo ni la estructura general del modelo.

### Diagrama antes → después

```
ANTES (insuficiente):                  DESPUÉS (mejorado):

        F                                    F
       / \                                  / \
      /   \                                /   \
     / ~~> \                              / → → \
    /       \                            /       \
  S1 ─────── S2                        S1 ─────── S2'
             (herramienta               (herramienta
              original)                  MODIFICADA)
```

### Explicación

Las modificaciones típicas de S2 incluyen:

| Modificación de S2 | Descripción | Ejemplo |
|-------------------|-------------|---------|
| **Cambiar material** | Usar otro material con mejores propiedades | Cambiar abrasivo de alúmina por diamante |
| **Cambiar estructura** | Alterar la geometría, porosidad, rugosidad | Rodillo liso → rodillo texturizado |
| **Cambiar estado** | Sólido → líquido → gas → plasma | Herramienta sólida → chorro de agua |
| **Segmentar** | Dividir S2 en partes más pequeñas | Un cuchillo → múltiples microcuchillas (láser) |
| **Hacer porosa** | Introducir cavidades en S2 | Muela abrasiva compacta → muela porosa |
| **Añadir aditivos** | Incorporar partículas, fibras, etc. | Polímero puro → polímero con fibra de carbono |
| **Usar campos internos** | S2 genera su propio campo | Herramienta magnetizada, cargada, calentada |

### Ejemplo

**Problema**: una broca estándar (S2) perfora chapa metálica (S1) con campo mecánico (F_mec), pero se desgasta rápidamente.

```
ANTES:                                 DESPUÉS:

      F_mec                                 F_mec
       / \                                  / \
      /   \                                /   \
     / ~~> \                              / → → \
    /       \                            /       \
  S1 ─────── S2                        S1 ─────── S2'
 (chapa)    (broca HSS)              (chapa)    (broca con
                                                 recubrimiento
                                                 de TiN)
```

La broca modificada (S2') con recubrimiento de nitruro de titanio tiene mayor dureza superficial y menor fricción, resolviendo el desgaste prematuro.

### Soluciones Estándar asociadas

→ Clase 2.2 (Evolución por modificación de S2)

---

## Regla 3: Modificar F (cambiar tipo de campo)

### Principio

Cuando el campo actual no proporciona el control, la precisión o la efectividad requeridos, **sustituir o complementar el campo F por otro tipo de campo** más adecuado.

### Diagrama antes → después

```
ANTES (campo inadecuado):              DESPUÉS (campo nuevo):

        F                                   F'
       / \                                  / \
      /   \                                /   \
     / ~~> \                              / → → \
    /       \                            /       \
  S1 ─────── S2                        S1 ─────── S2
              (misma herramienta)                 (puede necesitar
                                                   adaptación)
```

### Explicación

El cambio de campo sigue generalmente la tendencia evolutiva hacia campos más controlables:

```
F_grav ───→ F_mec ───→ F_term ───→ F_quim ───→ F_elec ───→ F_mag ───→ F_em
  │           │           │           │           │           │          │
  │     Vibración,   Calenta-    Reacciones  Electro-    Campos    Láser,
  │     presión,     miento,     químicas,   deposición, magnéticos, microondas,
  │     ultrasonido  enfriamiento catálisis   electro-    sujeción,  óptica
  │                                           foresis     separación
  │
Gravedad
(mínimo control)                                           (máximo control)
```

Las razones para cambiar el campo incluyen:

- **Mayor controlabilidad**: un campo electromagnético se enciende/apaga instantáneamente; uno gravitacional no.
- **Mayor selectividad**: un campo magnético solo afecta a materiales ferromagnéticos.
- **Mayor penetración**: ultrasonidos o rayos X penetran donde la luz visible no puede.
- **Menor daño colateral**: un campo químico puede ser más localizado que uno térmico.

### Ejemplo

**Problema**: la pintura líquida (S2) se aplica sobre carrocerías (S1) por gravedad y presión de aire (F_mec), pero la cobertura es irregular y hay desperdicio por sobrepulverización.

```
ANTES:                                 DESPUÉS:

      F_mec (aire)                         F_elec (electrostático)
       / \                                  / \
      /   \                                /   \
     / ~~> \                              / → → \
    /       \                            /       \
  S1 ─────── S2                        S1 ─────── S2
 (carrocería)(pintura)                (carrocería)(pintura
                                       conectada   cargada
                                       a tierra)   eléctricamente)
```

Al cambiar de campo mecánico a campo eléctrico (pintura electrostática), las partículas cargadas son atraídas hacia la superficie conectada a tierra, logrando cobertura uniforme y reduciendo el desperdicio al mínimo.

### Soluciones Estándar asociadas

→ Clase 2.3 (Evolución por cambio de campo) · Clase 2.4 (Transición a campos forzados)

---

## Regla 4: Introducir S3 (tercera sustancia como intermediaria)

### Principio

Cuando la interacción directa entre S2 y S1 causa daño, o cuando la interacción es insuficiente, se puede **interponer una tercera sustancia S3** entre S2 y S1 (o adjunta a S1) que modifique la interacción.

### Diagrama antes → después

```
ANTES (dañino):                        DESPUÉS (protegido):

        F                                    F
       /↯\                                  / \
      / ↯  \                               /   \
     / ↯  ↯ \                             / → → \
    /       \                            /    │    \
  S1 ─────── S2                        S1 ── S3 ── S2

                                       S3 interpuesta entre S1 y S2
                                       bloquea o absorbe el efecto dañino.
```

```
ANTES (insuficiente):                  DESPUÉS (potenciado):

        F                                    F
       / \                                  / \
      /   \                                /   \
     / ~~> \                              / → → \
    /       \                            /    │    \
  S1 ─────── S2                        S1 ── S3 ── S2

                                       S3 amplifica o mejora la
                                       transmisión de la interacción.
```

### Explicación

S3 puede actuar de diversas formas:

| Función de S3 | Descripción | Ejemplo |
|---------------|-------------|---------|
| **Barrera protectora** | Bloquea la componente dañina de F | Recubrimiento anticorrosión entre metal y ambiente |
| **Amplificador** | Mejora la transmisión de F | Gel conductor en ecografías (mejora transmisión ultrasónica) |
| **Convertidor** | Transforma un tipo de acción en otro | Piezoeléctrico: convierte presión mecánica en señal eléctrica |
| **Amortiguador** | Reduce la intensidad de F a nivel aceptable | Amortiguador entre motor y chasis (reduce vibración) |
| **Mediador sacrificial** | Se consume en lugar de S1 | Ánodo de sacrificio (zinc) protege al hierro de la corrosión |

### Regla de selección de S3

Siguiendo el principio de recursos de TRIZ, S3 se busca en este orden:

1. **Modificación de S1** (S3 es una versión transformada de la propia S1).
2. **Modificación de S2** (S3 es un derivado de S2).
3. **Sustancia del entorno** (aire, agua, residuos del proceso).
4. **Sustancia nueva** (solo como último recurso).

> Ver: [Recursos en TRIZ](../00-fundamentos/03-conceptos-clave.md)

### Ejemplo

**Problema**: al mecanizar aluminio (S1) con herramienta de corte (S2) mediante campo mecánico (F_mec), el aluminio se adhiere a la herramienta (efecto dañino de soldadura en frío).

```
ANTES (dañino):                        DESPUÉS (protegido):

      F_mec                                 F_mec
       /↯\                                  / \
      / ↯  \                               /   \
     / ↯  ↯ \                             / → → \
    /       \                            /    │    \
  S1 ─────── S2                        S1 ── S3 ── S2
 (aluminio)  (herramienta)            (Al)  (fluido (herramienta)
                                             de corte)

                                       S3 = fluido de corte lubricante
                                       que impide la soldadura en frío.
```

### Soluciones Estándar asociadas

→ Clase 1.2 (Destrucción de modelos dañinos: 1.2.1 a 1.2.5) · Clase 2.1 (Evolución con introducción de sustancia)

---

## Regla 5: Introducir F2 (segundo campo compensatorio)

### Principio

Cuando F produce un efecto dañino que no puede eliminarse modificando S2 o introduciendo S3, se introduce un **segundo campo F2** que **contrarreste** el efecto dañino de F sin interferir con su efecto útil.

### Diagrama antes → después

```
ANTES (dañino):                        DESPUÉS (compensado):

        F                                  F         F2
       /↯\                               / \       / \
      / ↯  \                             / → \     / → \
     / ↯  ↯ \                          /     \   /     \
    /       \                         S1 ───── S2      S1
  S1 ─────── S2
                                       F  produce el efecto útil.
  F causa daño                         F2 contrarresta el efecto dañino.
  a S1.                                Ambos actúan sobre S1 simultáneamente.
```

Representación simplificada:

```
ANTES:          DESPUÉS:

  F                F ──→ S1 ←── F2
 /↯\                (útil)  (compensatorio)
S1  S2               │         │
                     S2        (fuente de F2)
```

### Explicación

Esta regla se basa en el principio TRIZ de **compensación**: en lugar de eliminar un efecto dañino (que puede ser inherente al proceso), se introduce una acción opuesta que lo neutralice.

Ejemplos de pares campo-contracampo:

| Campo dañino (F) | Campo compensatorio (F2) | Ejemplo |
|-------------------|--------------------------|---------|
| F_term (calor excesivo) | F_term (enfriamiento forzado) | Refrigeración por agua en soldadura |
| F_mec (vibración) | F_mec (antivibración) | Amortiguadores activos |
| F_elec (carga estática) | F_elec (ionización) | Barras ionizadoras en impresión |
| F_quim (oxidación) | F_quim (reducción) | Atmósfera inerte (argón) en soldadura |
| F_mec (deformación) | F_mec (compresión previa) | Granallado (*shot peening*) antes de mecanizar |

### Ejemplo

**Problema**: el tratamiento térmico (F_term) de piezas de acero (S1) en un horno (S2) las endurece (efecto útil), pero la superficie se oxida (efecto dañino del campo térmico en presencia de oxígeno).

```
ANTES (dañino):                        DESPUÉS (compensado):

      F_term                              F_term     F_quim
       /↯\                                / \        / \
      / ↯  \                              / → \      / → \
     / ↯  ↯ \                            /     \    /     \
    /       \                           S1 ──── S2  S1 ─── S3
  S1 ─────── S2                        (acero) (horno)(acero)(gas
 (acero)    (horno)                                         argón)

  El calor endurece                    F_term endurece (útil).
  PERO también oxida.                  F_quim: atmósfera inerte (argón)
                                       IMPIDE la oxidación.
```

### Soluciones Estándar asociadas

→ Clase 1.2 (Destrucción de modelos dañinos: uso de contracampo)

---

## Regla 6: Encadenar modelos Su-Campo

### Principio

Cuando un solo modelo Su-Campo no puede resolver el problema completo, se **encadenan** dos o más modelos en secuencia: la **salida** (resultado) de un modelo se convierte en la **entrada** (S1) del siguiente.

### Diagrama antes → después

```
ANTES (un solo modelo insuficiente):

        F
       / \
      /   \
     / ~~> \         Un solo modelo no logra
    /       \        el resultado final deseado.
  S1 ─────── S2


DESPUÉS (cadena de modelos):

        F1                    F2
       / \                   / \
      /   \                 /   \
     / → → \               / → → \
    /       \             /       \
  S1 ─────── S2    →   S1' ─────── S3

  Modelo 1:              Modelo 2:
  S2 actúa sobre S1      S3 actúa sobre S1'
  mediante F1,            (que es S1 transformada
  produciendo S1'         por el Modelo 1)
  (S1 parcialmente        mediante F2 para
  transformada).          completar el resultado.
```

### Explicación

El encadenamiento es útil cuando:

- Una sola transformación no basta para lograr el resultado deseado.
- El proceso requiere **etapas secuenciales** con diferentes campos o herramientas.
- Cada etapa prepara al objeto S1 para la siguiente.

El encadenamiento puede ser:

| Tipo de cadena | Descripción |
|---------------|-------------|
| **Secuencial** | Modelo 1 → Modelo 2 → Modelo 3 (lineal) |
| **Paralela** | Varios modelos actúan simultáneamente sobre S1 |
| **Con retroalimentación** | La salida de un modelo modifica la entrada de un modelo anterior |

### Ejemplo

**Problema**: imprimir texto sobre una superficie de vidrio (S1) que sea permanente y resistente al desgaste. Un solo proceso no lo logra: la tinta directa no adhiere bien al vidrio.

```
Modelo 1 (preparación):          Modelo 2 (impresión):

    F_quim (tratamiento)              F_term (horneado)
     / \                               / \
    /   \                             /   \
   / → → \                          / → → \
  /       \                        /       \
S1 ─────── S2             →     S1' ─────── S3
(vidrio)  (solución de          (vidrio     (esmalte
           activación            tratado)    cerámico)
           superficial)

Paso 1: Tratamiento químico       Paso 2: Aplicar esmalte cerámico
activa la superficie del          y hornear. El esmalte se funde
vidrio para mejorar adhesión.     y se fusiona permanentemente al vidrio.
```

### Soluciones Estándar asociadas

→ Clase 2.1 (Encadenamiento de modelos Su-Campo)

---

## Regla 7: Transición a bi-sistema o poli-sistema

### Principio

Cuando las mejoras dentro de un sistema individual se agotan, se pasa a un **bi-sistema** (combinar dos sistemas iguales o diferentes) o a un **poli-sistema** (múltiples copias, versiones o variantes del sistema). Esta es una de las **leyes de evolución** de los sistemas técnicos.

### Diagrama antes → después

```
ANTES (sistema individual):

        F
       / \
      /   \
     / ~~> \         El sistema individual
    /       \        ha alcanzado su límite.
  S1 ─────── S2


DESPUÉS (bi-sistema homogéneo):

        F                  F
       / \                / \
      /   \              /   \
     / → → \            / → → \
    /       \          /       \
  S1a ────── S2a     S1b ────── S2b

  Dos sistemas iguales trabajan en conjunto,
  logrando un efecto que uno solo no puede.


DESPUÉS (bi-sistema heterogéneo):

        F1                 F2
       / \                / \
      /   \              /   \
     / → → \            / → → \
    /       \          /       \
  S1 ─────── S2a     S1 ─────── S2b

  Dos herramientas DIFERENTES actúan sobre el mismo S1,
  combinando ventajas de ambos enfoques.


DESPUÉS (poli-sistema):

    F       F       F       F
   / \     / \     / \     / \
  S1a-S2  S1b-S2  S1c-S2  S1d-S2  ...

  Múltiples copias del modelo trabajan en paralelo
  (p. ej., cabezal multi-husillo vs husillo único).
```

### Explicación

La transición sigue una tendencia evolutiva bien documentada en TRIZ:

```
Sistema          Bi-sistema        Bi-sistema          Poli-sistema     Sistema
individual  →    homogéneo    →    heterogéneo    →    complejo    →    de nivel
                 (dos iguales)     (dos diferentes)    (muchos)         superior

Ejemplo:
Un lápiz    →    Lápiz doble  →    Lápiz + goma  →    Set de 12    →   Procesador
                 (dos puntas)      (funciones            colores         de texto
                                    diferentes)                          (reemplaza
                                                                         al lápiz)
```

Las formas de crear bi-sistemas y poli-sistemas incluyen:

| Tipo | Descripción | Ejemplo |
|------|-------------|---------|
| **Duplicar S2** | Dos herramientas iguales | Motor bihélice (dos hélices iguales) |
| **Invertir S2** | Combinar S2 y anti-S2 | Navaja suiza: cuchilla + sierra |
| **Combinar S2 complementarios** | Dos herramientas de propiedades opuestas | Lápiz bicolor (rojo + azul) |
| **Duplicar F** | Dos campos iguales actuando | Calentamiento por ambas caras |
| **Combinar F diferentes** | Dos tipos de campo | Secado por convección + microondas |
| **Fragmentar S2** | Dividir S2 en muchas partes | Un chorro continuo → gotas (inkjet) |

### Ejemplo

**Problema**: un cuchillo de cocina (S2) corta alimentos (S1) con campo mecánico (F_mec), pero hay alimentos que no puede cortar bien (pan blando: lo aplasta; huesos: no tiene fuerza).

```
ANTES (sistema individual):

      F_mec
       / \
      / ~~> \
     /       \
  S1 ─────── S2 (cuchillo liso estándar)


DESPUÉS (bi-sistema heterogéneo → navaja de cocina con doble hoja):

      F_mec                F_mec
       / \                  / \
      / → → \              / → → \
     /       \            /       \
  S1_blando ── S2a     S1_duro ── S2b
              (hoja      (hoja
              serrada)    de hacha)

Solución: cuchillo con un lado liso y un lado serrado (o juego de cuchillos
especializados → poli-sistema heterogéneo).
```

### Soluciones Estándar asociadas

→ **Clase 3**: Transición a supersistema y a nivel micro (Soluciones 3.1.1 a 3.2.1)

> Ver: [Leyes de Evolución — Transición a supersistema](../08-leyes-evolucion/00-vision-general.md)

---

## Tabla resumen: cuándo aplicar cada regla

| Diagnóstico del modelo | Regla principal | Reglas complementarias |
|------------------------|:--------------:|----------------------|
| **Incompleto** (falta S2 y/o F) | **1** (completar) | 3 (seleccionar F óptimo) |
| **Dañino** (F causa daño a S1) | **4** (introducir S3) o **5** (introducir F2) | 2 (modificar S2) |
| **Insuficiente** (F demasiado débil) | **2** (modificar S2) o **3** (cambiar F) | 4 (S3 amplificador), 6 (encadenar), 7 (bi-sistema) |
| **Insuficiente tras intentar 2 y 3** | **6** (encadenar) o **7** (bi/poli-sistema) | — |
| **Sistema en límite evolutivo** | **7** (transición a bi/poli-sistema) | — |

## Flujo de aplicación de las reglas

```
         Modelo Su-Campo diagnosticado
                    │
        ┌───────────┼───────────┐
        ▼           ▼           ▼
   Incompleto    Dañino    Insuficiente
        │           │           │
        ▼           │           ▼
    Regla 1:        │       Regla 2: Modificar S2
    Completar       │       Regla 3: Cambiar F
        │           │           │
        │           │       ¿Resuelto?
        │           │       │       │
        │           │      SÍ      NO
        │           │       │       │
        │           ▼       │       ▼
        │     Regla 4: S3   │   Regla 4: S3 amplificador
        │     Regla 5: F2   │   Regla 6: Encadenar
        │           │       │   Regla 7: Bi/poli-sistema
        │           │       │       │
        ▼           ▼       ▼       ▼
              Modelo resuelto
                    │
                    ▼
         76 Soluciones Estándar
         (para implementación detallada)
```

> Ver: [76 Soluciones Estándar](../06-soluciones-estandar/00-indice-soluciones.md) · [ARIZ-85C](../07-ariz/00-que-es-ariz.md) (para problemas que resisten estas transformaciones)

---

**Navegación**: [← Modelos básicos](02-modelos-basicos.md) · [Notación y diagramas →](04-notacion-diagramas.md)
