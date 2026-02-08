# Ley 2: Conductividad Energética a Través del Sistema

## Enunciado

> Una condición necesaria para la viabilidad de un sistema técnico es el paso libre de
> energía a través de todas sus partes: desde el motor, a través de la transmisión,
> hasta la herramienta de trabajo.

Esta es la segunda **ley estática**. Mientras que la [Ley 1](01-ley-completitud.md)
exige que las cuatro partes estén presentes, esta ley exige que estén **conectadas
energéticamente** de forma efectiva.

## Principio fundamental

La energía debe fluir sin interrupciones ni pérdidas excesivas desde su fuente hasta
el punto donde se realiza la función útil:

```
   Fuente de       Transmisión        Herramienta
    energía         de energía         de trabajo
  ┌─────────┐    ┌──────────────┐    ┌──────────────┐
  │  MOTOR  │══E═▶│ TRANSMISIÓN  │══E═▶│ HERRAMIENTA  │══E═▶ OBJETO
  └─────────┘    └──────────────┘    └──────────────┘

  E = flujo de energía (debe ser continuo y eficiente)
```

Cualquier **bloqueo, fuga o transformación ineficiente** en esta cadena reduce la
efectividad del sistema y puede hacerlo no viable.

## Tipos de conductividad energética

### Conductividad de materia
Transferencia de material de un punto a otro: tuberías, transportadores, canales.

### Conductividad de energía mecánica
Engranajes, palancas, ejes, correas, resortes, transmisiones hidráulicas.

### Conductividad de energía térmica
Conducción, convección y radiación a través de materiales y medios.

### Conductividad de energía eléctrica
Cables, circuitos, semiconductores, campos electromagnéticos.

### Conductividad de información
Señales, datos, retroalimentación entre el órgano de control y las demás partes.

## Diagnóstico: conductividad deficiente vs. eficiente

| Aspecto | Conductividad deficiente | Conductividad eficiente |
|---------|--------------------------|-------------------------|
| Pérdidas | Altas pérdidas por fricción, calor, vibración | Pérdidas minimizadas |
| Transformaciones | Múltiples conversiones de energía innecesarias | Mínimas conversiones, las necesarias son eficientes |
| Bloqueos | Puntos de estrangulamiento en la cadena | Flujo libre sin restricciones |
| Adaptación | Impedancias desacopladas entre componentes | Impedancias coincidentes entre componentes |
| Distancia | Largas distancias de transmisión | Distancias mínimas o transmisión directa |

## Ejemplos prácticos

### Ejemplo 1: Sistema de calefacción

**Mala conductividad**: Caldera central con tuberías largas sin aislar. La energía térmica
se pierde en el trayecto. Al llegar a las habitaciones distantes, el agua ya está tibia.

**Buena conductividad**: Tuberías aisladas, circuitos zonificados, bomba de recirculación.
La energía térmica llega eficientemente a cada zona.

### Ejemplo 2: Taladro eléctrico

**Mala conductividad**: Motor potente, pero engranajes desgastados y mandril flojo. La
energía del motor se pierde en vibración y calor. La broca no recibe suficiente torque.

**Buena conductividad**: Engranajes precisos, mandril de sujeción firme. La energía
mecánica fluye del motor a la broca con mínimas pérdidas.

### Ejemplo 3: Comunicación en una organización

**Mala conductividad**: La información (energía informacional) pasa por 7 niveles
jerárquicos. Cada nivel distorsiona y retrasa el mensaje.

**Buena conductividad**: Canales directos entre quien genera la información y quien la
necesita. La señal llega íntegra y a tiempo.

## Tendencias evolutivas de la conductividad

Los sistemas evolucionan mejorando su conductividad energética siguiendo este patrón:

```
Conductividad          Conductividad         Conductividad        Transmisión
  mecánica    ───→      hidráulica    ───→     eléctrica    ───→   por campos
 (contacto)           (fluido medio)         (electrones)        (sin medio)
```

### Patrón general de mejora

1. **Eliminar intermediarios**: Reducir el número de eslabones en la cadena de transmisión.
   Esto se conecta con el [Principio 25: Autoservicio](../02-principios-inventivos/00-indice-principios.md).

2. **Sustituir el tipo de energía**: Cambiar a formas de energía más fáciles de transmitir
   y controlar. La energía eléctrica y los campos son más controlables que la mecánica.

3. **Usar campos en lugar de sustancias**: La transmisión por campos electromagnéticos,
   acústicos o térmicos elimina la necesidad de contacto físico y reduce pérdidas.

4. **Acercar la fuente al punto de acción**: Minimizar la distancia de transmisión.
   Idealmente, el motor está integrado en la herramienta de trabajo.

## Conexión con otras herramientas TRIZ

### Análisis Su-Campo

En el [modelo Su-Campo](../05-analisis-su-campo/02-modelos-basicos.md), el campo
representa la energía que conecta las sustancias. Un campo inadecuado o insuficiente
es un problema de conductividad energética. Las
[soluciones estándar](../06-soluciones-estandar/01-clase-1-construir.md) para modelos Su-Campo
ineficientes frecuentemente abordan problemas de conductividad.

### ARIZ-85C

Durante el [análisis de recursos en ARIZ](../07-ariz/04-parte-4-recursos.md), identificar
las vías de transmisión de energía es fundamental para encontrar recursos disponibles
en la zona del conflicto.

## Aplicación práctica

Para mejorar la conductividad energética de un sistema:

1. Trace el **mapa completo del flujo de energía** desde la fuente hasta el punto de acción.
2. Identifique cada **transformación y transferencia** en la cadena.
3. Mida o estime las **pérdidas en cada eslabón**.
4. Busque eliminar eslabones innecesarios, sustituir tipos de energía o acortar distancias.
5. Verifique que la mejora no genere nuevas contradicciones (use la
   [Matriz de Contradicciones](../04-matriz-contradicciones/00-como-usar-la-matriz.md) si es necesario).

---

**Navegación**: [← Ley 1](01-ley-completitud.md) · [Ley 3: Coordinación →](03-ley-coordinacion.md)
