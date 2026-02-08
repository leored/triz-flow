# Clase 4: Detección y medición

## Visión general

La Clase 4 contiene **17 soluciones estándar** enfocadas en problemas de **detección, medición y monitorización**. Mientras las Clases 1-3 se ocupan de modificar o mejorar la acción del sistema sobre un objeto, la Clase 4 se ocupa de obtener información sobre el estado del sistema, sus componentes o su entorno.

El enfoque general de la Clase 4 es: **todo problema de medición se puede reformular como un problema Su-Campo**, donde el objetivo es construir un modelo que traduzca la magnitud a medir en una señal detectable.

Se organiza en cinco subgrupos:

| Subgrupo | Tema | Soluciones |
|----------|------|-----------|
| 4.1 | Métodos indirectos | 4.1.1 -- 4.1.3 |
| 4.2 | Construcción de modelos de medición | 4.2.1 -- 4.2.4 |
| 4.3 | Mejora de modelos de medición | 4.3.1 -- 4.3.3 |
| 4.4 | Transición a bi y poli-sistemas de medición | 4.4.1 -- 4.4.5 |
| 4.5 | Medición en el micronivel | 4.5.1 -- 4.5.2 |

---

## 4.1 Métodos indirectos

Cuando la medición directa de un parámetro es difícil, costosa o imposible, se puede recurrir a métodos indirectos que midan algo relacionado y más accesible.

### 4.1.1 Medir un cambio en lugar de la magnitud directa

**Principio**: En lugar de medir el valor absoluto de un parámetro, medir el cambio (variación, diferencia, incremento) de ese parámetro o de otro relacionado. Los cambios suelen ser más fáciles de detectar que los valores absolutos.

**Ejemplo**: Medir el nivel exacto de líquido en un tanque opaco es difícil. En cambio, medir el *cambio* de peso del tanque es sencillo: un sensor de fuerza bajo el tanque detecta variaciones de masa que corresponden directamente a variaciones de nivel.

**Ejemplo 2**: Para detectar deformaciones mínimas en una estructura metálica, se pega una galga extensiométrica que no mide la deformación absoluta sino el *cambio de resistencia eléctrica* proporcional a la deformación.

---

### 4.1.2 Usar copias

**Principio**: Cuando no se puede medir directamente sobre el objeto original (es inaccesible, frágil, está en condiciones extremas), medir sobre una copia, modelo o réplica del objeto.

**Ejemplo**: Para medir el perfil de desgaste en el interior de un horno activo a 1500 C, se introduce periódicamente un material de moldeo que adquiere la forma del interior (copia). Se retira y se mide la copia en condiciones normales.

**Ejemplo 2**: En odontología, en lugar de medir directamente dentro de la boca del paciente, se toma una impresión (copia en silicona) que se analiza cómodamente en el laboratorio.

---

### 4.1.3 Medir derivadas sucesivas

**Principio**: Si la función original es difícil de medir, medir su primera o segunda derivada (velocidad de cambio, aceleración del cambio) u obtener la función integrando la derivada medida.

**Ejemplo**: Medir la posición exacta de un objeto en movimiento rápido es difícil. Un acelerómetro mide la segunda derivada de la posición (aceleración), que es fácil de captar con un sensor piezoeléctrico. Integrando dos veces se obtiene la posición.

**Ejemplo 2**: En sismología, los geófonos miden la velocidad del suelo (primera derivada del desplazamiento). La integración y derivación posteriores permiten obtener desplazamiento y aceleración según las necesidades del análisis.

---

## 4.2 Construcción de modelos de medición

### 4.2.1 Completar modelo Su-Campo de medición

**Principio**: Si no existe un modelo Su-Campo para la medición deseada, construirlo. Esto requiere identificar: qué sustancia se quiere medir (S1), qué campo la hace detectable (F), y qué sustancia actúa como detector (S2).

**Diagrama**:
```
  S1 (objeto a medir) ←-F_detección-→ S2 (detector)
                                         ↓
                                       Señal
```

**Ejemplo**: Para medir el espesor de una pared metálica sin acceso al otro lado, se construye un modelo Su-Campo ultrasónico: un transductor (S2) emite ondas ultrasónicas (F) que atraviesan la pared (S1) y se reflejan. El tiempo de ida y vuelta indica el espesor.

