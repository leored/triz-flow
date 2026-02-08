# Ley 1: Completitud de las Partes del Sistema

## Enunciado

> Una condición necesaria para la viabilidad de un sistema técnico es la presencia y
> funcionamiento mínimo de sus cuatro partes principales: motor, transmisión, herramienta
> de trabajo y órgano de control.

Esta es la primera de las **leyes estáticas**: define las condiciones mínimas de existencia
de cualquier sistema técnico viable.

## Las cuatro partes esenciales

Todo sistema técnico funcional requiere exactamente cuatro componentes fundamentales:

```
┌──────────────────────────────────────────────────────────┐
│                   SISTEMA TÉCNICO                        │
│                                                          │
│  ┌─────────┐    ┌──────────────┐    ┌──────────────┐   │
│  │  MOTOR   │───→│ TRANSMISIÓN  │───→│ HERRAMIENTA  │   │
│  │ (fuente  │    │ (transmisor  │    │  DE TRABAJO   │   │
│  │  de      │    │  de energía) │    │ (ejecuta la  │   │
│  │ energía) │    │              │    │  función)     │   │
│  └─────────┘    └──────────────┘    └──────────────┘   │
│       ↑                                     ↑           │
│       │         ┌──────────────┐            │           │
│       └─────────│  ÓRGANO DE   │────────────┘           │
│                 │   CONTROL    │                         │
│                 │ (regula el   │                         │
│                 │  sistema)    │                         │
│                 └──────────────┘                         │
└──────────────────────────────────────────────────────────┘
```

### 1. Motor (fuente de energía)

Proporciona la energía necesaria para que el sistema realice su función. Puede ser un
motor eléctrico, un músculo humano, una reacción química, energía solar, etc.

### 2. Transmisión (transmisor de energía)

Transfiere y transforma la energía desde el motor hasta la herramienta de trabajo. Incluye
engranajes, palancas, cables, campos electromagnéticos, fluidos hidráulicos, etc.

### 3. Herramienta de trabajo (elemento de trabajo)

Es el componente que interactúa directamente con el objeto para realizar la función útil
principal del sistema. Es la razón de ser del sistema.

### 4. Órgano de control

Regula el funcionamiento del sistema: coordina las partes, ajusta parámetros y gestiona
la retroalimentación. Puede ser un operador humano, un termostato, un software, etc.

## Ejemplos de las cuatro partes

| Sistema | Motor | Transmisión | Herramienta | Control |
|---------|-------|-------------|-------------|---------|
| Automóvil | Motor de combustión | Caja de cambios, ejes | Ruedas (sobre el camino) | Conductor + electrónica |
| Bicicleta | Piernas del ciclista | Pedales, cadena, piñón | Ruedas (sobre el camino) | Ciclista (manos, ojos) |
| Martillo | Brazo del usuario | Mango (palanca) | Cabeza del martillo | Ojos + mano del usuario |
| Lámpara | Red eléctrica | Cables, interruptor | Bombilla (filamento) | Interruptor (usuario) |
| Lavadora | Motor eléctrico | Correa, tambor | Agua + detergente + agitación | Programador electrónico |

## Diagnóstico de sistemas incompletos

Cuando un sistema técnico no funciona correctamente, la primera verificación debe ser
comprobar la presencia de las cuatro partes. Un sistema con una parte ausente o
disfuncional es **no viable**.

### Procedimiento de diagnóstico

1. Identificar la **función útil principal** del sistema.
2. Localizar la **herramienta de trabajo**: el componente que ejecuta esa función.
3. Rastrear la **cadena energética**: ¿de dónde viene la energía? (motor) ¿cómo llega?
   (transmisión).
4. Identificar el **órgano de control**: ¿quién o qué regula el proceso?
5. Si falta alguna parte, el sistema es incompleto y esa es la causa raíz del problema.

### Ejemplo de diagnóstico

Un calentador solar de agua que no funciona bien:
- **Motor**: energía solar (presente, pero variable).
- **Transmisión**: panel colector → tubos → tanque (revisar si hay bloqueos).
- **Herramienta**: el agua caliente (está realizando su función, pero insuficiente).
- **Control**: no hay termostato ni válvula de regulación (ausente).

Diagnóstico: falta el órgano de control. Solución: agregar un termostato y una válvula
de derivación.

## Conexión con el análisis Su-Campo

Esta ley se relaciona directamente con el
[análisis Su-Campo](../05-analisis-su-campo/02-modelos-basicos.md). Un modelo Su-Campo
completo (S1 - Campo - S2) refleja la completitud mínima del sistema:

- **S1** corresponde a la herramienta de trabajo.
- **S2** corresponde al objeto sobre el que se actúa.
- **Campo** corresponde a la energía (motor + transmisión).

Cuando un modelo Su-Campo está **incompleto** (falta una sustancia o el campo), las
[soluciones estándar de Clase 1](../06-soluciones-estandar/01-clase-1-construir.md) indican que debe
completarse el modelo, lo cual es una aplicación directa de esta ley.

## Tendencia evolutiva

Con la evolución, las cuatro partes tienden a:

1. **Especializarse**: cada parte se optimiza para su función específica.
2. **Miniaturizarse**: se vuelven más compactas (ver [Ley 7](07-ley-transicion-micronivel.md)).
3. **Integrarse**: varias partes se fusionan en un solo componente multifuncional
   (ver [Ley 6](06-ley-transicion-supersistema.md)).
4. **Automatizarse**: el órgano de control pasa de humano a automático a inteligente
   (ver [Ley 8](08-ley-dinamizacion.md)).

## Aplicación práctica

Al diseñar un nuevo sistema o mejorar uno existente, use esta ley como lista de
verificación. Asegure que las cuatro partes estén presentes, que cada una funcione
adecuadamente y que estén correctamente conectadas. Esto garantiza la viabilidad básica
del sistema antes de aplicar otras herramientas TRIZ como los
[40 Principios Inventivos](../02-principios-inventivos/00-indice-principios.md) o la
[Matriz de Contradicciones](../04-matriz-contradicciones/00-como-usar-la-matriz.md).

---

**Navegación**: [← Visión general](00-vision-general.md) · [Ley 2: Conductividad →](02-ley-conductividad.md)
