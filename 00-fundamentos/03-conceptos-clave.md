# Conceptos Clave de TRIZ

Este documento define el vocabulario fundamental de TRIZ. Los términos aquí descritos se utilizan en todas las herramientas del método.

## Sistema técnico

Un **sistema técnico** es cualquier conjunto de elementos organizados para cumplir una **función principal**. TRIZ analiza los sistemas en tres niveles:

| Nivel | Definición | Ejemplo (para un bolígrafo) |
|-------|-----------|----------------------------|
| **Supersistema** | El entorno que contiene al sistema | La mano del usuario, el papel, la mesa |
| **Sistema** | El objeto de estudio | El bolígrafo completo |
| **Subsistema** | Los componentes internos del sistema | Tinta, punta, carcasa, muelle, capuchón |

### Función principal

La función principal de un sistema se define como la **acción** que el sistema ejerce sobre su **objeto** para producir un **resultado útil**.

```
Función = Acción (verbo) + Objeto + Resultado
```

Ejemplo: La función principal de un bolígrafo es *depositar tinta sobre papel para crear marcas visibles*.

## Contradicciones

Las contradicciones son el núcleo del análisis TRIZ. Un problema inventivo existe cuando hay una contradicción que impide la mejora directa.

### Contradicción técnica (CT)

Se produce cuando mejorar un **parámetro** del sistema degrada otro parámetro diferente.

```
Si mejoro A → empeora B
Si mejoro B → empeora A
```

**Ejemplo**: Un avión necesita alas más largas para mayor sustentación (mejora de un parámetro), pero alas más largas aumentan el peso y la resistencia aerodinámica (empeoran otros parámetros).

Las contradicciones técnicas se resuelven usando la **Matriz de Contradicciones** y los **40 Principios Inventivos**.

→ Ver: [Matriz de Contradicciones](../04-matriz-contradicciones/00-como-usar-la-matriz.md)

### Contradicción física (CF)

Se produce cuando un **mismo elemento** del sistema debe poseer **propiedades opuestas** simultáneamente.

```
El elemento X debe ser A (para cumplir función 1)
El elemento X debe ser no-A (para cumplir función 2)
```

**Ejemplo**: El café debe estar caliente (para el sabor) y frío (para beberlo inmediatamente).

Las contradicciones físicas se resuelven mediante cuatro principios de separación:

| Principio de separación | Estrategia | Ejemplo |
|------------------------|-----------|---------|
| **En el tiempo** | X es A en un momento y no-A en otro | El café está caliente al servirlo y se enfría al soplar |
| **En el espacio** | X es A en una zona y no-A en otra | El vaso térmico: caliente dentro, frío fuera |
| **Entre el todo y las partes** | Las partes tienen propiedad A, el todo tiene propiedad no-A | Una cadena es flexible (todo) pero cada eslabón es rígido (parte) |
| **Bajo condición** | X es A bajo una condición y no-A bajo otra | Un cristal fotocromático es oscuro con luz UV y transparente sin ella |

### Contradicción administrativa (CA)

Existe cuando se sabe *qué* se necesita lograr pero no se sabe *cómo*. No es una contradicción TRIZ propiamente dicha; es el punto de partida que debe reformularse como CT o CF.

## Resultado Final Ideal (RFI)

El **Resultado Final Ideal** (en ruso: ИКР, Идеальный Конечный Результат) es una herramienta de pensamiento que define la solución perfecta:

> **El elemento X, por sí mismo, realiza la acción requerida en el momento y lugar necesarios, sin causar efectos dañinos y sin añadir complejidad al sistema.**

El RFI no es una solución práctica, sino una **dirección de búsqueda**. Fuerza al inventor a:

1. Definir exactamente **qué** necesita ocurrir (no cómo).
2. Eliminar la inercia psicológica que lleva a soluciones convencionales.
3. Buscar soluciones que se acerquen lo máximo posible a "el problema se resuelve solo".

### Formulación del RFI

```
[Elemento del sistema o recurso disponible]
por sí mismo
[realiza la acción útil requerida]
durante [tiempo requerido]
en [lugar requerido]
sin [efectos dañinos / costes / complicaciones]
```

**Ejemplo**: "La pintura, por sí misma, indica cuándo ha sido expuesta a temperatura excesiva, sin necesidad de sensores externos." → Esto lleva a la idea de pinturas termocromáticas.

## Recursos

