# Guia rapida TRIZ — Hoja de referencia

Referencia compacta de las herramientas principales de TRIZ.

---

## Flujo TRIZ

```
Problema           Problema            Solución            Solución
específico    -->  genérico       -->  genérica       -->  específica
    |                  |                   |                   |
 Mi problema     Contradicción /     Principio /         Diseño
 concreto        Modelo Su-Campo     Estándar / ARIZ     adaptado
```

---

## Cuándo usar cada herramienta

| Situación | Herramienta | Referencia |
|---|---|---|
| Sé qué parámetro mejora y cuál empeora | **Matriz de contradicciones** | [Matriz](../04-matriz-contradicciones/00-como-usar-la-matriz.md) |
| Un parámetro necesita dos valores opuestos | **Principios de separación** (CF) | [Contradicciones](../00-fundamentos/03-conceptos-clave.md) |
| Puedo modelar el problema como sustancias + campo | **Análisis Su-Campo + Soluciones estándar** | [Su-Campo](../05-analisis-su-campo/01-fundamentos-su-campo.md) |
| Problema complejo, herramientas simples no bastan | **ARIZ-85C** | [ARIZ](../07-ariz/00-que-es-ariz.md) |
| Quiero prever la siguiente generación del sistema | **Leyes de evolución / Curva S** | [Leyes](../08-leyes-evolucion/01-ley-completitud.md) |
| Quiero simplificar el sistema | **Trimming + Análisis funcional** | [Su-Campo](../05-analisis-su-campo/01-fundamentos-su-campo.md) |
| Estoy bloqueado mentalmente | **Operador STC / Hombrecillos inteligentes** | [Fundamentos](../00-fundamentos/01-que-es-triz.md) |

---

## Los 40 Principios Inventivos

| N.º | Principio | N.º | Principio |
|-----|---|-----|---|
| 1 | Segmentación | 21 | Saltar rápidamente |
| 2 | Extracción | 22 | Convertir daño en beneficio |
| 3 | Calidad local | 23 | Retroalimentación |
| 4 | Asimetría | 24 | Mediador |
| 5 | Unión / Consolidación | 25 | Autoservicio |
| 6 | Universalidad | 26 | Copia |
| 7 | Anidamiento (muñeca rusa) | 27 | Objeto desechable barato |
| 8 | Contrapeso | 28 | Sustitución de sistema mecánico |
| 9 | Acción previa opuesta | 29 | Neumática e hidráulica |
| 10 | Acción previa | 30 | Membranas flexibles y películas delgadas |
| 11 | Amortiguación previa | 31 | Material poroso |
| 12 | Equipotencialidad | 32 | Cambio de color |
| 13 | Inversión | 33 | Homogeneidad |
| 14 | Esferoidalidad / Curvatura | 34 | Desecho y recuperación |
| 15 | Dinamización | 35 | Cambio de parámetros (estado físico/químico) |
| 16 | Acción parcial o excesiva | 36 | Transición de fase |
| 17 | Transición a otra dimensión | 37 | Expansión térmica |
| 18 | Vibración mecánica | 38 | Oxidantes fuertes |
| 19 | Acción periódica | 39 | Atmósfera inerte |
| 20 | Continuidad de acción útil | 40 | Materiales compuestos |

---

## Los 39 Parámetros de Ingeniería

| N.º | Parámetro                            | N.º | Parámetro                                |
| --- | ------------------------------------ | --- | ---------------------------------------- |
| 1   | Peso del objeto móvil                | 21  | Potencia                                 |
| 2   | Peso del objeto estático             | 22  | Pérdida de energía                       |
| 3   | Longitud del objeto móvil            | 23  | Pérdida de sustancia                     |
| 4   | Longitud del objeto estático         | 24  | Pérdida de información                   |
| 5   | Área del objeto móvil                | 25  | Pérdida de tiempo                        |
| 6   | Área del objeto estático             | 26  | Cantidad de sustancia                    |
| 7   | Volumen del objeto móvil             | 27  | Fiabilidad                               |
| 8   | Volumen del objeto estático          | 28  | Precisión de medición                    |
| 9   | Velocidad                            | 29  | Precisión de fabricación                 |
| 10  | Fuerza                               | 30  | Factores dañinos sobre el objeto         |
| 11  | Tensión / Presión                    | 31  | Factores dañinos generados por el objeto |
| 12  | Forma                                | 32  | Facilidad de fabricación                 |
| 13  | Estabilidad de la composición        | 33  | Facilidad de uso                         |
| 14  | Resistencia                          | 34  | Facilidad de reparación                  |
| 15  | Durabilidad del objeto móvil         | 35  | Adaptabilidad / Versatilidad             |
| 16  | Durabilidad del objeto estático      | 36  | Complejidad del dispositivo              |
| 17  | Temperatura                          | 37  | Complejidad de control                   |
| 18  | Iluminación                          | 38  | Nivel de automatización                  |
| 19  | Energía usada por el objeto móvil    | 39  | Productividad                            |
| 20  | Energía usada por el objeto estático |     |                                          |

---

## Cómo usar la Matriz de Contradicciones

1. **Identificar** el parámetro que mejora (fila) y el que empeora (columna) entre los [39 parámetros](../04-matriz-contradicciones/00-como-usar-la-matriz.md).
2. **Buscar** la celda de intersección: contiene los números de los principios inventivos más frecuentes para ese par.
3. **Aplicar** cada principio sugerido al problema concreto, generando variantes de solución.

---

## Modelos Su-Campo

