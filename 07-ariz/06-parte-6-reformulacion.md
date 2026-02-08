# Parte 6: Cambio o reformulacion del problema

> **Objetivo**: Si las Partes 1-5 no produjeron una solucion satisfactoria, reformular el problema y reiniciar el proceso con una perspectiva diferente.

La Parte 6 es el **mecanismo de iteracion** de ARIZ. No es un fracaso llegar aqui; es una parte natural del algoritmo. Muchos problemas complejos requieren multiples iteraciones antes de encontrar la solucion correcta. Lo importante es que cada iteracion parte de una comprension mas profunda del problema que la anterior.

---

## Paso 6.1: Verificar si el problema se resolvio

Antes de reformular, confirmar que efectivamente no se encontro solucion en las Partes 1-5.

### Criterios de verificacion

- *Se encontro una solucion concreta (no vaga ni parcial) en alguno de los puntos de salida (1.7, 3.6, 4.7, o 5.1-5.4)?*
- Si se encontro una solucion parcial, *resuelve la contradiccion fisica o solo la reduce?*

**Si se encontro una solucion** (aunque sea parcial pero prometedora):
→ Pasar directamente a la [Parte 7: Analisis de la solucion](07-parte-7-solucion.md).

**Si no se encontro solucion:**
→ Continuar al paso 6.2.

---

## Paso 6.2: Reformular la mini-tarea (cambiar la CT o el elemento a modificar)

La primera estrategia de reformulacion es **volver a la Parte 1** con un cambio en la formulacion inicial.

### Opcion A: Elegir la otra contradiccion tecnica

En el paso 1.4, se eligio una de las dos CT (CT1 o CT2). Si el proceso completo no genero solucion con CT1, repetir todo el proceso con CT2.

Recordar:
- **CT1**: H tiene propiedad A → accion util + accion danina.
- **CT2**: H tiene propiedad anti-A → sin accion danina + sin accion util.

La CT no elegida inicialmente puede abrir un espacio de soluciones completamente diferente.

### Opcion B: Cambiar el elemento a modificar

En el paso 1.2, se identificaron la herramienta (H) y el objeto (O), y se decidio que H debia modificarse. La reformulacion consiste en:

- Mantener el par (H, O) pero ahora intentar modificar **O** en lugar de H.
- O bien, redefinir que elemento es H y cual es O (cambiar la perspectiva del conflicto).

### Opcion C: Redefinir el par conflictivo

Si el conflicto real no esta entre los elementos originalmente identificados, reconsiderar:
- *Hay otros pares de elementos en el sistema cuya interaccion genera el conflicto?*
- *El conflicto es realmente entre H y O, o entre O y otro elemento del entorno?*

### Procedimiento

1. Aplicar la reformulacion elegida (A, B o C).
2. Repetir la Parte 1 con la nueva formulacion.
3. Continuar con las Partes 2-5 normalmente.

---

## Paso 6.3: Reformular como tarea general

Si la reformulacion de la mini-tarea (paso 6.2) tampoco produce solucion, el problema es que la mini-tarea puede ser **demasiado restrictiva**.

### Diferencia entre mini-tarea y tarea general

| Tipo | Definicion | Restriccion |
|------|-----------|-------------|
| **Mini-tarea** | Resolver el conflicto con minimos cambios al sistema existente | Alta: el sistema se preserva |
| **Tarea general** | Lograr la funcion principal sin importar los cambios necesarios | Baja: el sistema puede rediseñarse |

### Cuando pasar a tarea general

- La mini-tarea asume que el sistema actual es fundamentalmente correcto y solo necesita un ajuste. Si despues de varias iteraciones no se encuentra solucion, puede ser que el sistema actual tenga una limitacion estructural.
- La tarea general permite considerar arquitecturas alternativas del sistema.

### Procedimiento

1. Reformular el problema como: *"Es necesario lograr [funcion util principal] sin importar los cambios necesarios al sistema."*
2. Reconsiderar si el sistema tecnico actual es el mejor vehiculo para la funcion requerida.
3. Volver a la Parte 1 con esta formulacion ampliada.

### Relacion con las Leyes de Evolucion

Pasar de mini-tarea a tarea general a menudo implica que el sistema esta en un punto de la curva S donde necesita una **transicion evolutiva**. Las [Leyes de Evolucion](../08-leyes-evolucion/00-vision-general.md) pueden orientar hacia que tipo de sistema alternativo evolucionar:

- [Transicion a supersistema](../08-leyes-evolucion/06-ley-transicion-supersistema.md): combinar el sistema con otros.
- [Transicion a micronivel](../08-leyes-evolucion/07-ley-transicion-micronivel.md): reemplazar mecanismos macro por efectos micro.
- [Aumento de dinamismo](../08-leyes-evolucion/08-ley-dinamizacion.md): hacer el sistema mas adaptable.

---

## Paso 6.4: Pasar a un problema de nivel superior

Si ni la reformulacion de la mini-tarea ni la tarea general producen solucion, considerar **cambiar el nivel del problema**.

### Estrategia: Subir al supersistema

En lugar de resolver el problema dentro del sistema actual, reformularlo como un problema del **supersistema** que contiene al sistema:

1. *Cual es el supersistema que incluye al sistema problematico?*
2. *El conflicto existe realmente a nivel del supersistema, o es un artefacto del diseño del subsistema?*
3. *Puede el supersistema reorganizarse para que el conflicto desaparezca?*

### Ejemplo

Si el problema es "el tubo se corroe con el liquido", subir al supersistema "sistema de transporte de liquido" puede llevar a preguntar: *"Necesitamos realmente un tubo? Puede el liquido transportarse de otra forma (canal abierto, encapsulamiento, solidificacion temporal)?"*

### Estrategia: Reformular la funcion

Otra forma de subir de nivel es cuestionar la **funcion** misma:

- *Es realmente necesaria esta funcion?*
- *Puede obtenerse el resultado final sin realizar esta funcion?*
- *Puede otra funcion sustituirla?*

Esto conecta con el concepto de RFI extremo: el sistema ideal es el que no existe pero cuya funcion se cumple.

> **Despues de la reformulacion**, repetir el ciclo Partes 1-5 con la nueva perspectiva. Si tras tres iteraciones completas no se encuentra solucion, revisar los prerrequisitos del problema (informacion incompleta, restricciones artificiales, supuestos incorrectos).

---

## Resumen de la Parte 6

| Paso | Accion | Resultado |
|:----:|--------|-----------|
| 6.1 | Verificar si hay solucion | Confirmar que se necesita reformulacion |
| 6.2 | Reformular la mini-tarea | Cambiar CT, elemento a modificar, o par conflictivo |
| 6.3 | Pasar a tarea general | Eliminar restriccion de preservar el sistema actual |
| 6.4 | Subir de nivel | Reformular como problema del supersistema |

---

**Navegacion**: [<< Parte 5](05-parte-5-conocimientos.md) · [Parte 7 >>](07-parte-7-solucion.md)
