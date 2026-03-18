# TRIZ Flow

> **Teoría para Resolver Problemas de Inventiva**
> Genrich Altshuller, 1946–1998

Referencia completa del método TRIZ en español + sistema de dinámicas interactivas para analizar problemas técnicos con Claude Code.

Un facilitador orquesta el análisis aplicando distintas "lentes TRIZ" en rondas secuenciales. Expertos de distintos dominios aportan perspectivas diversas — alineado con el principio TRIZ de que las mejores soluciones vienen de otros campos.

## Inicio rápido

```bash
# 1. Crear un reto
/new-challenge reducir-friccion-en-rodamientos

# 2. Editar challenges/reducir-friccion-en-rodamientos/00-challenge.md
#    con la descripción del problema técnico

# 3. Crear expertos de distintos dominios
/create-expert bióloga marina con 20 años en biomimética
/create-expert ingeniero aeronáutico especialista en tribología

# 4. Ejecutar la sesión — el facilitador elige las lentes TRIZ apropiadas
/run-session reducir-friccion-en-rodamientos
```

### Lentes TRIZ disponibles

| Agente | Lente | Qué hace |
|--------|-------|----------|
| `@analista` | Análisis de sistemas | Descompone componentes, funciones, contradicciones y recursos |
| `@principios` | 40 Principios + Matriz | Consulta la Matriz de Contradicciones y genera ideas concretas |
| `@su-campo` | Sustancia-Campo | Modela interacciones S1-S2-F y aplica las 76 soluciones estándar |
| `@evolucion` | Leyes de evolución | Evalúa estado evolutivo y predice dirección de desarrollo |
| `@idealidad` | RFI e Idealidad | Empuja soluciones hacia la máxima idealidad explotando recursos |
| `@facilitador` | Orquestador | Elige la secuencia de lentes y sintetiza resultados |

### Secuencias según tipo de problema

| Tipo de problema | Secuencia |
|-----------------|-----------|
| Contradicción técnica clara | Analista → Principios → Idealidad |
| Contradicción física | Analista → Principios (separación) → Idealidad |
| Problema de interacción | Analista → Su-Campo → Idealidad |
| Exploración completa | Analista → Principios → Su-Campo → Evolución → Idealidad |
| Predicción tecnológica | Analista → Evolución → Idealidad |

---

## Referencia del método TRIZ

### 00 · Fundamentos

- [¿Qué es TRIZ?](00-fundamentos/01-que-es-triz.md) — Introducción, pilares, cuándo usar TRIZ
- [Historia de Altshuller](00-fundamentos/02-historia-altshuller.md) — Biografía, estudio de patentes, cronología
- [Conceptos clave](00-fundamentos/03-conceptos-clave.md) — Contradicciones, RFI, recursos, niveles inventivos

### 01 · Flujo del método TRIZ

- [Visión general del flujo](01-flujo-triz/00-vision-general.md) — Diagrama del flujo + mapa de decisión
- [Etapa 1: Problema específico](01-flujo-triz/01-problema-especifico.md) — Definir el problema concreto
- [Etapa 2: Problema genérico](01-flujo-triz/02-problema-generico.md) — Reformular como modelo TRIZ
- [Etapa 3: Solución genérica](01-flujo-triz/03-solucion-generica.md) — Aplicar herramientas TRIZ
- [Etapa 4: Solución específica](01-flujo-triz/04-solucion-especifica.md) — Adaptar al caso concreto

### 02 · Los 40 Principios Inventivos

- [Índice de los 40 principios](02-principios-inventivos/00-indice-principios.md) — Tabla resumen