---

### 4.2.2 Modelo de medición con campo fácilmente detectable

**Principio**: Construir el modelo de medición utilizando un campo que sea fácilmente detectable con instrumentos disponibles, en particular campos electromagnéticos (luz, rayos X, radiofrecuencia).

**Ejemplo**: Para detectar fisuras internas en piezas metálicas, se usa radiografía industrial: rayos X (F_electromagnético, fácilmente detectable con película o sensor digital) atraviesan la pieza (S1) y revelan discontinuidades internas como sombras en la imagen.

---

### 4.2.3 Modelo de medición con aditivo detectable

**Principio**: Añadir una sustancia aditiva a S1 (o al entorno) que sea fácilmente detectable. El comportamiento del aditivo revela información sobre S1.

**Ejemplo**: Para detectar fugas en un sistema de tuberías presurizadas, se añade un gas trazador (helio o SF6) al fluido del sistema. Un detector de fugas (espectrómetro de masas de helio) capta concentraciones mínimas del trazador en el exterior, localizando la fuga con precisión.

**Ejemplo 2**: En medicina, se inyecta un contraste radiológico (aditivo detectable) en el torrente sanguíneo. Los rayos X revelan la anatomía vascular porque el contraste absorbe los rayos de forma diferente a los tejidos.

---

### 4.2.4 Modelo de medición con campo del entorno

**Principio**: En lugar de generar un campo de medición artificialmente, usar un campo que ya exista en el entorno del sistema.

**Ejemplo**: Un panel solar (S1) puede medirse con la luz solar natural (F_entorno) midiendo la corriente generada. No es necesario un simulador solar artificial para pruebas de campo.

**Ejemplo 2**: En geofísica, el campo magnético terrestre (F_entorno) se usa para detectar anomalías en la corteza terrestre. Un magnetómetro mide variaciones locales del campo, revelando depósitos minerales o estructuras geológicas.

---

## 4.3 Mejora de modelos de medición

### 4.3.1 Resonancia

**Principio**: Usar el fenómeno de resonancia para amplificar enormemente una señal de medición débil. Cuando la frecuencia de excitación coincide con la frecuencia natural del sistema, la amplitud de respuesta se multiplica.

**Ejemplo**: Un diapasón (detector acústico) resuena a una frecuencia específica. Si esa frecuencia está presente en el sonido ambiente, el diapasón vibra con gran amplitud, actuando como un filtro-amplificador natural. Este principio se usa en sensores de cuarzo que resuenan a frecuencias alteradas por masa, temperatura o presión depositada en su superficie.

**Ejemplo 2**: En resonancia magnética nuclear (RMN), los núcleos atómicos resuenan a frecuencias específicas bajo un campo magnético. La señal de resonancia es extremadamente débil, pero al excitar exactamente a la frecuencia de Larmor, la respuesta se amplifica hasta ser detectable, permitiendo obtener imágenes internas del cuerpo.

---

### 4.3.2 Frecuencia natural

**Principio**: Usar la frecuencia natural del sistema (o de un componente) como parámetro de medición. Los cambios en las propiedades del sistema alteran su frecuencia natural, que es muy sensible y fácil de medir con precisión.

**Ejemplo**: Una balanza de cuarzo. Un cristal de cuarzo oscila a su frecuencia natural. Cuando se deposita masa en su superficie, la frecuencia disminuye proporcionalmente. Se miden variaciones de masa del orden de nanogramos midiendo el cambio de frecuencia con un contador electrónico.

**Ejemplo 2**: Para detectar daño estructural en un puente, se miden sus frecuencias naturales de vibración. Cualquier fisura o deterioro altera las frecuencias modales de forma medible, permitiendo diagnóstico no destructivo.

---

### 4.3.3 Señal acoplada

**Principio**: Acoplar la medición a una señal oscilante o periódica ya existente en el sistema. La modulación de esa señal portadora por el parámetro a medir facilita la detección.

