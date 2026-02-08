# Parte 5: Aplicacion de la base de conocimientos

> **Objetivo**: Ampliar la busqueda de soluciones mediante la aplicacion sistematica de bases de conocimientos cientificos y tecnicos: Soluciones Estandar, efectos fisicos, efectos quimicos y efectos geometricos.

La Parte 5 es el tercer y ultimo intento sistematico de resolver el problema dentro del ciclo principal de ARIZ (Partes 1-5). A diferencia de los intentos anteriores (pasos 1.7 y 3.6), aqui el resolutor cuenta con:

- La contradiccion fisica formulada y separada (Parte 3).
- Los recursos inventariados y movilizados (Partes 2 y 4).
- Una comprension profunda de la zona operativa y el tiempo operativo.

---

## Paso 5.1: Aplicar las 76 Soluciones Estandar (tercer intento)

Este es el **tercer intento** de aplicar las [76 Soluciones Estandar](../06-soluciones-estandar/00-indice-soluciones.md), ahora con el maximo nivel de comprension del problema.

### Diferencia con los intentos anteriores

| Intento | Paso | Nivel de comprension | Enfoque |
|:-------:|:----:|---------------------|---------|
| 1o | 1.7 | Modelo del problema | Busqueda general por tipo de modelo Su-Campo |
| 2o | 3.6 | CF explicita | Busqueda guiada por la contradiccion fisica |
| **3o** | **5.1** | **CF + recursos + separacion** | **Busqueda precisa con criterios multiples** |

### Procedimiento

1. Revisar las 5 clases de Soluciones Estandar con los siguientes filtros:
   - *Que clase corresponde al tipo de modelo Su-Campo del conflicto?*
   - *Que soluciones abordan el tipo de separacion identificado en el paso 4.4?*
   - *Que soluciones utilizan los recursos identificados en los pasos 2.3, 4.5 y 4.6?*

2. Prestar especial atencion a:
   - [Clase 1](../06-soluciones-estandar/01-clase-1-construir.md): Si el modelo Su-Campo es incompleto o tiene interaccion danina.
   - [Clase 2](../06-soluciones-estandar/02-clase-2-desarrollar.md): Si el modelo necesita mayor eficiencia (campo insuficiente).
   - [Clase 3](../06-soluciones-estandar/03-clase-3-transicion.md): Si la solucion requiere transicion a supersistema o micronivel.
   - [Clase 4](../06-soluciones-estandar/04-clase-4-deteccion.md): Si el problema es de deteccion o medicion.
   - [Clase 5](../06-soluciones-estandar/05-clase-5-estrategias.md): Si se necesitan estrategias de simplificacion.

3. Si una Solucion Estandar es aplicable, formular la solucion concreta y pasar a la [Parte 7](07-parte-7-solucion.md).

---

## Paso 5.2: Aplicar los efectos fisicos

Si las Soluciones Estandar no resuelven el problema, buscar en la **base de datos de efectos fisicos** un efecto que proporcione la funcion requerida.

### Que es un efecto fisico

Un efecto fisico es un fenomeno natural documentado que produce un resultado especifico cuando se dan ciertas condiciones. Altshuller y sus colaboradores compilaron cientos de efectos fisicos organizados por la funcion que realizan.

### Procedimiento

1. Formular la funcion necesaria en terminos simples: *"Se necesita [accion] sobre [objeto] usando [condicion]."*
2. Buscar en la tabla de efectos fisicos que fenomenos proporcionan esa funcion.
3. Evaluar si el efecto encontrado puede implementarse con los recursos disponibles.

### Efectos fisicos frecuentes en soluciones inventivas

| Funcion requerida | Efectos fisicos aplicables |
|-------------------|---------------------------|
| Generar fuerza mecanica | Expansion termica, presion osmotica, piezoelectricidad, magnetostriccion |
| Cambiar de forma | Memoria de forma, bimetales, polimeros electroactivos |
| Generar calor | Efecto Joule, friccion, induccion, reacciones exotermicas |
| Eliminar calor | Efecto Peltier, evaporacion, radiacion |
| Detectar cambios | Efecto fotoelectrico, resonancia, piezoelectricidad, fluorescencia |
| Mover fluidos | Capilaridad, electroosmosis, efecto Marangoni, conveccion |
| Generar luz | Luminiscencia, triboluminiscencia, electroluminiscencia |