| | | | |
|---|---|---|---|
| [01 Segmentación](02-principios-inventivos/01-segmentacion.md) | [11 Amortiguación previa](02-principios-inventivos/11-amortiguacion-previa.md) | [21 Saltar rápido](02-principios-inventivos/21-saltar-rapido.md) | [31 Material poroso](02-principios-inventivos/31-material-poroso.md) |
| [02 Extracción](02-principios-inventivos/02-extraccion.md) | [12 Equipotencialidad](02-principios-inventivos/12-equipotencialidad.md) | [22 Convertir daño en beneficio](02-principios-inventivos/22-convertir-dano-en-beneficio.md) | [32 Cambio de color](02-principios-inventivos/32-cambio-de-color.md) |
| [03 Calidad local](02-principios-inventivos/03-calidad-local.md) | [13 Inversión](02-principios-inventivos/13-inversion.md) | [23 Retroalimentación](02-principios-inventivos/23-retroalimentacion.md) | [33 Homogeneidad](02-principios-inventivos/33-homogeneidad.md) |
| [04 Asimetría](02-principios-inventivos/04-asimetria.md) | [14 Esferoidalidad](02-principios-inventivos/14-esferoidalidad.md) | [24 Mediador](02-principios-inventivos/24-mediador.md) | [34 Descarte y recuperación](02-principios-inventivos/34-descarte-y-recuperacion.md) |
| [05 Combinación](02-principios-inventivos/05-combinacion.md) | [15 Dinamización](02-principios-inventivos/15-dinamizacion.md) | [25 Autoservicio](02-principios-inventivos/25-autoservicio.md) | [35 Cambio de parámetros](02-principios-inventivos/35-cambio-de-parametros.md) |
| [06 Universalidad](02-principios-inventivos/06-universalidad.md) | [16 Acción parcial o excesiva](02-principios-inventivos/16-accion-parcial-o-excesiva.md) | [26 Copia](02-principios-inventivos/26-copia.md) | [36 Transición de fase](02-principios-inventivos/36-transicion-de-fase.md) |
| [07 Anidamiento](02-principios-inventivos/07-anidamiento.md) | [17 Cambio de dimensión](02-principios-inventivos/17-cambio-de-dimension.md) | [27 Objeto económico desechable](02-principios-inventivos/27-objeto-economico-desechable.md) | [37 Expansión térmica](02-principios-inventivos/37-expansion-termica.md) |
| [08 Contrapeso](02-principios-inventivos/08-contrapeso.md) | [18 Vibración mecánica](02-principios-inventivos/18-vibracion-mecanica.md) | [28 Reemplazo mecánico](02-principios-inventivos/28-reemplazo-mecanico.md) | [38 Oxidantes fuertes](02-principios-inventivos/38-oxidantes-fuertes.md) |
| [09 Acción previa](02-principios-inventivos/09-accion-previa.md) | [19 Acción periódica](02-principios-inventivos/19-accion-periodica.md) | [29 Neumática e hidráulica](02-principios-inventivos/29-neumatica-e-hidraulica.md) | [39 Atmósfera inerte](02-principios-inventivos/39-atmosfera-inerte.md) |
| [10 Acción anticipada](02-principios-inventivos/10-accion-anticipada.md) | [20 Continuidad de acción útil](02-principios-inventivos/20-continuidad-de-accion-util.md) | [30 Membranas flexibles](02-principios-inventivos/30-membranas-flexibles.md) | [40 Materiales compuestos](02-principios-inventivos/40-materiales-compuestos.md) |

### 03 · Los 39 Parámetros de Ingeniería

- [Índice de parámetros](03-parametros-ingenieria/00-indice-parametros.md) — Tabla resumen
- [Descripción completa](03-parametros-ingenieria/parametros.md) — Todos los parámetros detallados

### 04 · Matriz de Contradicciones

- [Cómo usar la Matriz](04-matriz-contradicciones/00-como-usar-la-matriz.md) — Guía de uso + ejemplo resuelto
- [Parámetros 01–08](04-matriz-contradicciones/01-matriz-mejora-01-08.md)
- [Parámetros 09–16](04-matriz-contradicciones/02-matriz-mejora-09-16.md)
- [Parámetros 17–24](04-matriz-contradicciones/03-matriz-mejora-17-24.md)
- [Parámetros 25–31](04-matriz-contradicciones/04-matriz-mejora-25-31.md)
- [Parámetros 32–39](04-matriz-contradicciones/05-matriz-mejora-32-39.md)

