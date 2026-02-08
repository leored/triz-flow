# Parte 3: Definicion del Resultado Final Ideal y Contradiccion Fisica

> **Objetivo**: Formular el Resultado Final Ideal (RFI) a nivel macro y micro, y explicitar la contradiccion fisica que debe resolverse. Esta parte es el corazon conceptual de ARIZ.

La Parte 3 obliga al resolutor a definir *que deberia ocurrir idealmente* en la zona operativa, sin preocuparse aun por *como* lograrlo. Esta separacion entre el "que" y el "como" es uno de los principios fundamentales de ARIZ para evitar la inercia psicologica.

---

## Paso 3.1: Formular el RFI-1 (macro nivel)

El **Resultado Final Ideal a nivel macro (RFI-1)** describe lo que el recurso-X debe lograr en la zona operativa durante el tiempo operativo.

### Formato del RFI-1

> "El recurso-X, sin complicar el sistema y sin causar efectos daninos, [realiza la accion util requerida] durante T1 dentro de la zona operativa."

**Reglas de formulacion:**

1. El recurso-X debe actuar **por si mismo**, sin necesidad de mecanismos adicionales.
2. La accion debe ocurrir **sin introducir nuevos efectos daninos**.
3. La formulacion no debe especificar que es el recurso-X ni como actua.

### Por que "ideal"

El RFI no es una solucion realista; es una **brujula**. Al formular lo que seria perfecto, se orienta la busqueda hacia soluciones que se aproximen a ese ideal. Las soluciones que mas se acercan al RFI son las mas innovadoras y elegantes.

Recordar que la idealidad se define como:

```
            Funciones utiles
Idealidad = ─────────────────────────────────
            Funciones daninas + costes
```

El RFI ideal tiene idealidad infinita: la funcion util se cumple sin funciones daninas ni costes. Ver [Ley de aumento de idealidad](../08-leyes-evolucion/04-ley-idealidad.md).

---

## Paso 3.2: Intensificar el RFI-1

Reforzar la formulacion del RFI-1 anadiendo la condicion de que el sistema **no cambie en absoluto**:

> "El recurso-X, sin ninguna modificacion al sistema existente, proporciona [accion util] durante T1 en la zona operativa."

Esta intensificacion parece absurda (si el sistema no cambia, como se resuelve el problema?), pero ese es precisamente su valor. Al exigir lo imposible, se fuerza al pensamiento a buscar recursos ocultos dentro del propio sistema.

**Tecnica practica**: Preguntarse: *"Si no pudiera cambiar absolutamente nada del sistema, que tendria que ocurrir espontaneamente para que el problema desapareciera?"*

---

## Paso 3.3: Formular la contradiccion fisica a nivel macro

La **contradiccion fisica (CF)** establece que la zona operativa debe tener **propiedades opuestas simultaneamente**.

### Formato de la CF macro

> "La zona operativa debe tener la propiedad [P] para proporcionar [accion util], y simultaneamente debe tener la propiedad [anti-P] para evitar [accion danina]."

### Diferencia con la contradiccion tecnica

| Tipo | Que se opone | Ejemplo |
|------|-------------|---------|
| Contradiccion tecnica (CT) | Dos parametros distintos del sistema | "Si aumento la resistencia, aumenta el peso" |
| Contradiccion fisica (CF) | Dos valores opuestos del mismo parametro | "El material debe ser rigido y flexible al mismo tiempo" |

La CT describe un conflicto entre parametros; la CF lo reduce a un **solo parametro** que debe tomar dos valores contradictorios. La CF es siempre mas precisa y mas util para encontrar la solucion.

### Relacion con la Matriz de Contradicciones

Mientras que la [Matriz de Contradicciones](../04-matriz-contradicciones/00-como-usar-la-matriz.md) trabaja con contradicciones tecnicas (dos parametros), ARIZ llega a la contradiccion fisica (un parametro, dos estados). Esto explica por que ARIZ es mas potente: opera en un nivel de abstraccion mas profundo.

---

## Paso 3.4: Formular el RFI-2 (micro nivel)

El **RFI-2** reformula el ideal a nivel de las particulas (moleculas, atomos, electrones) que componen la zona operativa.

### Formato del RFI-2

> "Las particulas de [la zona operativa] deben [comportarse de tal manera] para proporcionar [accion util] y simultaneamente [comportarse de la manera opuesta] para evitar [accion danina]."

### Por que el micro nivel

Muchas soluciones inventivas operan a nivel micro (cambios de fase, reacciones quimicas, efectos electromagneticos). Pensar en terminos de particulas abre un espacio de soluciones que el pensamiento a nivel macro no permite ver.

La transicion del nivel macro al micro es una de las [Leyes de Evolucion](../08-leyes-evolucion/07-ley-transicion-micronivel.md) de los sistemas tecnicos: los sistemas evolucionan hacia el uso de efectos a escalas cada vez menores.

---

## Paso 3.5: Formular la contradiccion fisica a nivel micro

Explicitar la CF en terminos de particulas:

> "Las particulas de la zona operativa deben tener la propiedad [P] para [funcion util], y deben tener la propiedad [anti-P] para [evitar dano]."

Esta formulacion es mas concreta que la CF macro y a menudo sugiere directamente soluciones basadas en efectos fisicos o quimicos. Las particulas no pueden "negociar" un compromiso; la solucion debe ser una separacion real de las propiedades opuestas.

---

## Paso 3.6: Aplicar las Soluciones Estandar (segundo intento)

**Segundo intento** de solucion usando las [76 Soluciones Estandar](../06-soluciones-estandar/00-indice-soluciones.md), ahora con una comprension mucho mas profunda del problema.

### Diferencia con el paso 1.7

| Aspecto | Paso 1.7 (primer intento) | Paso 3.6 (segundo intento) |
|---------|---------------------------|---------------------------|
| Nivel de comprension | Modelo del problema (abstracto) | CF explicita + ZO + TO + recursos |
| Guia de busqueda | Tipo de modelo Su-Campo | La contradiccion fisica como filtro |
| Probabilidad de exito | Baja-media | Media-alta |

### Procedimiento

1. Reformular el conflicto como modelo [Su-Campo](../05-analisis-su-campo/01-fundamentos-su-campo.md) usando la CF como guia.
2. Buscar Soluciones Estandar que resuelvan especificamente la CF (separacion en el tiempo, en el espacio, por condicion, o por transicion entre niveles).
3. Considerar especialmente las Soluciones Estandar de [Clase 3](../06-soluciones-estandar/03-clase-3-transicion.md) (transicion a supersistema y micronivel).

> **Si se encuentra solucion** → pasar a [Parte 7: Analisis de la solucion](07-parte-7-solucion.md).
> **Si no se encuentra** → continuar a [Parte 4: Movilizacion de recursos](04-parte-4-recursos.md).

---

## Resumen de la Parte 3

| Paso | Accion | Resultado |
|:----:|--------|-----------|
| 3.1 | Formular RFI-1 | Ideal a nivel macro |
| 3.2 | Intensificar RFI-1 | Ideal extremo (sin cambios al sistema) |
| 3.3 | Formular CF macro | Propiedad P y anti-P en la zona operativa |
| 3.4 | Formular RFI-2 | Ideal a nivel micro (particulas) |
| 3.5 | Formular CF micro | P y anti-P a nivel de particulas |
| 3.6 | Aplicar Soluciones Estandar | Segundo intento con CF como guia |

---

**Navegacion**: [<< Parte 2](02-parte-2-modelo.md) · [Parte 4 >>](04-parte-4-recursos.md)