| Tipo | Diagrama | Descripción |
|---|---|---|
| **Completo** | S1 ←Campo→ S2 | Sistema funcional mínimo: dos sustancias y un campo |
| **Incompleto** | S1 ... S2 (sin campo) | Falta un elemento; la solución es completar el modelo |
| **Dañino** | S1 ←Campo→ S2 (línea ondulada) | Interacción no deseada entre componentes |
| **Insuficiente** | S1 ←Campo→ S2 (línea punteada) | La interacción existe pero es débil o insuficiente |

---

## Las 5 Clases de Soluciones Estándar

| Clase | Nombre | N.º | Enfoque |
|---|---|---|---|
| 1 | Construcción y destrucción de modelos Su-Campo | 13 | Completar, modificar o eliminar interacciones dañinas |
| 2 | Evolución de modelos Su-Campo | 23 | Hacer el sistema más eficiente (cadenas, bi-sistemas, campos) |
| 3 | Transición al supersistema y al micronivel | 6 | Cambiar de escala: macro → micro o sistema → supersistema |
| 4 | Detección y medición | 6 | Resolver problemas de medición y detección |
| 5 | Estrategias de simplificación | 17 | Introducir sustancias/campos derivados, usar vacío, campos combinados |

> Total: **76 soluciones estándar**. Ver [detalle completo](../06-soluciones-estandar/00-indice-soluciones.md).

---

## ARIZ-85C — Estructura en 9 partes

| Parte | Nombre | Acción clave |
|---|---|---|
| 1 | Análisis del problema | Formular mini-tarea, identificar contradicción técnica, elegir conflicto |
| 2 | Análisis del modelo del problema | Definir zona y tiempo operativo, formular contradicción física |
| 3 | Definir el RFI y la CF | Formular el resultado final ideal, intensificar la contradicción |
| 4 | Movilización de recursos | Inventariar recursos de sustancia y campo en zona operativa |
| 5 | Aplicación de la base de conocimiento | Consultar efectos físicos, químicos, geométricos |
| 6 | Cambio o reformulación del problema | Si no hay solución, reformular o ampliar la mini-tarea |
| 7 | Análisis del método de eliminación de la CF | Verificar que la contradicción física quede resuelta |
| 8 | Uso de la solución obtenida | Evaluar supersistema, buscar aplicaciones derivadas |
| 9 | Análisis del proceso de solución | Comparar con teoría, retroalimentar la base de conocimiento |

> Referencia completa: [ARIZ-85C](../07-ariz/00-que-es-ariz.md)

---

## Las 8 Leyes de Evolución de Sistemas Técnicos

| N.º | Ley | Enunciado compacto |
|---|---|---|
| 1 | [Completitud de partes](../08-leyes-evolucion/01-ley-completitud.md) | Todo ST viable necesita motor, transmisión, herramienta y control |
| 2 | [Conductividad energética](../08-leyes-evolucion/02-ley-conductividad.md) | La energía debe fluir libremente entre todos los componentes |
| 3 | [Coordinación de ritmos](../08-leyes-evolucion/03-ley-coordinacion.md) | Las frecuencias y ritmos de las partes deben armonizarse |
| 4 | [Idealidad creciente](../08-leyes-evolucion/04-ley-idealidad.md) | Los sistemas evolucionan hacia mayor idealidad (más función, menos costo) |
| 5 | [Desarrollo desigual](../08-leyes-evolucion/05-ley-desarrollo-desigual.md) | Los subsistemas evolucionan a ritmos distintos, generando contradicciones |
| 6 | [Transición al supersistema](../08-leyes-evolucion/06-ley-transicion-supersistema.md) | Los sistemas se integran en bi-sistemas, poli-sistemas y supersistemas |
| 7 | [Transición al micronivel](../08-leyes-evolucion/07-ley-transicion-micronivel.md) | La herramienta de trabajo evoluciona de macro a micro a campo |
| 8 | [Dinamización](../08-leyes-evolucion/08-ley-dinamizacion.md) | Los sistemas rígidos evolucionan hacia estructuras flexibles y adaptables |

---

## Principios de separación para Contradicciones Físicas

| Principio | Estrategia | Ejemplo |
|---|---|---|
| **Separación en el tiempo** | El parámetro tiene valor A en un momento y valor B en otro | Tren de aterrizaje: extendido al aterrizar, retraído en vuelo |
| **Separación en el espacio** | El parámetro tiene valor A en una zona y valor B en otra | Lápiz: duro por fuera (madera), blando por dentro (grafito) |
| **Separación entre el todo y las partes** | El todo tiene propiedad A, las partes tienen propiedad B | Cadena: flexible como todo, eslabones rígidos individualmente |
| **Separación por condición** | El parámetro cambia según una condición (temperatura, pH, campo...) | Válvula bimetálica: abre con calor, cierra con frío |

---

## Niveles de Invención

| Nivel | Nombre | % patentes | Descripción |
|---|---|---|---|
| 1 | Solución aparente | ~32% | Solución dentro del oficio, sin cambiar el sistema |
| 2 | Mejora menor | ~45% | Modificación de un elemento; decenas de ensayos |
| 3 | Mejora sustancial | ~19% | Resolución de contradicción dentro del campo; cientos de variantes |
| 4 | Concepto nuevo | ~3,7% | Solución fuera del campo; usa efectos de otras ciencias |
| 5 | Descubrimiento | ~0,3% | Nuevo fenómeno científico; base de sistemas radicalmente nuevos |

---

> Esta guía rápida resume las herramientas principales de TRIZ. Para profundizar en cada tema, siga los enlaces a las secciones correspondientes del curso.

---

**Navegación**: [← Glosario](02-glosario.md) · [Indice general →](../README.md)