### 05 · Análisis Sustancia-Campo (Su-Campo)

- [Fundamentos Su-Campo](05-analisis-su-campo/01-fundamentos-su-campo.md) — Teoría S1, S2, F
- [Modelos básicos](05-analisis-su-campo/02-modelos-basicos.md) — Completo, incompleto, dañino, insuficiente
- [Transformaciones](05-analisis-su-campo/03-transformaciones.md) — Reglas de transformación
- [Notación y diagramas](05-analisis-su-campo/04-notacion-diagramas.md) — Notación textual

### 06 · Las 76 Soluciones Estándar

- [Índice de soluciones](06-soluciones-estandar/00-indice-soluciones.md) — Tabla resumen
- [Clase 1: Construir/destruir modelos Su-Campo](06-soluciones-estandar/01-clase-1-construir.md) — 13 soluciones
- [Clase 2: Desarrollar modelos Su-Campo](06-soluciones-estandar/02-clase-2-desarrollar.md) — 23 soluciones
- [Clase 3: Transición a supersistema y micronivel](06-soluciones-estandar/03-clase-3-transicion.md) — 6 soluciones
- [Clase 4: Detección y medición](06-soluciones-estandar/04-clase-4-deteccion.md) — 17 soluciones
- [Clase 5: Estrategias de simplificación](06-soluciones-estandar/05-clase-5-estrategias.md) — 17 soluciones

### 07 · ARIZ-85C

- [¿Qué es ARIZ?](07-ariz/00-que-es-ariz.md) — Descripción y cuándo usarlo
- [Parte 1: Análisis del problema](07-ariz/01-parte-1-analisis.md)
- [Parte 2: Análisis del modelo del problema](07-ariz/02-parte-2-modelo.md)
- [Parte 3: Definición del RFI](07-ariz/03-parte-3-rfi.md)
- [Parte 4: Movilización de recursos](07-ariz/04-parte-4-recursos.md)
- [Parte 5: Aplicación de la base de conocimientos](07-ariz/05-parte-5-conocimientos.md)
- [Parte 6: Cambio o reformulación del problema](07-ariz/06-parte-6-reformulacion.md)
- [Parte 7: Análisis de la solución](07-ariz/07-parte-7-solucion.md)
- [Parte 8: Uso máximo de la solución](07-ariz/08-parte-8-uso-maximo.md)
- [Parte 9: Análisis del proceso de solución](07-ariz/09-parte-9-proceso.md)

### 08 · Las 8 Leyes de Evolución de Sistemas Técnicos

- [Visión general](08-leyes-evolucion/00-vision-general.md) — Las 8 leyes como sistema
- [Ley 1: Completitud de partes](08-leyes-evolucion/01-ley-completitud.md)
- [Ley 2: Conductividad energética](08-leyes-evolucion/02-ley-conductividad.md)
- [Ley 3: Coordinación de ritmos](08-leyes-evolucion/03-ley-coordinacion.md)
- [Ley 4: Aumento de idealidad](08-leyes-evolucion/04-ley-idealidad.md)
- [Ley 5: Desarrollo desigual](08-leyes-evolucion/05-ley-desarrollo-desigual.md)
- [Ley 6: Transición a supersistema](08-leyes-evolucion/06-ley-transicion-supersistema.md)
- [Ley 7: Transición a micronivel](08-leyes-evolucion/07-ley-transicion-micronivel.md)
- [Ley 8: Aumento de dinamismo](08-leyes-evolucion/08-ley-dinamizacion.md)

### 09 · Recursos

- [Bibliografía](09-recursos/01-bibliografia.md) — Libros, artículos, recursos online
- [Glosario ES/EN/RU](09-recursos/02-glosario.md) — Términos con definiciones
- [Guía rápida](09-recursos/03-guia-rapida.md) — Cheat sheet de referencia

---

> Referencia del método TRIZ clásico de Altshuller + dinámicas interactivas con Claude Code.
> Contenido en español. Compatible con GitHub y Obsidian.
