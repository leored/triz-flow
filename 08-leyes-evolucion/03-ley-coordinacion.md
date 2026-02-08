# Ley 3: Coordinación de Ritmos de las Partes del Sistema

## Enunciado

> Una condición necesaria para la viabilidad de un sistema técnico es la coordinación
> de los ritmos (frecuencias, periodicidades, frecuencias naturales) de todas las partes
> del sistema.

Esta es la tercera y última **ley estática**. Completa el trío de condiciones de
viabilidad: las partes deben estar presentes ([Ley 1](01-ley-completitud.md)), conectadas
energéticamente ([Ley 2](02-ley-conductividad.md)) y **sincronizadas en sus ritmos**.

## Concepto de "ritmo" en sistemas técnicos

El término "ritmo" abarca todas las características temporales y frecuenciales de un
componente o proceso:

- **Frecuencias de operación**: RPM de un motor, ciclos por segundo de una bomba.
- **Frecuencias naturales**: frecuencia de resonancia de una estructura o componente.
- **Periodicidades**: ciclos de trabajo, intervalos de mantenimiento, tiempos de proceso.
- **Velocidades**: velocidad lineal, angular, de flujo, de reacción.
- **Ritmos biológicos**: cuando el ser humano es parte del sistema.

## Efectos de la descoordinación

```
    Ritmos              Ritmos              Ritmos en
  descoordinados     coordinados          resonancia
       ↓                  ↓                   ↓
  ┌──────────┐      ┌──────────┐       ┌──────────┐
  │ Pérdida  │      │ Operación│       │ Máxima   │
  │ de       │ ───→ │ eficiente│  ───→ │ eficiencia│
  │ energía, │      │ y estable│       │ (o máxima │
  │ desgaste,│      │          │       │ destrucción│
  │ fallo    │      │          │       │ si no se  │
  └──────────┘      └──────────┘       │ controla) │
                                       └──────────┘
```

### Descoordinación: consecuencias negativas

- **Vibraciones destructivas**: cuando frecuencias no coinciden y generan interferencias.
- **Desgaste prematuro**: componentes forzados a operar fuera de su ritmo óptimo.
- **Pérdida de eficiencia**: energía desperdiciada en compensar la desincronización.
- **Fatiga del material**: ciclos de carga a frecuencias cercanas a la resonancia natural.
- **Fatiga del operador**: cuando los ritmos de la máquina no coinciden con los humanos.

### Coordinación: beneficios

- **Operación suave**: sin vibraciones ni picos de carga.
- **Máxima transferencia de energía**: cada componente opera en su punto óptimo.
- **Mayor vida útil**: menos desgaste y fatiga.
- **Ergonomía**: el sistema se adapta a los ritmos humanos.

## Ejemplos prácticos

### Ejemplo 1: Caja de cambios de un automóvil

El motor de combustión opera eficientemente en un rango estrecho de RPM (por ejemplo,
2000-4000 RPM). Las ruedas necesitan girar a velocidades muy diferentes según la
velocidad del vehículo. La caja de cambios **coordina estos dos ritmos**: adapta las RPM
del motor a la velocidad requerida por las ruedas. Sin esta coordinación, el motor se
calaría o las ruedas patinarían.

### Ejemplo 2: Instrumentos musicales

Una guitarra coordina múltiples ritmos: la frecuencia de vibración de la cuerda debe
coincidir con la frecuencia de resonancia de la caja acústica. Cuando están coordinadas,
el sonido se amplifica. Cuando no, el instrumento suena apagado o distorsionado.

### Ejemplo 3: Línea de producción

En una fábrica, cada estación de trabajo tiene su propio ritmo de procesamiento. Si la
estación de pintura tarda 5 minutos pero la de ensamblaje tarda 2, se genera un cuello
de botella. La **coordinación de ritmos** requiere equilibrar los tiempos de cada etapa
o usar buffers intermedios.

### Ejemplo 4: Microondas

La frecuencia de las microondas (2.45 GHz) está coordinada con la frecuencia de
resonancia de las moléculas de agua. Esta coordinación permite la máxima absorción de
energía por el agua contenida en los alimentos.

## Niveles de coordinación

La evolución de la coordinación de ritmos sigue una progresión:

| Nivel | Descripción | Ejemplo |
|-------|-------------|---------|
| 0. Sin coordinación | Cada parte opera independientemente | Motor sin caja de cambios conectado a las ruedas |
| 1. Coordinación fija | Ritmos ajustados una vez en el diseño | Engranaje de relación fija |
| 2. Coordinación ajustable | Ritmos ajustables por el operador | Caja de cambios manual |
| 3. Coordinación automática | El sistema ajusta ritmos solo | Transmisión automática |
| 4. Coordinación adaptativa | El sistema predice y se anticipa | Transmisión CVT con IA predictiva |

## Resonancia: coordinación extrema

La resonancia ocurre cuando los ritmos de dos componentes coinciden exactamente. Puede ser:

- **Beneficiosa**: máxima transferencia de energía (ejemplo: microondas, resonancia
  magnética en medicina).
- **Destructiva**: acumulación de energía hasta el fallo (ejemplo: puente de Tacoma,
  copa de cristal rota por sonido).

El ingeniero debe decidir si **buscar la resonancia** (para maximizar eficiencia) o
**evitarla** (para prevenir destrucción), lo cual frecuentemente genera una
**contradicción técnica** resoluble con la
[Matriz de Contradicciones](../04-matriz-contradicciones/00-como-usar-la-matriz.md).

## Conexión con otras herramientas TRIZ

- **Principio 19 (Acción periódica)**: Sugiere pasar de acción continua a periódica y
  ajustar la frecuencia. Es una aplicación directa de coordinación de ritmos.
- **Principio 18 (Vibración mecánica)**: Usar vibraciones a frecuencias coordinadas
  con el sistema.
- **Análisis Su-Campo**: Los [campos oscilantes](../05-analisis-su-campo/02-modelos-basicos.md)
  en modelos Su-Campo deben estar coordinados con las frecuencias naturales de las sustancias.
- **ARIZ**: En la [Parte 5 de ARIZ](../07-ariz/05-parte-5-conocimientos.md), la búsqueda
  de analogías puede revelar soluciones de coordinación de ritmos en otros dominios.

## Aplicación práctica

Para mejorar la coordinación de ritmos en un sistema:

1. **Identifique los ritmos** de cada componente (frecuencias, velocidades, ciclos).
2. **Detecte descoordinaciones**: donde un componente opera fuera de sincronía con otros.
3. **Determine si la solución es sincronizar o desincronizar** (evitar resonancias
   destructivas o buscar resonancias beneficiosas).
4. **Elija el nivel de coordinación** apropiado (fija, ajustable, automática, adaptativa).
5. **Implemente** usando los principios inventivos relevantes (18, 19, 20) y las
   [soluciones estándar](../06-soluciones-estandar/01-clase-1-construir.md) correspondientes.

---

**Navegación**: [← Ley 2](02-ley-conductividad.md) · [Ley 4: Idealidad →](04-ley-idealidad.md)
