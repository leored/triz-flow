# Clase 1: Construir y destruir modelos Su-Campo

## Visión general

La Clase 1 contiene **13 soluciones estándar** que abordan los dos problemas fundamentales de los modelos Su-Campo:

- **Subgrupo 1.1**: El modelo Su-Campo está **incompleto** (le falta algún componente) y debe completarse para que funcione.
- **Subgrupo 1.2**: El modelo Su-Campo está **completo pero produce un efecto dañino** que debe eliminarse o neutralizarse.

Estas soluciones son el punto de partida natural cuando el [Análisis Su-Campo](../05-analisis-su-campo/04-notacion-diagramas.md) revela un modelo incompleto o una interacción no deseada.

---

## 1.1 Construcción de modelos Su-Campo

### 1.1.1 Completar modelo Su-Campo incompleto

**Principio**: Si un sistema es incompleto (le falta una sustancia, un campo o ambos), completar el modelo Su-Campo añadiendo los elementos faltantes.

**Diagrama**:
```
ANTES:             DESPUÉS:
  S1                S1 ←--F--→ S2
  (sin interacción)   (modelo completo)
```

**Ejemplo**: Para mezclar dos líquidos inmiscibles (S1) que no interactúan, se introduce un agitador mecánico (S2) accionado por un campo mecánico (F_mec). Ahora el modelo Su-Campo está completo y la mezcla ocurre.

---

### 1.1.2 Añadir sustancia interna S3

**Principio**: Si no se pueden modificar directamente S1 ni S2, introducir una tercera sustancia S3 como modificación interna de una de las sustancias existentes.

**Diagrama**:
```
ANTES:              DESPUÉS:
  S1 ←-F-→ S2        S1 ←-F-→ [S2 + S3]
  (insuficiente)       (S3 modifica S2 internamente)
```

**Ejemplo**: Un cuchillo (S2) no corta bien un material blando (S1). Se introduce un recubrimiento antiadherente (S3) en la hoja del cuchillo para modificar la interacción de corte, permitiendo que la hoja deslice sin deformar el material.

---

### 1.1.3 Añadir sustancia externa S3

**Principio**: Si no se pueden modificar S1 ni S2, introducir una tercera sustancia S3 desde el exterior del sistema que actúe como mediadora.

**Diagrama**:
```
ANTES:              DESPUÉS:
  S1 ←-F-→ S2        S1 ←-F-→ S3 ←-F-→ S2
  (insuficiente)       (S3 media desde fuera)
```

**Ejemplo**: Una broca (S2) desgasta el material duro (S1) con excesiva fricción. Se añade un lubricante de corte externo (S3) que actúa como intermediario, reduciendo la fricción y mejorando el mecanizado.

---

### 1.1.4 Usar recurso del entorno como S3

**Principio**: Cuando no se puede añadir una sustancia nueva, emplear una sustancia que ya exista en el entorno del sistema como mediadora.

**Diagrama**:
```
ANTES:              DESPUÉS:
  S1 ←-F-→ S2        S1 ←-F-→ S_entorno ←-F-→ S2
  (insuficiente)       (sustancia del entorno como S3)
```

**Ejemplo**: Para transportar piezas delicadas (S1) sin dañarlas con una cinta transportadora (S2), se usa el aire del entorno (S_entorno) como colchón neumático entre la pieza y la cinta.

---

### 1.1.5 Usar recurso del entorno como F

**Principio**: Emplear un campo que ya esté disponible en el entorno en lugar de generar uno artificialmente.

**Diagrama**:
```
ANTES:              DESPUÉS:
  S1 ... S2          S1 ←-F_entorno-→ S2
  (falta campo)       (campo del entorno completa el modelo)
```

**Ejemplo**: Para secar piezas pintadas (S1), en lugar de instalar un horno (generar F_térmico artificialmente), se usan la radiación solar y el viento del entorno como fuente de campo térmico y mecánico.

---

### 1.1.6 Cantidad mínima de aditivo

**Principio**: Cuando hay restricciones para introducir grandes cantidades de sustancia, introducir una cantidad mínima de una sustancia muy activa.

**Diagrama**:
```
ANTES:              DESPUÉS:
  S1 ←-F-→ S2        S1 ←-F-→ [S2 + trazas de S3*]
  (insuficiente)       (S3* = sustancia muy activa, trazas)
```

**Ejemplo**: Para mejorar la conductividad de un polímero (S1), en lugar de cargarlo masivamente con metal, se añaden trazas de nanotubos de carbono (S3*) que crean una red conductora con mínima cantidad.

---

### 1.1.7 Cantidad máxima de aditivo temporal

**Principio**: Introducir temporalmente una gran cantidad de S3 durante la operación, y eliminarla después.

**Diagrama**:
```
ANTES:              DURANTE:             DESPUÉS:
  S1 ←-F-→ S2        S1 ←-F-→ [S2+S3]    S1 ←-F-→ S2
  (insuficiente)       (S3 masivo temporal)   (S3 retirada)
```

**Ejemplo**: Para mecanizar una pieza delgada (S1) que vibra, se rellena temporalmente con hielo (S3) que da rigidez durante el fresado. Al terminar, el hielo se derrite y se retira.

---

### 1.1.8 Modelo Su-Campo con F y S selectivos

**Principio**: Construir el campo y las sustancias de modo que la interacción actúe selectivamente solo sobre la zona o elemento deseado.

**Diagrama**:
```
ANTES:              DESPUÉS:
  S1 ←-F-→ S2        S1_zona ←-F_selectivo-→ S2
  (acción difusa)      (acción focalizada)
```

