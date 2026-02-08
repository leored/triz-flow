# Parte 1: Analisis del problema

> **Objetivo**: Transformar la situacion problematica inicial en un modelo del problema bien definido, identificando la contradiccion tecnica fundamental y los elementos en conflicto.

La Parte 1 es la mas critica de todo ARIZ. Un analisis deficiente aqui conduce a soluciones debiles o incorrectas. Altshuller insistia en que la mayoria de los fracasos al aplicar ARIZ se deben a errores en la Parte 1.

---

## Paso 1.1: Determinar la mini-tarea

Formular el problema **sin especificar** la solucion ni el metodo. La mini-tarea debe preservar la funcion principal del sistema y eliminar o reducir el efecto danino.

**Formato de la mini-tarea:**

> "El sistema tecnico [nombre] sirve para [funcion util principal]. La contradiccion tecnica 1 (o 2) es [descripcion]. Es necesario, con minimos cambios al sistema, [eliminar/reducir el efecto danino] preservando [la funcion util]."

**Reglas clave:**
- **No proponer la solucion** en la formulacion. La mini-tarea describe *que* se necesita, no *como* lograrlo.
- Buscar la **minima modificacion** al sistema existente (no redisenar desde cero).
- Si el problema tiene varias formulaciones, empezar con la que preserve mejor la funcion principal del sistema.

### Ejemplo

> *Incorrecto*: "Hacer el tubo de acero inoxidable" (ya especifica la solucion).
> *Correcto*: "El tubo de acero sirve para transportar liquido corrosivo. Es necesario eliminar la corrosion del tubo preservando su capacidad de transporte."

---

## Paso 1.2: Identificar los elementos en conflicto

Determinar los dos componentes del conflicto:

- **Herramienta (H)**: el elemento que actua sobre otro, realizando la accion util o danina.
- **Objeto (O)**: el elemento sobre el que actua la herramienta.

**Reglas para identificar H y O:**
1. Si el problema involucra una herramienta y su objeto directo, usarlos tal cual.
2. Si el problema es entre dos objetos que interactuan, la herramienta es el que puede modificarse mas facilmente.
3. Si el problema es interno a un solo objeto, dividirlo en dos partes funcionales.

El par (H, O) define la interaccion conflictiva que ARIZ intentara resolver.

---

## Paso 1.3: Graficos de las contradicciones tecnicas (CT1 y CT2)

Formular las **dos contradicciones tecnicas** opuestas. Toda situacion problematica contiene al menos un par de contradicciones tecnicas complementarias:

**CT1**: Si la herramienta tiene la propiedad A, entonces [accion util], pero [accion danina].

**CT2**: Si la herramienta tiene la propiedad anti-A, entonces [se elimina la accion danina], pero [se pierde la accion util].

Representacion grafica:

```
CT1:   H (propiedad A)  ──→  Accion util sobre O
                         ──→  Accion danina sobre O (o sobre otro elemento)

CT2:   H (propiedad ~A) ──→  Sin accion danina
                         ──→  Sin accion util
```

Este paso fuerza al resolutor a ver las **dos caras** del problema. No se trata de elegir entre A y ~A (eso seria un compromiso), sino de encontrar una forma de tener ambas.

Para identificar los parametros en conflicto, puede consultarse la lista de [39 Parametros de Ingenieria](../03-parametros-ingenieria/00-indice-parametros.md) y la [Matriz de Contradicciones](../04-matriz-contradicciones/00-como-usar-la-matriz.md) como herramientas auxiliares.

---

## Paso 1.4: Elegir la CT que proporciona la funcion principal

Seleccionar la contradiccion tecnica que, al resolverse, **preserva la funcion principal** del sistema tecnico.

**Criterio de seleccion:**
- Elegir la CT cuya accion util es la funcion principal del sistema.
- Si ambas CT involucran la funcion principal, elegir la que tenga la accion danina mas grave.
- Si el sistema es nuevo (no existe aun), elegir la CT que corresponde al desempeno util deseado.

> **Nota**: La eleccion de CT determina todo el flujo posterior de ARIZ. Si al final del proceso no se encuentra solucion, la Parte 6 indica volver aqui y elegir la otra CT.

---

## Paso 1.5: Intensificar la contradiccion

Llevar la contradiccion al extremo: **exagerar** tanto la accion util requerida como la accion danina que aparece. Esto elimina las soluciones de compromiso (*trade-offs*) y obliga a buscar soluciones verdaderamente inventivas.

**Tecnica:**
- Hacer que la accion util sea la maxima posible (ideal).
- Hacer que la accion danina sea la peor posible (catastrofica).

La intensificacion convierte un problema diluido (donde un compromiso parece aceptable) en un problema agudo (donde solo una solucion inventiva funciona).

---

## Paso 1.6: Formular el modelo del problema

El modelo del problema consta de:

1. **El par conflictivo**: la interaccion entre H y O (del paso 1.2).
2. **La contradiccion tecnica intensificada** (del paso 1.5).
3. **La indicacion de que debe cambiar** en el sistema (cual elemento debe modificarse).

**Formato:**

> "El par conflictivo [H, O] presenta la contradiccion: [CT intensificada]. Es necesario encontrar un recurso-X que permita [accion util] sin causar [accion danina]."

El recurso-X es la incognita que ARIZ ayudara a descubrir en las partes siguientes.

---

## Paso 1.7: Aplicar las Soluciones Estandar al modelo

**Primer intento** de solucion usando las [76 Soluciones Estandar](../06-soluciones-estandar/00-indice-soluciones.md).

Con el modelo del problema formulado, verificar si alguna de las 76 Soluciones Estandar es aplicable directamente. Este es el primer punto de salida del algoritmo: si una Solucion Estandar resuelve el problema, se pasa directamente a la Parte 7 (verificacion).

**Procedimiento:**
1. Modelar el conflicto como un modelo [Su-Campo](../05-analisis-su-campo/01-fundamentos-su-campo.md): identificar S1, S2, F.
2. Clasificar el tipo de modelo: incompleto, completo con efecto danino, completo con efecto insuficiente.
3. Buscar en las [5 clases de Soluciones Estandar](../06-soluciones-estandar/00-indice-soluciones.md) la solucion aplicable.

> **Si se encuentra solucion** → pasar a [Parte 7: Analisis de la solucion](07-parte-7-solucion.md).
> **Si no se encuentra** → continuar a [Parte 2: Analisis del modelo del problema](02-parte-2-modelo.md).

---

## Resumen de la Parte 1

| Paso | Accion | Resultado |
|:----:|--------|-----------|
| 1.1 | Formular la mini-tarea | Problema sin solucion predeterminada |
| 1.2 | Identificar H y O | Par conflictivo |
| 1.3 | Formular CT1 y CT2 | Dos contradicciones tecnicas opuestas |
| 1.4 | Elegir la CT principal | CT que preserva la funcion principal |
| 1.5 | Intensificar la CT | Contradiccion extrema sin compromiso |
| 1.6 | Formular el modelo | Modelo del problema con recurso-X |
| 1.7 | Aplicar Soluciones Estandar | Primer intento de solucion |

---

**Navegacion**: [<< Que es ARIZ?](00-que-es-ariz.md) · [Parte 2 >>](02-parte-2-modelo.md)