**Ejemplo**: En telecomunicaciones, la información (señal débil) se acopla a una portadora de radiofrecuencia (señal fuerte). De modo análogo, en medición, un parámetro físico débil se acopla a una señal periódica fuerte. Por ejemplo, un sensor de presión acoplado a una onda acústica modulada: la presión modula la frecuencia de la onda, y esa modulación se detecta fácilmente.

---

## 4.4 Transición a bi-sistemas y poli-sistemas de medición

### 4.4.1 Bi-sistema de medición

**Principio**: Crear un bi-sistema donde una parte sirve como referencia y la otra como elemento de medición activo. La comparación directa entre ambos elimina errores sistemáticos y aumenta la sensibilidad.

**Ejemplo**: Una balanza de brazos. Un plato contiene el objeto a medir; el otro contiene las pesas patrón (referencia). La comparación directa elimina errores debidos a gravedad variable, temperatura, etc.

**Ejemplo 2**: Un interferómetro de Michelson. Un haz láser se divide en dos: uno recorre el camino de referencia y otro el camino de medición. La interferencia de ambos haces revela diferencias de camino óptico con precisión nanométrica.

---

### 4.4.2 Medir la derivada en vez de la función

**Principio**: Si la función varía lentamente y es difícil de medir con precisión, medir su derivada (velocidad de cambio), que amplifica las variaciones y es más sensible.

**Ejemplo**: Para detectar una fuga lenta en un recipiente presurizado, medir la presión absoluta es poco sensible (cambio muy lento). En cambio, medir la *tasa de cambio de presión* (dp/dt) revela la fuga inmediatamente, pues cualquier fuga produce un dp/dt negativo no nulo.

---

### 4.4.3 Medir la integral en vez de la función

**Principio**: Si la función fluctúa rápidamente y las fluctuaciones dificultan la medición, medir la integral acumulada, que promedia las fluctuaciones y da un valor más estable.

**Ejemplo**: Para medir el caudal instantáneo de un fluido turbulento (fluctúa enormemente), se mide el volumen total acumulado en un tiempo dado (integral del caudal). Un medidor volumétrico totaliza litros, dando una medida estable del caudal medio.

---

### 4.4.4 Diferencia de mediciones

**Principio**: Usar la diferencia entre dos mediciones para obtener mayor sensibilidad o para eliminar componentes no deseados (ruido, deriva, offset).

**Ejemplo**: En un puente de Wheatstone, se mide la diferencia de potencial entre dos ramas de un circuito, una con el sensor y otra con una resistencia de referencia. La medición diferencial elimina el efecto de la tensión de alimentación, temperatura ambiente y ruido común.

**Ejemplo 2**: En astronomía, para detectar un exoplaneta, se mide la diferencia periódica en la posición o velocidad radial de una estrella, eliminando el movimiento propio y el ruido instrumentar.

---

### 4.4.5 Poli-sistema de sensores

**Principio**: Distribuir múltiples sensores (poli-sistema) para captar variaciones espaciales, temporales o de diferentes parámetros simultáneamente.

**Ejemplo**: Una red de estaciones meteorológicas distribuidas geográficamente (poli-sistema de sensores) proporciona un mapa meteorológico completo que ninguna estación individual puede generar. La interpolación entre estaciones permite predecir el tiempo en cualquier punto.

**Ejemplo 2**: En una línea de producción, múltiples cámaras de visión artificial (poli-sistema) inspeccionan un producto desde diferentes ángulos simultáneamente, detectando defectos que una sola cámara no vería.

---

## 4.5 Medición en el micronivel

### 4.5.1 Marcadores moleculares

**Principio**: Usar marcadores o trazadores a nivel molecular para detectar la presencia, concentración o distribución de sustancias. Los marcadores se eligen por su alta detectabilidad.

**Ejemplo**: En biología molecular, se usan marcadores fluorescentes (GFP, fluoresceína) que se unen a moléculas específicas. Bajo luz ultravioleta, las moléculas marcadas brillan, permitiendo su localización y cuantificación con microscopio de fluorescencia.

**Ejemplo 2**: Los trazadores radiactivos en medicina nuclear. Se administra al paciente una sustancia marcada con un isótopo radiactivo (tecnecio-99m). Un detector de radiación gamma mapea la distribución del trazador en el organismo, revelando la función de órganos.