### Conexion con TRIZ

La base de efectos fisicos es complementaria a las [76 Soluciones Estandar](../06-soluciones-estandar/00-indice-soluciones.md). Mientras las Soluciones Estandar dicen *que tipo* de transformacion hacer al modelo Su-Campo, los efectos fisicos dicen *con que fenomeno concreto* implementarla.

---

## Paso 5.3: Aplicar los efectos quimicos

Buscar en la **base de datos de efectos quimicos** reacciones que puedan proporcionar la funcion requerida, especialmente si el paso 5.2 no produjo resultados o si la contradiccion fisica involucra propiedades quimicas.

### Efectos quimicos frecuentes

| Funcion requerida | Efectos quimicos aplicables |
|-------------------|-----------------------------|
| Generar gas | Descomposicion, efervescencia, electrolisis |
| Generar calor | Reacciones exotermicas, oxidacion, polimerizacion |
| Absorber calor | Reacciones endotermicas, disolucion de sales |
| Cambiar viscosidad | Gelificacion, polimerizacion, cambio de pH |
| Proteger superficie | Pasivacion, anodizado, recubrimiento autocatalitico |
| Generar fuerza | Expansion de gas (reaccion quimica), presion osmotica |
| Limpiar | Disolucion selectiva, catalisis, oxidacion |

### Sustancias derivadas

Recordar los recursos del paso 4.5: las sustancias derivadas de lo ya existente en el sistema. Una reaccion quimica entre componentes del propio sistema puede generar la sustancia o el efecto necesario sin introducir nada nuevo.

---

## Paso 5.4: Aplicar efectos geometricos y tabla de separacion de CFs

Si los efectos fisicos y quimicos no resuelven el problema, revisar dos recursos adicionales:

### Efectos geometricos

Considerar si la solucion puede encontrarse mediante una **reconfiguracion geometrica** de la zona operativa:

- Cambio de forma (de plano a curvo, de simetrico a asimetrico).
- Cambio de dimension (de 1D a 2D, de 2D a 3D).
- Uso de geometrias fractales o porosas.
- Inversion geometrica (interior ↔ exterior, concavo ↔ convexo).

Principios inventivos relacionados: [04 Asimetria](../02-principios-inventivos/04-asimetria.md), [07 Anidamiento](../02-principios-inventivos/07-anidamiento.md), [14 Esferoidalidad](../02-principios-inventivos/14-esferoidalidad.md), [17 Cambio de dimension](../02-principios-inventivos/17-cambio-de-dimension.md).

### Tabla de principios para resolver contradicciones fisicas

Altshuller desarrollo una tabla especifica para la resolucion de CFs que cruza el **tipo de separacion** (tiempo, espacio, todo/partes, condicion) con los [40 Principios Inventivos](../02-principios-inventivos/00-indice-principios.md) mas frecuentes para cada tipo:

| Tipo de separacion | Principios inventivos mas frecuentes |
|--------------------|--------------------------------------|
| En el tiempo | 15, 16, 18, 19, 20, 21, 26, 34, 37 |
| En el espacio | 1, 2, 3, 4, 7, 13, 17, 24, 26, 30 |
| Entre todo y partes | 1, 5, 6, 7, 8, 22, 25, 27, 31, 33, 40 |
| Por condicion | 28, 29, 35, 36, 38, 39 |

> **Si se encuentra solucion** → pasar a [Parte 7: Analisis de la solucion](07-parte-7-solucion.md).
> **Si no se encuentra** → continuar a [Parte 6: Cambio o reformulacion del problema](06-parte-6-reformulacion.md).

---

## Resumen de la Parte 5

| Paso | Accion | Resultado |
|:----:|--------|-----------|
| 5.1 | Soluciones Estandar (3er intento) | Busqueda precisa con maxima comprension |
| 5.2 | Efectos fisicos | Fenomenos fisicos para implementar la solucion |
| 5.3 | Efectos quimicos | Reacciones quimicas como recurso de solucion |
| 5.4 | Efectos geometricos y tabla de CFs | Reconfiguracion geometrica y principios por separacion |

---

**Navegacion**: [<< Parte 4](04-parte-4-recursos.md) · [Parte 6 >>](06-parte-6-reformulacion.md)
