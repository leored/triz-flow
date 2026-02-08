# Etapa 2: Problema Genérico

## Objetivo

Traducir el problema específico (formulado en la [Etapa 1](01-problema-especifico.md)) a un **modelo abstracto TRIZ** que permita aplicar las herramientas del método. Esta es la etapa de abstracción: pasar del lenguaje del dominio al lenguaje de TRIZ.

## Tres caminos de reformulación

Dependiendo del tipo de problema, se elige uno (o varios) de estos modelos:

| Modelo TRIZ | Cuándo usarlo | Herramienta que lo resuelve |
|-------------|--------------|---------------------------|
| **Contradicción técnica** | Mejorar parámetro A empeora parámetro B | Matriz de Contradicciones → 40 Principios |
| **Contradicción física** | Un elemento debe tener propiedades opuestas | Principios de separación |
| **Modelo Su-Campo** | El problema involucra interacciones entre sustancias y campos | 76 Soluciones Estándar |

### Camino 1: Formular como contradicción técnica

1. **Identificar qué se quiere mejorar** → seleccionar el parámetro de ingeniería que mejora (de los [39 parámetros](../03-parametros-ingenieria/00-indice-parametros.md)).
2. **Identificar qué empeora** → seleccionar el parámetro que se degrada como consecuencia.
3. **Expresar la contradicción**:

```
CT: Si mejoro [Parámetro #XX: nombre]
    entonces empeora [Parámetro #YY: nombre]
```

**Ejemplo** (barco):
```
CT: Si mejoro [Parámetro #13: Estabilidad del objeto]
    (mayor espesor de pintura = mejor protección)
    entonces empeora [Parámetro #25: Pérdida de tiempo]
    (más tiempo de aplicación y secado)
```

> Nota: Puede formularse más de una contradicción técnica para el mismo problema. Cada una puede generar distintas soluciones.

### Camino 2: Formular como contradicción física

1. **Identificar el elemento conflictivo** (la parte del sistema donde se concentra el problema).
2. **Definir las dos propiedades opuestas** que ese elemento necesita tener.
3. **Expresar la contradicción**:

```
CF: [Elemento X] debe ser [propiedad A] para [función/razón 1]
    Y debe ser [propiedad opuesta: no-A] para [función/razón 2]
```

**Ejemplo** (barco):
```
CF: La pintura debe ser LÍQUIDA para poder aplicarse sobre el casco
    Y debe ser SÓLIDA para proteger contra la corrosión
```

### Camino 3: Formular como modelo Su-Campo

1. **Identificar las sustancias** (S1: objeto del problema, S2: herramienta que actúa sobre S1).
2. **Identificar el campo** (F: tipo de energía/interacción entre S1 y S2).
3. **Clasificar el modelo** (completo, incompleto, dañino, insuficiente).

```
Modelo Su-Campo:
  S1 = [sustancia 1: objeto]
  S2 = [sustancia 2: herramienta]
  F  = [campo: tipo de interacción]
  Tipo: [completo / incompleto / dañino / insuficiente]
```

**Ejemplo** (barco):
```
  S1 = Casco del barco
  S2 = Pintura anticorrosiva
  F  = Campo mecánico (aplicación por presión)
  Tipo: Insuficiente (la interacción existe pero el resultado no es satisfactorio)
```

→ Ver: [Análisis Su-Campo](../05-analisis-su-campo/01-fundamentos-su-campo.md)

## Reglas de reformulación

### Formular el problema invertido

Una técnica útil es formular el **problema invertido**: ¿cómo haría para *empeorar* la situación al máximo? Luego invertir esa respuesta.

**Ejemplo**: "¿Cómo haría para que la pintura del barco fallara lo más rápido posible?" → Aplicar capa muy fina, en superficie sucia, con pintura caducada. → Invertir: asegurar capa gruesa, superficie limpia, pintura fresca. → Pero esto nos devuelve al problema de partida. → Ahora buscamos maneras de lograr capa gruesa sin los inconvenientes.

### Formular el RFI

Expresar el Resultado Final Ideal para orientar la búsqueda:

```
RFI: [El recurso X / el propio sistema], por sí mismo,
     [realiza la función requerida]
     sin [efectos dañinos / costes / complicaciones]
```

**Ejemplo**:
```
RFI: El casco del barco, por sí mismo, se protege de la corrosión
     sin necesidad de aplicar pintura manualmente.
```

Esto abre el pensamiento hacia: recubrimientos autorreparables, materiales resistentes a la corrosión, protección catódica, etc.

## Errores comunes en esta etapa

| Error | Consecuencia | Corrección |
|-------|-------------|-----------|
| Elegir parámetros de ingeniería demasiado genéricos | La Matriz sugiere principios poco relevantes | Ser lo más específico posible al seleccionar parámetros |
| Formular solo una contradicción | Se pierde la riqueza del problema | Formular al menos 2-3 contradicciones y probar cada una |
| Confundir contradicción técnica con física | Se aplica la herramienta equivocada | CT = dos parámetros distintos; CF = un elemento, dos propiedades opuestas |
| Saltarse el RFI | Se buscan soluciones convencionales | Siempre formular el RFI antes de aplicar herramientas |

---

**Navegación**: [← Etapa 1: Problema específico](01-problema-especifico.md) · [Etapa 3: Solución genérica →](03-solucion-generica.md)
