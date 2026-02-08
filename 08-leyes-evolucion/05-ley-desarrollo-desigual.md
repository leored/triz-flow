# Ley 5: Desarrollo Desigual de las Partes del Sistema

## Enunciado

> Las diferentes partes de un sistema técnico evolucionan de forma desigual. Cuanto más
> complejo es el sistema, más desigual es el desarrollo de sus partes. Esta desigualdad
> genera contradicciones que son la fuerza motriz de la evolución del sistema.

Esta es la segunda **ley cinemática**. Complementa la [Ley 4 (Idealidad)](04-ley-idealidad.md)
al explicar **por qué** los sistemas enfrentan límites y necesitan innovación: las partes
no evolucionan al mismo ritmo.

## El problema del eslabón más débil

Un sistema técnico es tan fuerte como su subsistema más débil. Cuando un subsistema
alcanza su límite de rendimiento antes que los demás, se convierte en el **cuello de
botella** que limita todo el sistema:

```
  Rendimiento
      │
      │  Subsistema A  ─────────────────────── (límite alcanzado)
      │                  ╱╱╱╱╱╱╱╱╱╱╱╱╱╱╱╱╱
      │  Subsistema B  ─────────────╱─── (todavía puede crecer)
      │                  ╱╱╱╱╱╱╱╱╱╱
      │  Subsistema C  ───────╱──────── (el que más limita = cuello de botella)
      │                  ╱╱╱╱
      │
      └──────────────────────────────────────→ Tiempo
```

El **rendimiento global del sistema** está determinado por el subsistema C, aunque A y B
tengan capacidad de sobra.

## Curvas S individuales de los subsistemas

Cada subsistema sigue su propia [curva S de evolución](04-ley-idealidad.md). Pero estas
curvas no están sincronizadas:

```
  Rendimiento
      │
      │    Motor                    Transmisión
      │    ╭──────                  ╭──────
      │  ╱─╯                      ╱─╯
      │╱─╯                      ╱─╯
      │╱     Electrónica       ╱
      │      ╭──────         ╱─╯        Batería
      │    ╱─╯             ╱─╯          ╭───
      │  ╱─╯             ╱─╯          ╱─╯
      │╱─╯             ╱─╯          ╱─╯
      │╱             ╱─╯          ╱─╯
      │            ╱─╯          ╱─╯
      └──────────────────────────────────────→ Tiempo
```

En este diagrama, la batería evoluciona más lentamente que los demás subsistemas. Es el
factor limitante del sistema completo.

## Mecanismo de generación de contradicciones

El desarrollo desigual genera dos tipos de contradicciones:

### Contradicción técnica

Mejorar el subsistema limitante empeora otro aspecto del sistema. Por ejemplo: aumentar
la capacidad de la batería incrementa el peso y tamaño del dispositivo. Estas
contradicciones se resuelven con la
[Matriz de Contradicciones](../04-matriz-contradicciones/00-como-usar-la-matriz.md) y los
[40 Principios Inventivos](../02-principios-inventivos/00-indice-principios.md).

### Contradicción física

El subsistema limitante necesita propiedades opuestas simultáneamente. Por ejemplo: la
batería debe ser grande (para almacenar más energía) y pequeña (para caber en un
dispositivo compacto). Estas contradicciones se abordan en
[ARIZ-85C](../07-ariz/00-que-es-ariz.md) mediante separación en tiempo, espacio,
condición o escala.

## Ejemplos de desarrollo desigual

### Ejemplo 1: Smartphone

| Subsistema | Estado evolutivo | Limitación |
|------------|-----------------|------------|
| Procesador | Madurez avanzada | Genera calor excesivo por miniaturización |
| Pantalla | Crecimiento tardío | Resolución ya supera la percepción humana |
| Cámara | Crecimiento | Limitada por tamaño del sensor y óptica |
| **Batería** | **Crecimiento temprano** | **Factor limitante principal**: densidad energética insuficiente |
| Software | Crecimiento | Consume recursos más rápido de lo que el hardware mejora |