**Ejemplo**: Para calentar solo una zona específica de una pieza metálica (S1), se usa calentamiento por inducción (F_electromagnético selectivo) con una bobina conformada al perfil de la zona deseada, en lugar de meter toda la pieza en un horno.

---

## 1.2 Destrucción de modelos Su-Campo

Las soluciones de este subgrupo se aplican cuando el modelo Su-Campo está completo pero la interacción entre las sustancias es **dañina** o **no deseada**.

### 1.2.1 Introducir S3 entre S1 y S2

**Principio**: Eliminar o reducir la interacción dañina insertando una tercera sustancia S3 entre S1 y S2 que actúe como barrera o amortiguador.

**Diagrama**:
```
ANTES:                DESPUÉS:
  S1 ←~~F_daño~~→ S2    S1 ←-F-→ [S3] ←-F-→ S2
  (interacción dañina)    (S3 bloquea/amortigua)
```

**Ejemplo**: Un ácido (S2) corroe un tanque metálico (S1). Se introduce un revestimiento de polímero (S3) en las paredes internas del tanque que actúa como barrera entre el ácido y el metal.

---

### 1.2.2 Modificar S1 con aditivo

**Principio**: Alterar la sustancia S1 (el objeto) internamente añadiendo un aditivo que la haga resistente al efecto dañino de F.

**Diagrama**:
```
ANTES:                DESPUÉS:
  S1 ←~~F_daño~~→ S2    [S1+S3] ←-F-→ S2
  (S1 dañado por F)       (S1 modificado resiste F)
```

**Ejemplo**: Una tubería de acero (S1) se corroe por el agua salada (S2, F_químico). Se modifica S1 aleándola con cromo y níquel (S3), convirtiéndola en acero inoxidable que resiste la corrosión.

---

### 1.2.3 Modificar S2 con aditivo

**Principio**: Alterar la sustancia S2 (la herramienta o el agente dañino) añadiendo un aditivo que reduzca su efecto nocivo.

**Diagrama**:
```
ANTES:                DESPUÉS:
  S1 ←~~F_daño~~→ S2    S1 ←-F-→ [S2+S3]
  (S2 causa daño)         (S2 modificado, menos dañino)
```

**Ejemplo**: Un detergente (S2) daña los tejidos delicados (S1). Se añade un suavizante (S3) al detergente que modifica su acción química, reduciendo la agresividad sobre las fibras.

---

### 1.2.4 Contrarrestar con F2

**Principio**: Introducir un segundo campo F2 que contrarreste el efecto dañino de F1, neutralizando la interacción no deseada.

**Diagrama**:
```
ANTES:                DESPUÉS:
  S1 ←~~F1_daño~~→ S2    S1 ←~~F1~~→ S2
  (efecto dañino de F1)        ←--F2--→
                           (F2 contrarresta F1)
```

**Ejemplo**: La vibración mecánica (F1_mec) de un motor (S2) daña los instrumentos sensibles (S1) montados cerca. Se introducen amortiguadores activos que generan vibraciones en contrafase (F2_mec), neutralizando la vibración original (cancelación activa de vibraciones).

---

### 1.2.5 Desconectar F mediante campo magnético

**Principio**: Eliminar la interacción dañina sustituyendo alguna sustancia por partículas ferromagnéticas controladas por un campo magnético, lo que permite "desconectar" la interacción cuando sea necesario.

**Diagrama**:
```
ANTES:                DESPUÉS:
  S1 ←~~F_daño~~→ S2    S1 ←-F_mag-→ S2_ferro
  (no controlable)        (controlable on/off con F_mag)
```

**Ejemplo**: Un freno mecánico (S2) causa desgaste por fricción (F_daño) en un eje (S1). Se sustituye por un freno de polvo magnético: partículas ferromagnéticas (S2_ferro) que solo generan fricción cuando se activa un campo magnético (F_mag), eliminando el desgaste en reposo.

---

## Guía rápida de selección — Clase 1

```
¿Su modelo Su-Campo está completo?
  │
  ├── NO (incompleto) ──→ Subgrupo 1.1 (Construcción)
  │     ├── ¿Puede añadir S o F directamente? → 1.1.1
  │     ├── ¿Puede modificar S2 internamente?  → 1.1.2
  │     ├── ¿Puede añadir S3 externa?          → 1.1.3
  │     ├── ¿Hay sustancia útil en el entorno? → 1.1.4
  │     ├── ¿Hay campo útil en el entorno?     → 1.1.5
  │     ├── ¿Restricción de cantidad?          → 1.1.6 o 1.1.7
  │     └── ¿Necesita acción selectiva?        → 1.1.8
  │
  └── SÍ (pero la interacción es dañina) ──→ Subgrupo 1.2 (Destrucción)
        ├── ¿Puede insertar S3 entre S1 y S2? → 1.2.1
        ├── ¿Puede modificar S1?               → 1.2.2
        ├── ¿Puede modificar S2?               → 1.2.3
        ├── ¿Puede añadir un contra-campo?     → 1.2.4
        └── ¿Puede usar control magnético?     → 1.2.5
```

---

## Relación con el Análisis Su-Campo

Las soluciones de la Clase 1 se corresponden directamente con las dos situaciones problemáticas básicas del [Análisis Su-Campo](../05-analisis-su-campo/04-notacion-diagramas.md):

- **Modelo incompleto** → aplicar soluciones 1.1.x para completarlo.
- **Modelo con efecto dañino** (representado con línea ondulada `~~~`) → aplicar soluciones 1.2.x para neutralizar o eliminar la interacción dañina.

En ambos casos, el objetivo es transformar el modelo Su-Campo problemático en uno funcional y eficaz.

---

**Navegación**: [← Índice](00-indice-soluciones.md) · [Clase 2 →](02-clase-2-desarrollar.md)
