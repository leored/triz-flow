# ¿Qué es TRIZ?

## Definición

**TRIZ** (Теория решения изобретательских задач — *Teoriya Resheniya Izobretatelskikh Zadach*) es la **Teoría para Resolver Problemas de Inventiva**, desarrollada por Genrich Altshuller y sus colaboradores a partir de 1946 en la Unión Soviética.

TRIZ es un marco metodológico sistemático para la innovación técnica basado en el análisis de patrones extraídos de cientos de miles de patentes. A diferencia de los métodos de creatividad basados en prueba y error (como el *brainstorming*), TRIZ propone que la invención sigue leyes objetivas que pueden estudiarse, formalizarse y enseñarse.

## Premisa central

> **Los problemas de invención ya han sido resueltos antes en otros campos.**
> La clave es reconocer el patrón abstracto del problema y buscar soluciones análogas.

El flujo fundamental de TRIZ es:

```
Problema específico → Problema genérico → Solución genérica → Solución específica
```

En lugar de buscar soluciones directamente (lo que lleva a inercia psicológica), TRIZ abstrae el problema a un modelo conocido y luego adapta las soluciones probadas.

## Pilares de TRIZ

### 1. Contradicciones

Todo problema inventivo contiene una **contradicción**: mejorar un aspecto del sistema empeora otro. TRIZ distingue dos tipos:

- **Contradicción técnica**: mejorar un parámetro del sistema degrada otro parámetro. Ejemplo: aumentar la resistencia de una pieza aumenta su peso.
- **Contradicción física**: un mismo elemento del sistema debe tener propiedades opuestas simultáneamente. Ejemplo: un eje debe ser rígido (para transmitir fuerza) y flexible (para absorber vibraciones).

La innovación real **resuelve** la contradicción en vez de aceptar un compromiso (*trade-off*).

### 2. Idealidad

El **Resultado Final Ideal (RFI)** es el estado en que el sistema cumple su función útil sin existir físicamente (sin costes, sin efectos dañinos). Aunque inalcanzable en la práctica, el RFI orienta la búsqueda de soluciones hacia la máxima eficiencia.

```
            Suma de funciones útiles
Idealidad = ─────────────────────────────────────
            Suma de funciones dañinas + costes
```

### 3. Recursos

Antes de añadir elementos nuevos al sistema, TRIZ exige explotar los **recursos** ya existentes:

- Recursos de sustancia (materiales disponibles)
- Recursos de campo (energías presentes)
- Recursos de espacio y tiempo
- Recursos de información
- Recursos funcionales (funciones no aprovechadas)

### 4. Evolución de sistemas técnicos

Los sistemas técnicos evolucionan siguiendo **leyes objetivas** (no al azar). Conocer estas leyes permite predecir la dirección de evolución y diseñar la próxima generación del sistema.

## ¿Cuándo usar TRIZ?

| Situación | TRIZ es útil | Método alternativo |
|-----------|:------------:|-------------------|
| Problema con contradicción clara (mejorar A empeora B) | ✓ | — |
| Optimización sin contradicción (solo mejorar A) | — | DOE, Six Sigma |
| Problema nuevo sin soluciones conocidas en el campo | ✓ | — |
| Problema bien definido con solución estándar conocida | — | Ingeniería convencional |
| Necesidad de innovación disruptiva | ✓ | — |
| Mejora incremental dentro de parámetros conocidos | — | Kaizen, Lean |
| Predicción de evolución tecnológica | ✓ | Prospectiva tecnológica |

## Herramientas principales de TRIZ

TRIZ no es una sola herramienta, sino un sistema de herramientas interrelacionadas:

| Herramienta | Propósito | Referencia |
|-------------|-----------|------------|
| **40 Principios Inventivos** | Resolver contradicciones técnicas | [02-principios-inventivos/](../02-principios-inventivos/00-indice-principios.md) |
| **39 Parámetros de Ingeniería** | Clasificar qué mejora y qué empeora | [03-parametros-ingenieria/](../03-parametros-ingenieria/00-indice-parametros.md) |
| **Matriz de Contradicciones** | Cruzar parámetros → principios sugeridos | [04-matriz-contradicciones/](../04-matriz-contradicciones/00-como-usar-la-matriz.md) |
| **Análisis Sustancia-Campo** | Modelar problemas como triadas S1-S2-F | [05-analisis-su-campo/](../05-analisis-su-campo/01-fundamentos-su-campo.md) |
| **76 Soluciones Estándar** | Resolver modelos Su-Campo | [06-soluciones-estandar/](../06-soluciones-estandar/00-indice-soluciones.md) |
| **ARIZ-85C** | Algoritmo completo para problemas complejos | [07-ariz/](../07-ariz/00-que-es-ariz.md) |
| **8 Leyes de Evolución** | Predecir dirección de evolución | [08-leyes-evolucion/](../08-leyes-evolucion/00-vision-general.md) |

## Niveles de invención de Altshuller

Altshuller clasificó las soluciones inventivas en 5 niveles según su grado de novedad:

| Nivel | Descripción | % patentes | Soluciones probadas | Herramienta TRIZ |
|:-----:|-------------|:----------:|:-------------------:|-----------------|
| 1 | Solución rutinaria, dentro del oficio | ~32% | ~10 | Conocimiento del dominio |
| 2 | Mejora menor, resolución de contradicción menor | ~45% | ~100 | Principios inventivos, Matriz |
| 3 | Mejora sustancial dentro del paradigma tecnológico | ~18% | ~1.000 | ARIZ, 76 Soluciones |
| 4 | Nuevo principio de funcionamiento | ~4% | ~100.000 | Leyes de evolución, bases de efectos |
| 5 | Descubrimiento científico nuevo | ~1% | ~1.000.000 | Fuera del alcance directo de TRIZ |

TRIZ es más efectivo en los niveles 2-4, donde las soluciones requieren pensamiento inventivo pero pueden encontrarse mediante análisis sistemático.

---

**Navegación**: [← Índice general](../README.md) · [Historia de Altshuller →](02-historia-altshuller.md)