La batería es el subsistema que más limita la evolución del smartphone. Esto impulsa
la innovación en tecnologías de baterías, carga rápida y eficiencia energética.

### Ejemplo 2: Aviación comercial

| Subsistema | Estado evolutivo | Limitación |
|------------|-----------------|------------|
| Aerodinámica | Madurez | Cerca del límite teórico para aviones subsónicos |
| Motores | Madurez | Mejoras incrementales en eficiencia de combustible |
| **Materiales** | **Crecimiento** | **Factor limitante**: peso vs. resistencia vs. costo |
| Electrónica de vuelo | Madurez avanzada | Altamente sofisticada y confiable |
| Cabina de pasajeros | Estancamiento | Limitada por decisiones económicas, no técnicas |

Los materiales compuestos (fibra de carbono, etc.) representan el frente actual de
innovación porque son el subsistema que más limita la eficiencia global.

### Ejemplo 3: Energía solar

| Subsistema | Estado evolutivo | Limitación |
|------------|-----------------|------------|
| Panel solar | Crecimiento tardío | Eficiencia cerca del límite de Shockley-Queisser |
| Inversor | Madurez | Eficiencias superiores al 98% |
| **Almacenamiento** | **Nacimiento/Crecimiento** | **Factor limitante principal** |
| Red de distribución | Madurez | Infraestructura establecida pero inflexible |

## Cómo identificar el subsistema limitante

### Método de análisis

1. **Descomponer el sistema** en sus subsistemas principales.
2. Para cada subsistema, determinar su **posición en la curva S**.
3. Identificar cuál subsistema está **más cerca de su límite** o **más lejos del
   rendimiento necesario**.
4. Ese subsistema es el candidato a cuello de botella.
5. Verificar: si se mejorara significativamente ese subsistema, ¿mejoraría
   significativamente el sistema completo?

### Indicadores de que un subsistema es limitante

- Recibe la mayor parte de las quejas de usuarios.
- Genera la mayoría de los fallos del sistema.
- Es el que tiene más patentes recientes (muchos inventores intentan mejorarlo).
- Es el que los competidores intentan diferenciar.

## Estrategias para abordar el desarrollo desigual

1. **Mejorar el subsistema limitante**: Invertir recursos en el cuello de botella.
   Usar [soluciones estándar](../06-soluciones-estandar/01-clase-1-construir.md) específicas.

2. **Compensar con otros subsistemas**: Si el limitante no puede mejorarse, hacer que
   otros subsistemas compensen. Ejemplo: si la batería no mejora, optimizar el consumo
   energético del software.

3. **Rediseñar la arquitectura**: Cambiar cómo se relacionan los subsistemas para
   que el limitante deje de ser crítico. Esto conecta con la
   [Ley 6 (Transición a supersistema)](06-ley-transicion-supersistema.md).

4. **Sustituir el principio de funcionamiento**: Reemplazar el subsistema limitante
   por uno basado en un principio diferente (nueva curva S). Ejemplo: sustituir
   batería de litio por celda de combustible de hidrógeno.

## Conexión con otras herramientas TRIZ

- **Análisis Su-Campo**: Modelar el subsistema limitante como un
  [modelo Su-Campo incompleto o ineficiente](../05-analisis-su-campo/02-modelos-basicos.md)
  ayuda a encontrar soluciones específicas.
- **ARIZ-85C**: La [Parte 1 de ARIZ](../07-ariz/01-parte-1-analisis.md) comienza
  identificando el conflicto, que frecuentemente se origina en el desarrollo desigual.
- **Principio 3 (Calidad local)**: Optimizar cada parte independientemente según su
  estado evolutivo.

---

**Navegación**: [← Ley 4](04-ley-idealidad.md) · [Ley 6: Transición a supersistema →](06-ley-transicion-supersistema.md)
