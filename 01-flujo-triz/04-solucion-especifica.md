# Etapa 4: Solución Específica

## Objetivo

Traducir las soluciones genéricas obtenidas en la [Etapa 3](03-solucion-generica.md) al contexto concreto del problema real. Esta etapa cierra el ciclo del flujo TRIZ.

## Proceso de adaptación

### 4.1 Interpretar cada principio en el contexto

Para cada principio o solución genérica obtenida, preguntarse:

- **¿Qué significaría este principio aplicado a mi sistema concreto?**
- **¿Qué componente del sistema se vería afectado?**
- **¿Qué cambio físico, químico o de diseño implica?**

**Ejemplo**: Si el principio es *#35 Cambio de parámetros físicos/químicos* y el problema es la pintura del barco → cambiar el estado físico de la pintura: usar recubrimiento en polvo (sólido) que se funde al aplicar calor, eliminando la necesidad de disolventes líquidos.

### 4.2 Generar conceptos de solución

Para cada principio relevante, generar al menos una idea concreta. Técnicas útiles:

| Técnica | Descripción |
|---------|------------|
| **Analogía directa** | ¿Cómo se aplica este principio en otros campos? Buscar ejemplos conocidos |
| **Pregunta "¿Y si...?"** | Explorar variantes extremas de la idea |
| **Combinación de principios** | Combinar dos principios en una sola solución |
| **Verificación contra RFI** | ¿Se acerca la idea al Resultado Final Ideal? |

### 4.3 Evaluar las soluciones candidatas

Criterios de evaluación:

| Criterio | Pregunta |
|----------|---------|
| **Resolución de contradicción** | ¿La solución elimina la contradicción o solo la reduce? |
| **Idealidad** | ¿Aumenta la idealidad del sistema (más funciones útiles, menos daño/coste)? |
| **Uso de recursos** | ¿Usa recursos ya existentes o requiere añadir elementos nuevos? |
| **Viabilidad técnica** | ¿Es implementable con la tecnología disponible? |
| **Simplicidad** | ¿Es la solución más simple que logra el objetivo? |
| **Efectos secundarios** | ¿Introduce nuevas contradicciones? Si sí, ¿son resolubles? |

### 4.4 Verificar con las Leyes de Evolución

Comprobar que la solución está alineada con las [Leyes de Evolución](../08-leyes-evolucion/00-vision-general.md):

- ¿La solución **aumenta la idealidad** del sistema? (Ley 4)
- ¿La solución **dinamiza** elementos rígidos? (Ley 8)
- ¿La solución avanza hacia el **micronivel**? (Ley 7)
- ¿La solución mejora la **conductividad energética**? (Ley 2)

Si la solución va *contra* una ley de evolución, es una señal de alerta (aunque no necesariamente invalidante).

## Si la solución no es satisfactoria

```
Solución insatisfactoria
        │
        ├─→ ¿Se exploraron todos los principios sugeridos?
        │     NO → Volver a Etapa 3, explorar más principios
        │
        ├─→ ¿Se formularon múltiples contradicciones?
        │     NO → Volver a Etapa 2, reformular el problema
        │
        ├─→ ¿Se probaron las tres vías (CT, CF, Su-Campo)?
        │     NO → Volver a Etapa 2, probar otra vía
        │
        └─→ Si todo lo anterior se agotó → Escalar a ARIZ-85C
```

## Documentación de la solución

Una vez seleccionada la mejor solución, documentar:

1. **Problema original**: descripción del problema específico.
2. **Contradicción(es) formulada(s)**: CT, CF o modelo Su-Campo.
3. **Herramienta(s) usada(s)**: qué herramienta TRIZ y qué principios.
4. **Solución genérica**: qué principio(s) se aplicaron.
5. **Solución específica**: descripción concreta de la solución.
6. **Evaluación**: cómo resuelve la contradicción, impacto en idealidad.
7. **Nuevas contradicciones** (si las hay): problemas secundarios a resolver.

## Ejemplo completo del flujo (barco)

| Etapa | Resultado |
|-------|-----------|
| **1. Problema específico** | Pintar el casco de un barco es lento y costoso; la pintura debe proteger pero es difícil de aplicar |
| **2. Problema genérico** | CT: Mejorar #13 (estabilidad) empeora #25 (pérdida de tiempo). CF: Pintura debe ser líquida y sólida |
| **3. Solución genérica** | Principio #35: Cambio de parámetros. Separación entre todo/partes |
| **4. Solución específica** | Recubrimiento en polvo electrostático: partículas sólidas (cada parte es sólida) se aplican como nube (el todo se comporta como fluido), luego se funden con calor. Elimina disolventes, reduce tiempo, mejora uniformidad |

---

**Navegación**: [← Etapa 3: Solución genérica](03-solucion-generica.md) · [Los 40 Principios Inventivos →](../02-principios-inventivos/00-indice-principios.md)