Los **recursos** son sustancias, campos, propiedades, información o funciones que ya están presentes en el sistema o en su entorno y que pueden usarse para resolver el problema sin añadir elementos nuevos.

### Clasificación de recursos

| Tipo | Descripción | Ejemplos |
|------|------------|---------|
| **Sustancias** | Materiales presentes en el sistema o entorno | Aire, agua, residuos, material del propio objeto |
| **Campos / Energías** | Energías disponibles o generables | Gravedad, calor residual, vibración, campos magnéticos |
| **Espacio** | Espacio no utilizado dentro o fuera del sistema | Huecos, superficies, dimensiones no aprovechadas |
| **Tiempo** | Intervalos temporales no aprovechados | Pausas, periodos previos/posteriores, simultaneidad |
| **Información** | Datos o señales disponibles | Color, forma, posición, secuencia |
| **Funcionales** | Funciones secundarias de elementos existentes | Un envase que también sirve como herramienta |

### Regla de uso de recursos

TRIZ establece una jerarquía para la búsqueda de soluciones:

1. **Primero**: usar recursos internos del sistema (subsistema).
2. **Segundo**: usar recursos del entorno inmediato (supersistema).
3. **Tercero**: usar recursos de un sistema externo diferente.
4. **Solo si no hay alternativa**: añadir un elemento nuevo.

## Niveles de invención

Altshuller clasificó las invenciones en **5 niveles** según la distancia entre el problema y la solución:

### Nivel 1 — Solución aparente
- **Descripción**: Solución obvia dentro del dominio, sin resolver contradicción.
- **Búsqueda**: ~10 variantes.
- **Ejemplo**: Cambiar el diámetro de un tornillo para ajustar la resistencia.

### Nivel 2 — Mejora menor
- **Descripción**: Resolución de una contradicción técnica menor, dentro del dominio.
- **Búsqueda**: ~100 variantes.
- **Ejemplo**: Usar un material diferente para reducir peso sin perder resistencia.

### Nivel 3 — Mejora sustancial
- **Descripción**: Resolución de una contradicción dentro del campo tecnológico, pero con solución proveniente de otro campo.
- **Búsqueda**: ~1.000 variantes.
- **Ejemplo**: Aplicar el efecto piezoeléctrico (campo de la física) para autodiagnóstico en una estructura mecánica.

### Nivel 4 — Nuevo principio de funcionamiento
- **Descripción**: Solución fuera del campo tecnológico actual; se basa en un efecto o fenómeno científico nuevo para el dominio.
- **Búsqueda**: ~100.000 variantes.
- **Ejemplo**: Reemplazar un sistema mecánico por uno óptico (p. ej., lectura láser en vez de aguja fonográfica).

### Nivel 5 — Descubrimiento
- **Descripción**: Basada en un fenómeno científico previamente desconocido.
- **Búsqueda**: ~1.000.000 variantes.
- **Ejemplo**: El descubrimiento de la superconductividad permite trenes de levitación magnética.

## Inercia psicológica

La **inercia psicológica** es la tendencia humana a buscar soluciones dentro de lo ya conocido, repitiendo enfoques familiares. TRIZ combate la inercia psicológica mediante:

- **Reformulación del problema**: expresar el problema en términos abstractos (contradicciones, RFI).
- **Operador STC** (*Tamaño-Tiempo-Costo*): imaginar qué pasa si un parámetro se lleva al extremo (infinito o cero).
- **Método del hombrecillo inteligente** (*smart little people*): imaginar que el sistema está compuesto por pequeñas criaturas inteligentes que pueden reorganizarse a voluntad.
- **Inversión**: considerar la solución opuesta a la intuitiva.

## Mapa de relaciones entre conceptos

```
                    Contradicción administrativa
                              │
                    (reformular como)
                              │
               ┌──────────────┴──────────────┐
               ▼                              ▼
    Contradicción técnica           Contradicción física
               │                              │
     (resolver con)                  (resolver con)
               │                              │
    ┌──────────┴──────────┐         Principios de separación
    ▼                     ▼           (tiempo, espacio,
  Matriz de           Análisis         todo/partes, condición)
  Contradicciones     Su-Campo
    │                     │
    ▼                     ▼
  40 Principios       76 Soluciones
  Inventivos          Estándar
    │                     │
    └──────────┬──────────┘
               ▼
            ARIZ-85C
         (integra todo)
```

---

**Navegación**: [← Historia de Altshuller](02-historia-altshuller.md) · [Flujo TRIZ →](../01-flujo-triz/00-vision-general.md)
