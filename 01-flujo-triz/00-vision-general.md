# Visión General del Flujo TRIZ

## El flujo fundamental

TRIZ se basa en un flujo de cuatro etapas que transforma un problema específico en una solución específica, pasando por modelos genéricos:

```
┌─────────────────┐         ┌─────────────────┐
│   1. PROBLEMA    │────────▶│   2. PROBLEMA    │
│   ESPECÍFICO     │ abstraer│   GENÉRICO       │
│                  │         │   (modelo TRIZ)   │
└─────────────────┘         └────────┬──────────┘
                                     │
                                     │ aplicar herramientas
                                     ▼
┌─────────────────┐         ┌─────────────────┐
│   4. SOLUCIÓN    │◀────────│   3. SOLUCIÓN    │
│   ESPECÍFICA     │ adaptar │   GENÉRICA       │
│                  │         │   (patrón TRIZ)   │
└─────────────────┘         └─────────────────┘
```

Este flujo evita la búsqueda directa (problema → solución por prueba y error) que lleva a inercia psicológica y soluciones convencionales.

## Detalle de cada etapa

| Etapa | Qué se hace | Resultado |
|-------|------------|-----------|
| [1. Problema específico](01-problema-especifico.md) | Analizar la situación real, identificar funciones, contradicciones, recursos | Formulación clara del problema y sus contradicciones |
| [2. Problema genérico](02-problema-generico.md) | Reformular como modelo TRIZ: contradicción técnica, física, o modelo Su-Campo | Modelo abstracto reconocible por las herramientas TRIZ |
| [3. Solución genérica](03-solucion-generica.md) | Aplicar la herramienta correspondiente para obtener un principio o patrón de solución | Principio(s) inventivo(s), solución estándar, o dirección de solución |
| [4. Solución específica](04-solucion-especifica.md) | Traducir el principio genérico al contexto del problema real | Solución concreta implementable |

## Mapa de decisión: ¿Qué herramienta usar?

```
                        ¿El problema está claro?
                              │
                    ┌─── NO ──┴── SÍ ───┐
                    ▼                    ▼
              Usar ARIZ-85C        ¿Se puede formular
              (Parte 1: análisis)   como contradicción?
                                         │
                               ┌── SÍ ──┴── NO ──┐
                               ▼                   ▼
                    ¿Qué tipo de              Formular como
                    contradicción?            modelo Su-Campo
                         │                         │
                ┌── CT ──┴── CF ──┐               ▼
                ▼                  ▼         76 Soluciones
          Matriz de         Principios de    Estándar
          Contradicciones   separación
                │           (tiempo, espacio,
                ▼            todo/partes,
          40 Principios      condición)
          Inventivos

          Si ninguna herramienta simple resuelve el problema:
                              │
                              ▼
                         ARIZ-85C
                    (algoritmo completo)
```

### Guía rápida de selección

| Situación | Herramienta recomendada | Referencia |
|-----------|------------------------|------------|
| Contradicción técnica clara: mejorar A empeora B | Matriz de Contradicciones → 40 Principios | [04-matriz](../04-matriz-contradicciones/00-como-usar-la-matriz.md) |
| Contradicción física clara: X debe ser A y no-A | Principios de separación | [03-conceptos-clave](../00-fundamentos/03-conceptos-clave.md) |
| Problema modelable como interacción entre sustancias y campos | Análisis Su-Campo → 76 Soluciones | [05-su-campo](../05-analisis-su-campo/01-fundamentos-su-campo.md) |
| Problema complejo, las herramientas simples no dan resultado | ARIZ-85C | [07-ariz](../07-ariz/00-que-es-ariz.md) |
| Necesidad de predecir evolución de un sistema | 8 Leyes de Evolución | [08-leyes](../08-leyes-evolucion/00-vision-general.md) |
| Problema no técnico (negocios, gestión, software) | Adaptar: primero modelar como sistema técnico análogo | — |

## Iteración

El flujo TRIZ no es estrictamente lineal. Es común:

1. **Reformular**: Si la herramienta no genera buenas soluciones, volver a la etapa 2 y reformular el problema (distinta contradicción, distinto modelo).
2. **Escalar**: Si las herramientas simples no funcionan, escalar a ARIZ-85C.
3. **Combinar**: Usar varias herramientas en paralelo y comparar resultados.
4. **Iterar**: Resolver un problema puede revelar un nuevo problema (la solución genera una nueva contradicción) que requiere otro ciclo.

## Relación entre herramientas

```
                    ┌──────────────────────┐
                    │     ARIZ-85C          │
                    │  (integra todas las   │
                    │   herramientas)       │
                    └──────────┬───────────┘
                               │
            ┌──────────────────┼──────────────────┐
            ▼                  ▼                   ▼
   ┌────────────────┐  ┌──────────────┐   ┌──────────────┐
   │ Contradicciones │  │  Su-Campo    │   │ Leyes de     │
   │ técnicas        │  │  + 76 Sol.   │   │ Evolución    │
   │ + Matriz        │  │  Estándar    │   │              │
   │ + 40 Principios │  │              │   │              │
   └────────────────┘  └──────────────┘   └──────────────┘

   Problemas con         Problemas de        Predicción y
   trade-off claro       interacción         dirección de
   entre parámetros      sustancia-campo     desarrollo
```

---

**Navegación**: [← Conceptos clave](../00-fundamentos/03-conceptos-clave.md) · [Etapa 1: Problema específico →](01-problema-especifico.md)