**Ejemplo 3**: En hidrología, se añaden trazadores (rodamina, bromuro, isótopos estables) al agua subterránea para rastrear el flujo y la velocidad del acuífero.

---

### 4.5.2 Efectos físicos a micronivel

**Principio**: Aprovechar efectos físicos que operan a escala molecular, atómica o subatómica para medir parámetros macroscópicos con alta sensibilidad.

**Ejemplo**: El efecto piezoeléctrico. Ciertos cristales (cuarzo, titanato de bario) generan una tensión eléctrica proporcional a la presión mecánica aplicada a nivel molecular. Esto permite construir sensores de presión, acelerómetros y micrófonos de altísima sensibilidad.

**Ejemplo 2**: El efecto Hall. Cuando un material conductor porta corriente en presencia de un campo magnético perpendicular, aparece un voltaje transversal (a nivel electrónico) proporcional al campo. Los sensores Hall miden campos magnéticos, posición, velocidad de rotación y corriente eléctrica.

**Ejemplo 3**: El efecto túnel cuántico. En un microscopio de efecto túnel (STM), una corriente de electrones "tunela" entre una punta afilada y la superficie de una muestra cuando la distancia es de unos pocos angstroms. Las variaciones de corriente mapean la superficie con resolución atómica.

**Ejemplo 4**: Espectroscopía. La absorción o emisión de fotones por átomos y moléculas (transiciones electrónicas a nivel cuántico) produce espectros característicos. El análisis espectral permite identificar composición química, temperatura y velocidad de sustancias remotas (desde estrellas hasta gases industriales).

---

## Guía rápida de selección — Clase 4

```
Necesito detectar o medir algo.
  │
  ├── ¿La medición directa es posible?
  │     │
  │     ├── NO → 4.1 (métodos indirectos)
  │     │     ├── ¿Puedo medir un cambio relacionado?  → 4.1.1
  │     │     ├── ¿Puedo medir sobre una copia?        → 4.1.2
  │     │     └── ¿Puedo medir la derivada/integral?   → 4.1.3
  │     │
  │     └── SÍ, pero no hay modelo de medición → 4.2 (construir modelo)
  │           ├── ¿Puedo construir un Su-Campo?          → 4.2.1
  │           ├── ¿Puedo usar campo detectable?          → 4.2.2
  │           ├── ¿Puedo añadir aditivo detectable?      → 4.2.3
  │           └── ¿Puedo usar campo del entorno?         → 4.2.4
  │
  ├── Hay modelo de medición pero es poco sensible → 4.3 (mejorar)
  │     ├── ¿Puedo usar resonancia?                → 4.3.1
  │     ├── ¿Puedo usar frecuencia natural?        → 4.3.2
  │     └── ¿Puedo acoplar a señal existente?      → 4.3.3
  │
  ├── Necesito mayor sensibilidad o cobertura → 4.4 (bi/poli-sistema)
  │     ├── ¿Puedo crear referencia + medición?    → 4.4.1
  │     ├── ¿Medir derivada?                       → 4.4.2
  │     ├── ¿Medir integral?                       → 4.4.3
  │     ├── ¿Usar medición diferencial?            → 4.4.4
  │     └── ¿Distribuir múltiples sensores?        → 4.4.5
  │
  └── Necesito detección a nivel molecular → 4.5 (micronivel)
        ├── ¿Puedo usar marcadores/trazadores?     → 4.5.1
        └── ¿Puedo usar efectos físicos micro?     → 4.5.2
```

---

## Relación con el Análisis Su-Campo

Todo problema de medición se puede formular como un [modelo Su-Campo](../05-analisis-su-campo/04-notacion-diagramas.md) donde:

- **S1** = objeto/parámetro a medir.
- **F** = campo de detección (el medio por el cual se obtiene la información).
- **S2** = detector/sensor (la sustancia que transforma el campo en una señal útil).

Las soluciones de la Clase 4 proporcionan estrategias sistemáticas para construir, completar y mejorar estos modelos Su-Campo de medición.

---

**Navegación**: [← Clase 3](03-clase-3-transicion.md) · [Clase 5 →](05-clase-5-estrategias.md)
