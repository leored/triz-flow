# ARIZ-85C: Algoritmo para la Resolucion de Problemas Inventivos

## Que es ARIZ

**ARIZ** (Алгоритм решения изобретательских задач — *Algoritm Resheniya Izobretatelskikh Zadach*) es el **Algoritmo para la Resolucion de Problemas Inventivos**, la herramienta mas potente y completa de todo el sistema TRIZ. Mientras que las demas herramientas TRIZ (Matriz de Contradicciones, 76 Soluciones Estandar, Analisis Su-Campo) abordan aspectos parciales de un problema, ARIZ integra todas ellas en un proceso secuencial riguroso que guia al inventor paso a paso desde la formulacion del problema hasta la solucion y su verificacion.

ARIZ no es un metodo heuristico ni creativo en el sentido habitual. Es un **algoritmo analitico**: una secuencia logica de pasos que obliga al pensador a superar la inercia psicologica, identificar las contradicciones reales del sistema y resolverlas usando recursos ya disponibles.

## Historia y versiones

Altshuller desarrollo ARIZ de forma iterativa a lo largo de casi tres decadas. Cada version incorporo los hallazgos de la investigacion continua sobre patentes y la experiencia de aplicacion practica:

| Version | Ano | Caracteristicas principales |
|---------|:---:|----------------------------|
| ARIZ-56 | 1959 | Primera version publicada. Proceso basico de analisis de contradicciones. |
| ARIZ-61 | 1961 | Incorporacion del concepto de Resultado Final Ideal (RFI). |
| ARIZ-64 | 1964 | Operador STC (Tamano-Tiempo-Costo) para vencer inercia psicologica. |
| ARIZ-68 | 1968 | Primer uso sistematico de las tablas de efectos fisicos. |
| ARIZ-71 | 1971 | Integracion del analisis Sustancia-Campo. |
| ARIZ-77 | 1977 | Nueve partes completas. Uso de Soluciones Estandar. |
| ARIZ-82 | 1982 | Refinamiento del flujo. Contradiccion fisica explicita. |
| **ARIZ-85C** | **1985** | **Version definitiva**. Estructura consolidada en 9 partes y ~40 pasos. |

ARIZ-85C es la version canonica reconocida por la comunidad TRIZ internacional. Las versiones posteriores propuestas por otros autores no alcanzaron el mismo consenso.

## Cuando usar ARIZ

ARIZ esta disenado para **problemas complejos** donde las herramientas mas simples de TRIZ no bastan. La regla practica es:

| Nivel inventivo | Herramienta adecuada | ARIZ necesario |
|:---------------:|----------------------|:--------------:|
| 1 (rutinario) | Conocimiento del dominio | No |
| 2 (mejora menor) | [Matriz de Contradicciones](../04-matriz-contradicciones/00-como-usar-la-matriz.md), [40 Principios](../02-principios-inventivos/00-indice-principios.md) | No |
| 3 (mejora sustancial) | [76 Soluciones Estandar](../06-soluciones-estandar/00-indice-soluciones.md), ARIZ | Si |
| 4 (nuevo principio) | ARIZ, [Leyes de Evolucion](../08-leyes-evolucion/00-vision-general.md) | Si |
| 5 (descubrimiento) | Fuera del alcance directo de TRIZ | Parcial |

**Usar ARIZ cuando:**
- Las herramientas simples (Matriz, Principios) no generan soluciones satisfactorias.
- El problema contiene contradicciones que no se resuelven con un solo principio.
- No esta claro cual es la contradiccion real del sistema.
- Existe una fuerte inercia psicologica que impide ver soluciones no obvias.

## Prerrequisitos

Para aplicar ARIZ-85C de forma efectiva, el resolutor debe comprender:

1. **Contradicciones tecnicas y fisicas** — [Conceptos clave](../00-fundamentos/03-conceptos-clave.md)
2. **Analisis Sustancia-Campo (Su-Campo)** — [Fundamentos Su-Campo](../05-analisis-su-campo/01-fundamentos-su-campo.md)
3. **40 Principios Inventivos** — [Indice de principios](../02-principios-inventivos/00-indice-principios.md)
4. **76 Soluciones Estandar** — [Indice de soluciones](../06-soluciones-estandar/00-indice-soluciones.md)
5. **Resultado Final Ideal (RFI)** — Concepto de idealidad y como formularlo
6. **Recursos** — Clasificacion y deteccion de recursos del sistema, entorno y supersistema

## Las 9 partes de ARIZ-85C

ARIZ-85C se estructura en **9 partes** con aproximadamente 40 pasos en total. Las partes 1-6 forman el nucleo analitico-resolutivo; las partes 7-9 son de verificacion, generalizacion y aprendizaje.

| Parte | Nombre | Objetivo | Pasos |
|:-----:|--------|----------|:-----:|
| **1** | [Analisis del problema](01-parte-1-analisis.md) | Identificar la contradiccion tecnica y formular el modelo del problema | 1.1 – 1.7 |
| **2** | [Analisis del modelo del problema](02-parte-2-modelo.md) | Definir zona operativa, tiempo operativo y recursos disponibles | 2.1 – 2.3 |
| **3** | [Definicion del RFI y Contradiccion Fisica](03-parte-3-rfi.md) | Formular el Resultado Final Ideal y la contradiccion fisica | 3.1 – 3.6 |
| **4** | [Movilizacion de recursos](04-parte-4-recursos.md) | Aplicar metodos para vencer inercia y movilizar recursos | 4.1 – 4.7 |
| **5** | [Aplicacion de la base de conocimientos](05-parte-5-conocimientos.md) | Aplicar Soluciones Estandar, efectos fisicos, quimicos y geometricos | 5.1 – 5.4 |
| **6** | [Cambio o reformulacion del problema](06-parte-6-reformulacion.md) | Si no hay solucion, reformular el problema y reiniciar | 6.1 – 6.4 |
| **7** | [Analisis de la solucion](07-parte-7-solucion.md) | Verificar que la solucion satisface el RFI y registrar sub-problemas | 7.1 – 7.4 |
| **8** | [Uso maximo de la solucion](08-parte-8-uso-maximo.md) | Generalizar la solucion al supersistema y otros problemas | 8.1 – 8.3 |
| **9** | [Analisis del proceso de resolucion](09-parte-9-proceso.md) | Reflexion metacognitiva sobre el proceso seguido | 9.1 – 9.3 |

## Flujo general

```
Parte 1 ──→ Parte 2 ──→ Parte 3 ──→ Parte 4 ──→ Parte 5
  │                                                   │
  │                     Parte 6  ←────────────────────┘
  │                       │ (si no hay solucion, reformular y volver a Parte 1)
  │                       │
  │                     Parte 7 ──→ Parte 8 ──→ Parte 9
  │                       │
  └───────────────────────┘
```

Las partes 1-5 forman un ciclo que puede repetirse varias veces (a traves de la Parte 6) hasta encontrar una solucion que satisfaga el Resultado Final Ideal.

## Relacion con otras herramientas TRIZ

ARIZ no reemplaza las demas herramientas; las **orquesta**:

- Los [40 Principios Inventivos](../02-principios-inventivos/00-indice-principios.md) se aplican en la Parte 4 para resolver la contradiccion fisica.
- Las [76 Soluciones Estandar](../06-soluciones-estandar/00-indice-soluciones.md) se intentan en las Partes 1, 3 y 5 (tres intentos con niveles crecientes de comprension del problema).
- El [Analisis Su-Campo](../05-analisis-su-campo/01-fundamentos-su-campo.md) se usa para modelar el conflicto.
- Las [Leyes de Evolucion](../08-leyes-evolucion/00-vision-general.md) orientan la direccion de la solucion.
- La [Matriz de Contradicciones](../04-matriz-contradicciones/00-como-usar-la-matriz.md) puede usarse como herramienta auxiliar en el paso 1.3.

---

**Navegacion**: [<< Indice general](../README.md) · [Parte 1: Analisis del problema >>](01-parte-1-analisis.md)
