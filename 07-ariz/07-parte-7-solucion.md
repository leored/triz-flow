# Parte 7: Analisis de la solucion

> **Objetivo**: Verificar la calidad de la solucion obtenida, evaluar si satisface el Resultado Final Ideal, identificar sub-problemas secundarios y registrarlos para iteraciones futuras.

La Parte 7 marca la transicion del proceso de busqueda al proceso de evaluacion. Una solucion no esta completa hasta que pasa por esta verificacion rigurosa. Altshuller observo que muchos inventores aceptan la primera solucion que aparece sin evaluarla criticamente, lo que lleva a soluciones debiles.

---

## Paso 7.1: Verificacion preliminar contra el RFI

Comparar la solucion obtenida con el Resultado Final Ideal formulado en la Parte 3.

### Lista de verificacion

| Criterio | Pregunta | Si/No |
|----------|----------|:-----:|
| Funcion util | *La solucion proporciona la funcion util principal requerida?* | |
| Contradiccion fisica | *La solucion resuelve la CF (no solo la reduce o la oculta)?* | |
| Efectos daninos | *La solucion introduce nuevos efectos daninos significativos?* | |
| Complejidad | *La solucion es mas simple o mas compleja que el sistema original?* | |
| Recursos | *La solucion utiliza recursos ya existentes o requiere nuevos?* | |
| Controlabilidad | *La solucion es controlable y predecible?* | |
| Proximidad al RFI | *En que medida se acerca al RFI formulado en el paso 3.1?* | |

### Evaluacion de la idealidad

Calcular cualitativamente la idealidad de la solucion:

```
                 Funciones utiles obtenidas
Idealidad = ─────────────────────────────────────────
             Funciones daninas + costes + complejidad
```

La solucion ideal:
- **Maximiza** las funciones utiles.
- **Minimiza** las funciones daninas, los costes y la complejidad.
- No introduce nuevos elementos al sistema (o los minimos posibles).

### Que hacer si la solucion no satisface el RFI

- Si la solucion es parcial pero prometedora: documentarla y buscar como completarla.
- Si la solucion introduce nuevos problemas graves: tratarlos como sub-problemas (paso 7.2).
- Si la solucion es claramente insatisfactoria: volver a la [Parte 6](06-parte-6-reformulacion.md) para reformular.

---

## Paso 7.2: Identificar sub-problemas de la nueva solucion

Toda solucion nueva genera sub-problemas. Este paso consiste en identificarlos y evaluar si son resolubles.

### Tipos de sub-problemas

1. **Sub-problemas tecnicos**: *Como implementar fisicamente la solucion? Que tecnologia se necesita?*
2. **Sub-problemas de compatibilidad**: *La solucion es compatible con el resto del sistema? Con el supersistema?*
3. **Sub-problemas de fabricacion**: *Se puede fabricar/implementar con los medios disponibles?*
4. **Sub-problemas de efecto secundario**: *Que nuevos efectos daninos aparecen?*
5. **Sub-problemas economicos**: *El costo de implementacion es aceptable?*

### Evaluacion de los sub-problemas

Para cada sub-problema identificado:

| Sub-problema | Gravedad (1-5) | Resoluble con herramientas TRIZ simples | Requiere nuevo ciclo ARIZ |
|--------------|:--------------:|:---------------------------------------:|:-------------------------:|
| (describir) | | Si/No | Si/No |

- Si todos los sub-problemas son resolubles con herramientas simples ([Matriz](../04-matriz-contradicciones/00-como-usar-la-matriz.md), [Principios](../02-principios-inventivos/00-indice-principios.md), [Soluciones Estandar](../06-soluciones-estandar/00-indice-soluciones.md)): la solucion es viable.
- Si algun sub-problema requiere un nuevo ciclo de ARIZ: registrarlo como problema independiente para una iteracion futura.
- Si un sub-problema es irresolubles y critico: la solucion puede no ser viable; considerar volver a la [Parte 6](06-parte-6-reformulacion.md).

---

## Paso 7.3: Verificar contra patentes y soluciones conocidas

Antes de aceptar la solucion como definitiva, verificar:

### Busqueda de antecedentes

1. *Existe ya una patente que cubra esta solucion o una muy similar?*
2. *Se ha publicado esta solucion en la literatura tecnica o cientifica?*
3. *Otros campos de la ingenieria ya usan este principio?*

### Proposito

- **Evitar reinventar**: si la solucion ya existe, se puede aprender de las implementaciones existentes.
- **Validar el principio**: si la solucion ya ha sido patentada y comercializada, es una validacion indirecta de su viabilidad.
- **Identificar mejoras**: las patentes existentes a menudo revelan limitaciones que pueden superarse.
- **Proteger la propiedad intelectual**: si la solucion es nueva, evaluar su patentabilidad.

### Fuentes de verificacion

- Bases de datos de patentes (nacionales e internacionales).
- Literatura tecnica y cientifica del campo.
- Bases de datos de soluciones TRIZ y casos de estudio.
- Consulta con expertos del dominio.

---

## Paso 7.4: Registrar todas las sub-tareas generadas

Documentar sistematicamente todos los sub-problemas y tareas secundarias generados durante el proceso de solucion.

### Que registrar

1. **Sub-problemas no resueltos**: problemas identificados en el paso 7.2 que requieren iteraciones futuras.
2. **Variantes de solucion descartadas**: soluciones parciales encontradas en las Partes 1-5 que no se desarrollaron completamente pero que podrian ser utiles en otros contextos.
3. **Problemas del supersistema**: cambios necesarios en el supersistema para que la solucion funcione.
4. **Informacion faltante**: datos tecnicos o cientificos que se necesitarian para completar la solucion.

### Formato recomendado

| # | Sub-tarea | Origen (paso) | Prioridad | Estado |
|:-:|-----------|:-------------:|:---------:|--------|
| 1 | (describir) | (ej: 7.2) | Alta/Media/Baja | Pendiente |
| 2 | ... | ... | ... | ... |

Este registro es fundamental para el trabajo posterior. ARIZ no es un proceso que se aplica una sola vez: los sub-problemas registrados aqui se convierten en los problemas de entrada para futuras aplicaciones del algoritmo.

---

## Resumen de la Parte 7

| Paso | Accion | Resultado |
|:----:|--------|-----------|
| 7.1 | Verificar contra el RFI | Evaluacion de idealidad de la solucion |
| 7.2 | Identificar sub-problemas | Lista de problemas secundarios y su resolubilidad |
| 7.3 | Verificar antecedentes | Comparacion con patentes y literatura |
| 7.4 | Registrar sub-tareas | Documentacion para iteraciones futuras |

---

**Navegacion**: [<< Parte 6](06-parte-6-reformulacion.md) · [Parte 8 >>](08-parte-8-uso-maximo.md)
