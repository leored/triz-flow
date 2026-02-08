# Etapa 1: Problema Específico

## Objetivo

Comprender profundamente la situación real antes de abstraerla. Esta etapa transforma una situación problemática vaga en una formulación precisa que pueda traducirse a un modelo TRIZ.

## Actividades clave

### 1.1 Describir el sistema

Identificar los componentes del sistema y sus relaciones:

- **¿Cuál es la función principal del sistema?** (verbo + objeto + resultado)
- **¿Cuáles son los subsistemas?** (componentes internos)
- **¿Cuál es el supersistema?** (entorno, usuario, sistemas adyacentes)
- **¿Qué funciones útiles realiza el sistema?**
- **¿Qué funciones dañinas produce el sistema?**

### 1.2 Identificar el problema

Definir con precisión qué se quiere lograr y qué lo impide:

- **Situación deseada**: ¿Cómo debería funcionar el sistema?
- **Situación actual**: ¿Qué falla o es insatisfactorio?
- **Brecha**: ¿Cuál es la diferencia entre lo deseado y lo actual?
- **Restricciones**: ¿Qué no se puede cambiar? (coste, normativa, materiales disponibles)

### 1.3 Análisis funcional

Listar todas las funciones del sistema en formato:

```
[Componente] → [acción] → [objeto de la acción]
```

Clasificar cada función como:

| Tipo | Descripción |
|------|------------|
| **Útil** | Contribuye a la función principal |
| **Dañina** | Produce un efecto negativo |
| **Insuficiente** | Cumple su función, pero no al nivel requerido |
| **Excesiva** | Cumple su función, pero en exceso |
| **Ausente** | Función necesaria que no existe en el sistema actual |

### 1.4 Identificar contradicciones

Buscar los conflictos inherentes al problema:

**Para contradicciones técnicas**:
- "Si hago [acción] para mejorar [parámetro A], entonces empeora [parámetro B]"
- Puede haber más de una contradicción; listarlas todas.

**Para contradicciones físicas**:
- "El elemento [X] debe ser [propiedad A] para [función 1] y debe ser [propiedad opuesta] para [función 2]"

### 1.5 Inventario de recursos

Catalogar los recursos disponibles antes de buscar soluciones externas:

| Categoría | Preguntas guía |
|-----------|---------------|
| Sustancias | ¿Qué materiales hay en el sistema y su entorno? ¿Hay residuos o subproductos? |
| Campos/Energías | ¿Qué energías están presentes? ¿Hay calor, vibración, campos electromagnéticos? |
| Espacio | ¿Hay espacio libre dentro del sistema? ¿Se aprovechan todas las superficies? |
| Tiempo | ¿Hay tiempos muertos? ¿Se puede hacer algo antes o después del proceso? |
| Información | ¿Hay datos o señales no utilizados? |
| Funciones | ¿Algún componente puede hacer algo adicional sin coste significativo? |

## Ejemplo: Pintura de un barco

**Situación**: Pintar el casco de un barco grande es lento y costoso. La pintura debe proteger contra la corrosión, pero la aplicación manual requiere andamios, tiempo de secado, y genera emisiones de disolventes.

**Análisis**:
- **Función principal**: Proteger el casco de la corrosión marina.
- **Subsistemas**: Pintura, brocha/rodillo/pistola, andamios, operarios.
- **Supersistema**: Astillero, agua de mar, atmósfera.
- **Contradicción técnica**: Si aumento el espesor de la pintura (mejora la protección), aumento el tiempo y coste de aplicación.
- **Contradicción física**: La pintura debe ser líquida (para aplicarse) y sólida (para proteger).
- **Recursos disponibles**: Agua de mar (sustancia), corrientes marinas (campo), superficie del casco (espacio), tiempo en dique seco (tiempo).

## Errores comunes en esta etapa

| Error | Consecuencia | Corrección |
|-------|-------------|-----------|
| Definir la solución en vez del problema | Se pierde la oportunidad de encontrar mejores soluciones | Formular como "necesito que..." no como "necesito un..." |
| Ignorar el supersistema | Se pierden recursos y contexto | Siempre incluir el entorno en el análisis |
| Aceptar restricciones sin cuestionarlas | Se limita artificialmente el espacio de soluciones | Verificar si cada restricción es real o asumida |
| Conformarse con una sola contradicción | Se puede estar resolviendo el problema equivocado | Listar todas las contradicciones y priorizar |

---

**Navegación**: [← Visión general](00-vision-general.md) · [Etapa 2: Problema genérico →](02-problema-generico.md)
