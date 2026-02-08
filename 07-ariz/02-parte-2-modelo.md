# Parte 2: Analisis del modelo del problema

> **Objetivo**: Delimitar con precision *donde*, *cuando* y *con que* ocurre el conflicto. Definir la zona operativa, el tiempo operativo y los recursos sustancia-campo disponibles.

La Parte 2 transforma el modelo abstracto del problema (formulado en la Parte 1) en un modelo espaciotemporal concreto. Esta concrecion es esencial para que las Partes 3-5 puedan buscar soluciones dentro del espacio real del conflicto, no en abstracciones vagas.

---

## Paso 2.1: Determinar la zona operativa (ZO)

La **zona operativa** es el espacio fisico donde ocurre el conflicto entre la herramienta (H) y el objeto (O).

### Como definir la zona operativa

1. Identificar la region exacta donde la accion util y la accion danina coexisten.
2. La ZO no es todo el sistema: es la zona minima donde se manifiesta la contradiccion.
3. Si el conflicto ocurre en una superficie de contacto, la ZO es esa superficie (y su entorno inmediato).
4. Si el conflicto ocurre en un volumen, la ZO es ese volumen.

### Reglas de delimitacion

- **Reducir** la ZO tanto como sea posible. Cuanto mas pequena la zona, mas facil encontrar el recurso que resuelve el conflicto.
- No confundir la ZO con todo el espacio del sistema tecnico. El conflicto es local, no global.
- En algunos casos la ZO puede tener geometria variable (cambia con el tiempo). En ese caso, definir la ZO para cada momento relevante.

### Ejemplo

En el problema del tubo que transporta liquido corrosivo, la ZO no es todo el tubo: es la **superficie interna del tubo en contacto con el liquido**. Ahi es donde coexisten la funcion util (contener y guiar el fluido) y la accion danina (la corrosion).

---

## Paso 2.2: Determinar el tiempo operativo (TO)

El **tiempo operativo** define los intervalos temporales relevantes para el conflicto. ARIZ distingue dos intervalos:

### T1: Tiempo del conflicto

El periodo durante el cual la accion danina se manifiesta activamente. Es el momento en que la contradiccion esta "viva".

- *Cuando exactamente se produce la accion danina?*
- *Cuanto dura?*
- *Es continua o intermitente?*

### T2: Tiempo antes del conflicto

El periodo inmediatamente anterior a T1. Este intervalo es estrategicamente importante porque ofrece la oportunidad de **preparar** la zona operativa antes de que el conflicto aparezca.

- *Que ocurre justo antes del conflicto?*
- *Se puede actuar preventivamente en este periodo?*
- *Se pueden movilizar recursos durante T2 para que esten disponibles en T1?*

### Por que importa T2

Muchas soluciones inventivas actuan en T2, no en T1. Es mas facil prevenir un conflicto que resolverlo mientras ocurre. El concepto de [accion previa](../02-principios-inventivos/09-accion-previa.md) y [accion anticipada](../02-principios-inventivos/10-accion-anticipada.md) (principios inventivos 9 y 10) se basan en esta idea.

### Ejemplo

En el problema del tubo con liquido corrosivo:
- **T1**: todo el tiempo que el liquido esta en contacto con el tubo (durante el flujo).
- **T2**: el momento antes de que el liquido ingrese al tubo (o durante la fabricacion del tubo).

---

## Paso 2.3: Determinar los recursos sustancia-campo disponibles

Los **recursos** son todas las sustancias y campos que estan presentes en el sistema y su entorno y que pueden usarse para resolver el conflicto. Altshuller clasifico los recursos en tres categorias segun su origen:

### Recursos del sistema (internos)

Sustancias y campos que ya forman parte del sistema tecnico:

- La propia herramienta (H) y sus propiedades no utilizadas.
- El propio objeto (O) y sus propiedades no utilizadas.
- Los subproductos de la interaccion H-O.
- Los campos presentes en la operacion del sistema (termico, mecanico, electromagnetico, etc.).

### Recursos del entorno

Sustancias y campos presentes en el ambiente donde opera el sistema:

- El medio circundante (aire, agua, temperatura ambiente, gravedad).
- Sustancias residuales o desperdicios presentes en el entorno.
- Campos ambientales (luz solar, campo magnetico terrestre, vibraciones del entorno).

### Recursos del supersistema

Sustancias y campos del sistema mayor que contiene al sistema tecnico:

- Otros subsistemas adyacentes.
- Flujos de energia o materia del supersistema que pasan por la zona operativa.
- Funciones no aprovechadas de otros componentes del supersistema.

### Jerarquia de preferencia

ARIZ establece una preferencia clara al seleccionar recursos:

| Prioridad | Tipo de recurso | Razon |
|:---------:|-----------------|-------|
| 1 (mejor) | Recursos de la zona operativa | No requieren cambios al sistema |
| 2 | Recursos del sistema (fuera de la ZO) | Cambio minimo al sistema |
| 3 | Recursos del entorno | Disponibles sin costo, pero requieren integracion |
| 4 | Recursos del supersistema | Pueden requerir cambios significativos |
| 5 (peor) | Recursos nuevos (introducir sustancias o campos) | Ultimo recurso; aumenta complejidad |

Esta jerarquia esta directamente vinculada al concepto de **idealidad**: la solucion ideal no introduce nada nuevo, solo aprovecha lo que ya existe. Ver el concepto de [aumento de idealidad](../08-leyes-evolucion/04-ley-idealidad.md) en las Leyes de Evolucion.

### Tabla de inventario de recursos

Es recomendable crear una tabla como la siguiente para cada problema:

| Recurso | Tipo | Disponible en ZO | Disponible en T1 | Disponible en T2 | Propiedades utiles |
|---------|------|:-----------------:|:-----------------:|:-----------------:|-------------------|
| (listar) | Sust./Campo | Si/No | Si/No | Si/No | (describir) |

Este inventario sera la base para las Partes 3 y 4, donde se formulara el RFI y se movilizaran los recursos para resolver la contradiccion fisica.

---

## Conexion con las Partes 1 y 3

La Parte 2 funciona como puente entre el analisis abstracto (Parte 1) y la formulacion del ideal (Parte 3):

```
Parte 1 (modelo abstracto)
    │
    ▼
Parte 2 (modelo espaciotemporal + recursos)
    │
    ▼
Parte 3 (RFI + contradiccion fisica)
```

Sin la Parte 2, el Resultado Final Ideal de la Parte 3 seria una abstraccion sin anclaje fisico. Los recursos identificados aqui son los candidatos concretos para convertirse en el "recurso-X" postulado en el paso 1.6.

---

## Resumen de la Parte 2

| Paso | Accion | Resultado |
|:----:|--------|-----------|
| 2.1 | Definir la zona operativa | Espacio fisico minimo del conflicto |
| 2.2 | Definir el tiempo operativo | T1 (durante conflicto) y T2 (antes del conflicto) |
| 2.3 | Inventariar recursos | Lista de sustancias y campos disponibles, priorizados |

---

**Navegacion**: [<< Parte 1](01-parte-1-analisis.md) · [Parte 3 >>](03-parte-3-rfi.md)
