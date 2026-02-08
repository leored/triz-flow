# Los 39 Parámetros de Ingeniería de TRIZ — Descripción completa

Este documento presenta la descripción detallada de los 39 parámetros de ingeniería definidos por G. S. Altshuller. Estos parámetros constituyen el eje de filas y columnas de la [Matriz de Contradicciones](../04-matriz-contradicciones/) y son la herramienta fundamental para formular **contradicciones técnicas** dentro del flujo TRIZ.

Para cada parámetro se incluye:
- **Número y nombre** según la clasificación clásica de TRIZ.
- **Descripción** conceptual.
- **Qué mide** — magnitudes, unidades o criterios asociados.
- **Ejemplos de sistemas** donde el parámetro es relevante.

> **Convención**: en TRIZ se distingue entre objetos **móviles** (que cambian su posición espacial durante el funcionamiento) y **estacionarios** (que permanecen fijos). Esta distinción se refleja en los parámetros 1-8 y 15-16, 19-20.

---

## Parámetro 1 — Peso del objeto móvil

**Descripción**: Masa del objeto que se desplaza o cuya posición varía durante el funcionamiento del sistema, medida en un campo gravitatorio. Incluye tanto el peso propio del objeto como el de las cargas que transporta durante su movimiento.

**Qué mide**: Fuerza gravitatoria sobre el objeto móvil. Se expresa en newtons (N) o, de forma más habitual en ingeniería, en kilogramos-fuerza (kgf). Indirectamente refleja la masa (kg) del objeto.

**Ejemplos de sistemas relevantes**:
- Vehículos terrestres, aéreos y espaciales: reducir el peso mejora el consumo energético pero puede comprometer la resistencia estructural.
- Robots industriales y sus efectores finales: un brazo más ligero permite mayor velocidad pero puede perder rigidez.
- Proyectiles y munición: la masa afecta tanto al alcance como a la energía cinética en el impacto.
- Dispositivos portátiles (teléfonos, herramientas manuales): el peso influye directamente en la facilidad de uso (parámetro 33).

**Contradicciones frecuentes en la Matriz**: Peso del objeto móvil (1) vs. Resistencia (14); Peso del objeto móvil (1) vs. Velocidad (9); Peso del objeto móvil (1) vs. Fiabilidad (27).

---

## Parámetro 2 — Peso del objeto estacionario

**Descripción**: Masa del objeto que no cambia de posición durante la operación del sistema, medida en un campo gravitatorio. Incluye estructuras de soporte, cimentaciones, bastidores, carcasas fijas y cualquier elemento cuya función se realice sin desplazamiento.

**Qué mide**: Fuerza gravitatoria sobre el objeto estacionario. Mismas unidades que el parámetro 1 (N, kgf, kg).

**Ejemplos de sistemas relevantes**:
- Edificios y estructuras civiles: reducir el peso de la estructura sin comprometer la estabilidad (parámetro 13).
- Bancadas y bastidores de máquinas herramienta: la masa aporta amortiguación de vibraciones pero dificulta el transporte e instalación.
- Torres de telecomunicaciones y antenas: el peso de la torre debe soportar cargas de viento sin ser excesivo.
- Mobiliario industrial: mesas de trabajo, armarios y estanterías fijas.

**Contradicciones frecuentes en la Matriz**: Peso del objeto estacionario (2) vs. Resistencia (14); Peso del objeto estacionario (2) vs. Facilidad de fabricación (32).

---

## Parámetro 3 — Longitud del objeto móvil

**Descripción**: Dimensión lineal mayor (o cualquier dimensión lineal crítica) del objeto en movimiento. Comprende longitud, anchura, altura, diámetro o cualquier medida lineal relevante del objeto que se desplaza.

**Qué mide**: Dimensiones lineales en metros (m), milímetros (mm) u otras unidades de longitud. Puede referirse a una dimensión específica o al tamaño global del objeto.

**Ejemplos de sistemas relevantes**:
- Aviones: la envergadura alar determina sustentación pero limita el acceso a hangares y pistas.
- Trenes y convoyes: la longitud total afecta la capacidad de carga y la maniobrabilidad en curvas.
- Herramientas quirúrgicas endoscópicas: la longitud permite alcance interno pero complica el control preciso.
- Cables y tuberías flexibles en movimiento: la longitud influye en pérdidas de presión o señal.

**Contradicciones frecuentes en la Matriz**: Longitud del objeto móvil (3) vs. Volumen del objeto móvil (7); Longitud del objeto móvil (3) vs. Facilidad de uso (33).

---

## Parámetro 4 — Longitud del objeto estacionario

**Descripción**: Dimensión lineal mayor (o cualquier dimensión lineal crítica) del objeto fijo. Aplica a estructuras, conductos, vigas, ejes fijos y cualquier elemento estacionario cuya dimensión lineal sea funcionalmente significativa.

**Qué mide**: Dimensiones lineales del objeto estacionario, en las mismas unidades que el parámetro 3.

**Ejemplos de sistemas relevantes**:
- Puentes: la luz (longitud libre entre apoyos) define la capacidad de cruce pero exige mayor resistencia estructural.
- Tuberías de proceso industrial: la longitud de tubería fija afecta las pérdidas de carga y el coste de material.
- Vías férreas y carreteras: la extensión determina la conectividad pero también el coste de construcción y mantenimiento.
- Antenas y mástiles fijos: la longitud de la antena se relaciona con la frecuencia de resonancia.

**Contradicciones frecuentes en la Matriz**: Longitud del objeto estacionario (4) vs. Peso del objeto estacionario (2); Longitud del objeto estacionario (4) vs. Resistencia (14).

---

## Parámetro 5 — Área del objeto móvil

**Descripción**: Superficie exterior, sección transversal o cualquier característica bidimensional relevante del objeto en movimiento. Incluye áreas de contacto, superficies de sustentación, secciones de flujo, etc.

**Qué mide**: Área en metros cuadrados (m²) o unidades derivadas. Puede referirse a la superficie total, una sección transversal o un área funcional específica.

**Ejemplos de sistemas relevantes**:
- Alas de aeronaves: mayor área alar genera más sustentación pero también más resistencia aerodinámica.
- Neumáticos: el área de contacto con el suelo afecta la tracción y el desgaste.
- Velas de embarcaciones: la superficie vélica captura más viento pero exige una estructura más robusta.
- Paracaídas: el área determina la velocidad de descenso.

**Contradicciones frecuentes en la Matriz**: Área del objeto móvil (5) vs. Velocidad (9); Área del objeto móvil (5) vs. Peso del objeto móvil (1).

---

## Parámetro 6 — Área del objeto estacionario

**Descripción**: Superficie exterior, sección transversal o cualquier característica bidimensional relevante del objeto fijo. Incluye áreas de intercambio térmico, superficies de cimentación, secciones de conductos fijos, etc.

**Qué mide**: Área en metros cuadrados (m²). Puede ser superficie total, área útil o sección funcional.

**Ejemplos de sistemas relevantes**:
- Intercambiadores de calor: mayor área de transferencia mejora la eficiencia térmica pero aumenta el volumen y el coste.
- Paneles solares fijos: la superficie de captación determina la energía generada.
- Cimientos y zapatas: el área de apoyo distribuye las cargas sobre el terreno.
- Placas de circuitos impresos: la superficie disponible limita la densidad de componentes.

**Contradicciones frecuentes en la Matriz**: Área del objeto estacionario (6) vs. Volumen del objeto estacionario (8); Área del objeto estacionario (6) vs. Peso del objeto estacionario (2).

---

## Parámetro 7 — Volumen del objeto móvil

**Descripción**: Espacio tridimensional ocupado por el objeto en movimiento. Incluye tanto el volumen externo (envolvente) como el volumen interno útil (capacidad de carga, habitáculo, etc.).

**Qué mide**: Volumen en metros cúbicos (m³), litros (L) o centímetros cúbicos (cm³).

**Ejemplos de sistemas relevantes**:
- Contenedores de transporte marítimo: maximizar el volumen de carga dentro de dimensiones estándar.
- Satélites: el volumen debe ajustarse al carenado del vehículo de lanzamiento.
- Maletas y mochilas: volumen interior vs. facilidad de transporte.
- Cápsulas espaciales: el volumen habitable afecta la ergonomía y la autonomía de la misión.

**Contradicciones frecuentes en la Matriz**: Volumen del objeto móvil (7) vs. Peso del objeto móvil (1); Volumen del objeto móvil (7) vs. Velocidad (9).

---

## Parámetro 8 — Volumen del objeto estacionario

**Descripción**: Espacio tridimensional ocupado por el objeto fijo. Incluye el volumen de la estructura, de los depósitos estáticos, del espacio interior de edificios, etc.

**Qué mide**: Volumen en m³, L o cm³.

**Ejemplos de sistemas relevantes**:
- Tanques de almacenamiento: el volumen determina la capacidad pero también la presión sobre las paredes y la cimentación.
- Edificios y naves industriales: el volumen interior define la capacidad operativa.
- Reactores químicos: el volumen del reactor afecta el tiempo de residencia y la conversión.
- Hornos industriales: el volumen de la cámara determina el tamaño de las piezas procesables.

**Contradicciones frecuentes en la Matriz**: Volumen del objeto estacionario (8) vs. Peso del objeto estacionario (2); Volumen del objeto estacionario (8) vs. Temperatura (17).

---

## Parámetro 9 — Velocidad

**Descripción**: Rapidez con que un objeto cambia de posición en el espacio o velocidad de ejecución de un proceso. Incluye velocidad lineal, angular, velocidad de flujo, tasa de operación y cualquier medida de rapidez funcional del sistema.

**Qué mide**: Velocidad lineal (m/s, km/h), angular (rad/s, rpm), velocidad de flujo (m³/s), o velocidad de proceso (unidades/tiempo).

**Ejemplos de sistemas relevantes**:
- Vehículos de todo tipo: mayor velocidad reduce el tiempo de viaje pero puede comprometer la seguridad y aumentar el consumo energético (parámetros 19, 22).
- Máquinas herramienta: la velocidad de corte afecta la productividad (parámetro 39) y el desgaste de la herramienta.
- Procesadores informáticos: la velocidad de reloj mejora el rendimiento pero genera más calor (parámetro 17).
- Líneas de producción: la velocidad de la cinta transportadora determina la cadencia de producción.

**Contradicciones frecuentes en la Matriz**: Velocidad (9) vs. Peso del objeto móvil (1); Velocidad (9) vs. Pérdida de energía (22); Velocidad (9) vs. Precisión de fabricación (29).

---

## Parámetro 10 — Fuerza (intensidad)

**Descripción**: Interacción mecánica entre objetos capaz de provocar aceleración, deformación o cambio de estado. En un sentido amplio, incluye cualquier tipo de intensidad de interacción: fuerza mecánica, campo magnético, campo eléctrico, presión de radiación, etc.

**Qué mide**: Fuerza en newtons (N), kilonewtons (kN); intensidad de campo en las unidades correspondientes (T, V/m, W/m²). También puede referirse a par motor (N·m) o empuje.

**Ejemplos de sistemas relevantes**:
- Prensas hidráulicas: la fuerza aplicada determina la capacidad de conformado pero requiere estructuras más robustas.
- Motores: el par motor define la capacidad de arrastre.
- Imanes y electroimanes: la fuerza de sujeción magnética.
- Sistemas de frenado: la fuerza de frenado determina la distancia de parada.

**Contradicciones frecuentes en la Matriz**: Fuerza (10) vs. Peso del objeto móvil (1); Fuerza (10) vs. Pérdida de energía (22); Fuerza (10) vs. Complejidad del dispositivo (36).

---

## Parámetro 11 — Tensión/Presión

**Descripción**: Fuerza distribuida sobre una superficie o un volumen. Incluye tensión mecánica (tracción, compresión, cortante, flexión, torsión), presión de fluidos, presión de contacto y cualquier forma de esfuerzo distribuido en el material o sistema.

**Qué mide**: Presión o tensión en pascales (Pa), megapascales (MPa), bares, atmósferas o PSI. También esfuerzos internos del material.

**Ejemplos de sistemas relevantes**:
- Recipientes a presión: calderas, autoclaves, cilindros de gas. La presión interna determina la capacidad operativa pero exige paredes más gruesas.
- Neumáticos: la presión de inflado afecta la huella de contacto (parámetro 5), la resistencia a la rodadura y el confort.
- Turbinas hidráulicas y de vapor: la presión del fluido de trabajo define la potencia extraíble (parámetro 21).
- Estructuras sometidas a cargas: vigas, columnas y cables donde las tensiones determinan la integridad estructural.

**Contradicciones frecuentes en la Matriz**: Tensión/Presión (11) vs. Resistencia (14); Tensión/Presión (11) vs. Volumen del objeto estacionario (8).

---

## Parámetro 12 — Forma

**Descripción**: Contorno, configuración geométrica o apariencia externa del objeto. Incluye la geometría tridimensional, la topología superficial, la simetría y cualquier atributo que defina la morfología del sistema.

**Qué mide**: No posee una unidad única; se evalúa mediante parámetros geométricos (radios de curvatura, ángulos, perfiles), coeficientes de forma, relaciones de aspecto y descripciones topológicas.

**Ejemplos de sistemas relevantes**:
- Carrocerías de vehículos: la forma determina el coeficiente aerodinámico (Cx) y la estética.
- Perfiles alares: la forma del perfil define las características de sustentación y resistencia.
- Envases y embalajes: la forma debe optimizar el almacenamiento, el apilado y la ergonomía de uso.
- Componentes electrónicos: la forma del encapsulado afecta la disipación térmica y la densidad de montaje.

**Contradicciones frecuentes en la Matriz**: Forma (12) vs. Facilidad de fabricación (32); Forma (12) vs. Resistencia (14); Forma (12) vs. Peso del objeto móvil (1).

---

## Parámetro 13 — Estabilidad de la composición del objeto

**Descripción**: Capacidad del sistema para mantener su estructura interna, composición material e integridad ante perturbaciones externas o internas. Incluye estabilidad química, estabilidad de fase, resistencia a la degradación, mantenimiento de las propiedades del material a lo largo del tiempo.

**Qué mide**: Se evalúa mediante indicadores de degradación, tasas de corrosión, cambios de composición, vida útil del material, estabilidad dimensional y resistencia al envejecimiento.

**Ejemplos de sistemas relevantes**:
- Materiales expuestos a la intemperie: pinturas, recubrimientos, polímeros que deben resistir la degradación UV.
- Alimentos y fármacos: estabilidad de la composición durante el almacenamiento.
- Aleaciones a alta temperatura: mantener las propiedades metalúrgicas en servicio.
- Baterías: estabilidad electroquímica durante los ciclos de carga y descarga.

**Contradicciones frecuentes en la Matriz**: Estabilidad de la composición (13) vs. Temperatura (17); Estabilidad de la composición (13) vs. Factores dañinos externos (30).

---

## Parámetro 14 — Resistencia

**Descripción**: Capacidad del objeto de soportar cargas mecánicas (estáticas, dinámicas, cíclicas) sin sufrir deformación permanente, fractura ni pérdida funcional. Incluye resistencia a la tracción, compresión, flexión, fatiga, impacto y desgaste.

**Qué mide**: Límite elástico (MPa), resistencia última (MPa), tenacidad (J/m²), vida a fatiga (ciclos), dureza (escalas Rockwell, Vickers, Brinell), resistencia al desgaste.

**Ejemplos de sistemas relevantes**:
- Estructuras aeronáuticas: requieren alta resistencia con mínimo peso (parámetro 1), lo que impulsa el uso de materiales compuestos.
- Herramientas de corte: la resistencia al desgaste determina la vida útil.
- Equipos de protección personal: cascos, chalecos, que deben absorber impactos.
- Ejes, engranajes y rodamientos: sometidos a cargas cíclicas donde la fatiga es el modo de fallo dominante.

**Contradicciones frecuentes en la Matriz**: Resistencia (14) vs. Peso del objeto móvil (1); Resistencia (14) vs. Facilidad de fabricación (32); Resistencia (14) vs. Tensión/Presión (11).

---

## Parámetro 15 — Duración de la acción del objeto móvil

**Descripción**: Tiempo durante el cual el objeto móvil puede realizar su función de manera continua o acumulada. Incluye vida útil operativa, autonomía, tiempo de funcionamiento sin mantenimiento y durabilidad en servicio del objeto en movimiento.

**Qué mide**: Tiempo en segundos, horas o años; también en ciclos de operación, kilómetros recorridos u otra unidad que represente la duración del servicio funcional.

**Ejemplos de sistemas relevantes**:
- Satélites: la duración de la misión determina la rentabilidad; depende del combustible, la degradación de paneles solares y la electrónica.
- Baterías de vehículos eléctricos: la autonomía (horas o km) es un parámetro clave de diseño.
- Herramientas eléctricas portátiles: el tiempo de uso por carga limita la productividad en campo.
- Sondas espaciales: deben operar durante años en condiciones extremas.

**Contradicciones frecuentes en la Matriz**: Duración de la acción del objeto móvil (15) vs. Peso del objeto móvil (1); Duración de la acción del objeto móvil (15) vs. Pérdida de energía (22).

---

## Parámetro 16 — Duración de la acción del objeto estacionario

**Descripción**: Tiempo durante el cual el objeto fijo puede realizar su función de manera continua o acumulada. Incluye vida útil de estructuras, vida de servicio de instalaciones fijas, durabilidad de componentes estáticos.

**Qué mide**: Las mismas unidades que el parámetro 15, aplicadas al contexto estacionario: horas de servicio, años de vida útil, ciclos soportados.

**Ejemplos de sistemas relevantes**:
- Infraestructuras civiles (puentes, presas, edificios): diseñadas para vidas útiles de 50-100 años.
- Reactores nucleares: la duración operativa se mide en décadas y está limitada por la irradiación de materiales.
- Tuberías de proceso: la corrosión y la erosión limitan la vida útil.
- Cimientos y muros de contención: deben mantener su función durante toda la vida de la estructura.

**Contradicciones frecuentes en la Matriz**: Duración de la acción del objeto estacionario (16) vs. Peso del objeto estacionario (2); Duración de la acción del objeto estacionario (16) vs. Tensión/Presión (11).

---

## Parámetro 17 — Temperatura

**Descripción**: Condición térmica del objeto, del proceso o del entorno operativo. Incluye la temperatura de operación, los gradientes térmicos, los límites de temperatura del material y la gestión térmica del sistema.

**Qué mide**: Temperatura en grados Celsius (°C), kelvin (K) o Fahrenheit (°F). También gradientes térmicos (°C/m, °C/s) y flujos de calor (W/m²).

**Ejemplos de sistemas relevantes**:
- Motores de combustión interna: temperaturas elevadas mejoran la eficiencia termodinámica pero aceleran la degradación de materiales (parámetro 13).
- Sistemas electrónicos: el calor generado por los componentes debe disiparse para evitar fallos.
- Procesos metalúrgicos: la temperatura de tratamiento térmico define las propiedades mecánicas.
- Sistemas criogénicos: superconductores, almacenamiento de gases licuados, donde se requieren temperaturas extremadamente bajas.

**Contradicciones frecuentes en la Matriz**: Temperatura (17) vs. Resistencia (14); Temperatura (17) vs. Estabilidad de la composición (13); Temperatura (17) vs. Fiabilidad (27).

---

## Parámetro 18 — Brillo/Luminosidad

**Descripción**: Flujo luminoso, intensidad de iluminación o energía lumínica asociada al objeto o proceso. Incluye cualquier forma de energía radiante en el espectro visible, así como extensiones al infrarrojo y ultravioleta cuando sean funcionalmente relevantes.

**Qué mide**: Luminancia (cd/m²), iluminancia (lux), flujo luminoso (lúmenes), intensidad luminosa (candelas), irradiancia (W/m²).

**Ejemplos de sistemas relevantes**:
- Sistemas de iluminación: LED, lámparas, faros. Mayor brillo mejora la visibilidad pero aumenta el consumo energético (parámetro 19) y el calor (parámetro 17).
- Pantallas y displays: la luminosidad determina la legibilidad pero afecta la vida útil y el consumo.
- Sistemas láser: la intensidad del haz es clave para corte, soldadura y comunicaciones.
- Sistemas ópticos de inspección: la iluminación adecuada determina la precisión de medición (parámetro 28).

**Contradicciones frecuentes en la Matriz**: Brillo (18) vs. Pérdida de energía (22); Brillo (18) vs. Temperatura (17).

---

## Parámetro 19 — Energía consumida por el objeto móvil

**Descripción**: Cantidad total de energía que necesita el objeto móvil para realizar su función. Incluye energía cinética, energía para superar la fricción, energía eléctrica consumida por sistemas embarcados, combustible, etc.

**Qué mide**: Energía en julios (J), kilovatios-hora (kWh), calorías, o combustible equivalente (litros, kg). También consumo específico (energía por unidad de masa transportada, por kilómetro, etc.).

**Ejemplos de sistemas relevantes**:
- Automóviles y camiones: el consumo de combustible es un parámetro competitivo fundamental.
- Drones: la energía de la batería limita el tiempo de vuelo (parámetro 15) y la carga útil (parámetro 1).
- Trenes de alta velocidad: el consumo eléctrico es proporcional al cubo de la velocidad.
- Equipos quirúrgicos robotizados: el consumo energético afecta el diseño de baterías y la autonomía.

**Contradicciones frecuentes en la Matriz**: Energía consumida por el objeto móvil (19) vs. Velocidad (9); Energía consumida por el objeto móvil (19) vs. Peso del objeto móvil (1); Energía consumida por el objeto móvil (19) vs. Potencia (21).

---

## Parámetro 20 — Energía consumida por el objeto estacionario

**Descripción**: Cantidad total de energía que necesita el objeto estacionario para realizar su función. Incluye energía eléctrica, térmica, neumática, hidráulica y cualquier otra forma de energía requerida por un sistema fijo.

**Qué mide**: Mismas unidades que el parámetro 19, aplicadas al contexto estacionario.

**Ejemplos de sistemas relevantes**:
- Sistemas HVAC (calefacción, ventilación y aire acondicionado): el consumo energético es un factor principal del coste operativo de edificios.
- Hornos industriales: el consumo energético determina el coste de producción.
- Centros de datos: la energía consumida por servidores y por su refrigeración.
- Iluminación de naves industriales: el consumo eléctrico permanente es significativo.

**Contradicciones frecuentes en la Matriz**: Energía consumida por el objeto estacionario (20) vs. Temperatura (17); Energía consumida por el objeto estacionario (20) vs. Área del objeto estacionario (6).

---

## Parámetro 21 — Potencia

**Descripción**: Tasa de realización de trabajo o de transformación de energía por unidad de tiempo. Describe la capacidad del sistema para entregar o procesar energía de forma sostenida.

**Qué mide**: Potencia en vatios (W), kilovatios (kW), caballos de fuerza (CV, HP). También potencia específica (W/kg, kW/L).

**Ejemplos de sistemas relevantes**:
- Motores eléctricos y de combustión: la potencia nominal define la capacidad de trabajo.
- Generadores eólicos y turbinas: la potencia determina la producción eléctrica.
- Amplificadores de señal: la potencia de salida limita el alcance de la comunicación.
- Sistemas de calefacción: la potencia térmica dimensiona la capacidad de climatización.

**Contradicciones frecuentes en la Matriz**: Potencia (21) vs. Peso del objeto móvil (1); Potencia (21) vs. Pérdida de energía (22); Potencia (21) vs. Complejidad del dispositivo (36).

---

## Parámetro 22 — Pérdida de energía

**Descripción**: Energía que se disipa o desperdicia sin contribuir a la función útil del sistema. Incluye pérdidas por fricción, pérdidas eléctricas (efecto Joule), pérdidas por radiación, pérdidas hidrodinámicas, pérdidas aerodinámicas y cualquier forma de disipación no deseada.

**Qué mide**: Energía perdida en julios (J), vatios (W) de potencia disipada, o como porcentaje de eficiencia (rendimiento = energía útil / energía total).

**Ejemplos de sistemas relevantes**:
- Transmisiones mecánicas: pérdidas por fricción en engranajes, correas y rodamientos.
- Redes eléctricas: pérdidas por efecto Joule en líneas de transmisión y transformadores.
- Motores térmicos: pérdidas por calor evacuado (limitadas por el ciclo de Carnot).
- Sistemas hidráulicos: pérdidas de carga en tuberías, válvulas y accesorios.

**Contradicciones frecuentes en la Matriz**: Pérdida de energía (22) vs. Velocidad (9); Pérdida de energía (22) vs. Potencia (21); Pérdida de energía (22) vs. Peso del objeto móvil (1).

---

## Parámetro 23 — Pérdida de sustancia

**Descripción**: Material que se pierde, consume o degrada durante el funcionamiento del sistema sin contribuir directamente a la función útil. Incluye desgaste, evaporación, fugas, corrosión, emisiones y cualquier forma de pérdida material.

**Qué mide**: Masa perdida por unidad de tiempo (g/h, kg/año), tasa de desgaste (mm/h, μm/ciclo), tasa de fuga (L/min, mL/h), emisiones (g/km, ppm).

**Ejemplos de sistemas relevantes**:
- Herramientas de corte: desgaste del filo durante el mecanizado.
- Motores de combustión: consumo de aceite lubricante y emisiones de gases.
- Sistemas de refrigeración: fugas de refrigerante.
- Procesos de fabricación: generación de virutas, rebabas y recortes como desperdicio material.
- Tuberías: pérdida de material por erosión interna o corrosión.

**Contradicciones frecuentes en la Matriz**: Pérdida de sustancia (23) vs. Resistencia (14); Pérdida de sustancia (23) vs. Velocidad (9); Pérdida de sustancia (23) vs. Temperatura (17).

---

## Parámetro 24 — Pérdida de información

**Descripción**: Datos, señales o conocimiento que se degradan, distorsionan o pierden durante la operación del sistema. Incluye ruido en señales, errores de transmisión, pérdida de trazabilidad, degradación de datos almacenados y cualquier reducción en la calidad o cantidad de la información disponible.

**Qué mide**: Tasa de error de bits (BER), relación señal/ruido (SNR, dB), integridad de datos (%), pérdida de resolución, distorsión de señal.

**Ejemplos de sistemas relevantes**:
- Sistemas de telecomunicaciones: atenuación y ruido en la transmisión de señales.
- Sistemas de almacenamiento de datos: degradación del medio (discos, cintas) con el tiempo.
- Sensores y sistemas de medición: ruido que reduce la precisión de medición (parámetro 28).
- Cadenas de mando en procesos industriales: pérdida de instrucciones o especificaciones entre etapas.
- Copias y reproducciones: degradación progresiva de la información en copias sucesivas.

**Contradicciones frecuentes en la Matriz**: Pérdida de información (24) vs. Velocidad (9); Pérdida de información (24) vs. Complejidad de control (37).

---

## Parámetro 25 — Pérdida de tiempo

**Descripción**: Tiempo consumido que no contribuye directamente a la función útil del sistema. Incluye tiempos muertos, tiempos de espera, tiempos de preparación, retardos, interrupciones y cualquier período improductivo.

**Qué mide**: Tiempo en segundos, minutos, horas. También como porcentaje del tiempo total de ciclo, eficiencia temporal (OEE — Overall Equipment Effectiveness), tiempo de ciclo vs. tiempo neto de valor añadido.

**Ejemplos de sistemas relevantes**:
- Líneas de producción: tiempos de cambio de herramienta (setup), tiempos de espera entre operaciones.
- Transporte: tiempo de carga/descarga, congestiones, escalas.
- Procesos administrativos: tiempos de aprobación, colas en trámites.
- Sistemas informáticos: latencia, tiempos de arranque, tiempos de compilación.

**Contradicciones frecuentes en la Matriz**: Pérdida de tiempo (25) vs. Precisión de fabricación (29); Pérdida de tiempo (25) vs. Complejidad del dispositivo (36); Pérdida de tiempo (25) vs. Productividad (39).

---

## Parámetro 26 — Cantidad de sustancia

**Descripción**: Masa, volumen o cantidad total de material utilizado en el sistema o procesado por él. Se refiere tanto a la materia que forma parte del sistema como a la materia prima que consume durante su operación.

**Qué mide**: Masa (kg, t), volumen (m³, L), número de moles, o cualquier otra medida cuantitativa de la materia involucrada.

**Ejemplos de sistemas relevantes**:
- Procesos químicos: la cantidad de reactivos define la escala de producción.
- Construcción: el volumen de hormigón, acero y otros materiales estructurales.
- Industria farmacéutica: la dosificación precisa de principios activos.
- Embalaje: la cantidad de material de empaque afecta el coste y el impacto ambiental (parámetro 31).

**Contradicciones frecuentes en la Matriz**: Cantidad de sustancia (26) vs. Peso del objeto móvil (1); Cantidad de sustancia (26) vs. Pérdida de sustancia (23); Cantidad de sustancia (26) vs. Facilidad de fabricación (32).

---

## Parámetro 27 — Fiabilidad

**Descripción**: Probabilidad de que el sistema realice su función prevista sin fallo durante un período de tiempo y bajo condiciones especificadas. Incluye disponibilidad, mantenibilidad y seguridad funcional.

**Qué mide**: Probabilidad de funcionamiento sin fallo (R(t)), tiempo medio entre fallos (MTBF), tasa de fallos (λ, fallos/hora), disponibilidad (%), tiempo medio de reparación (MTTR).

**Ejemplos de sistemas relevantes**:
- Sistemas aeronáuticos: la fiabilidad es crítica por razones de seguridad; se exigen tasas de fallo extremadamente bajas (10⁻⁹/hora de vuelo para sistemas críticos).
- Equipos médicos: marcapasos, ventiladores, monitores de constantes vitales donde un fallo puede ser letal.
- Redes eléctricas: la fiabilidad del suministro se mide en "nueves" (99,99% de disponibilidad).
- Sistemas militares: deben operar en condiciones extremas sin posibilidad inmediata de reparación.

**Contradicciones frecuentes en la Matriz**: Fiabilidad (27) vs. Complejidad del dispositivo (36); Fiabilidad (27) vs. Peso del objeto móvil (1); Fiabilidad (27) vs. Facilidad de fabricación (32).

---

## Parámetro 28 — Precisión de medición

**Descripción**: Grado de concordancia entre el valor medido y el valor real (verdadero) de la magnitud. Incluye exactitud, resolución, repetibilidad, reproducibilidad y la capacidad de detección del sistema de medición.

**Qué mide**: Error de medición (absoluto o relativo), incertidumbre (±), resolución (mínima variación detectable), repetibilidad (desviación estándar en mediciones repetidas), linealidad y sesgo del instrumento.

**Ejemplos de sistemas relevantes**:
- Instrumentación de laboratorio: balanzas analíticas, espectrómetros, microscopios.
- Sistemas de navegación: GPS, sistemas inerciales, donde la precisión posicional es crítica.
- Control de calidad industrial: máquinas de medición por coordenadas (CMM), calibres, galgas.
- Diagnóstico médico: precisión de análisis clínicos y sistemas de imagen.

**Contradicciones frecuentes en la Matriz**: Precisión de medición (28) vs. Velocidad (9); Precisión de medición (28) vs. Complejidad de control (37); Precisión de medición (28) vs. Pérdida de energía (22).

---

## Parámetro 29 — Precisión de fabricación

**Descripción**: Grado en que las dimensiones, propiedades y características del objeto fabricado se ajustan a las especificaciones de diseño. Incluye tolerancias dimensionales, acabado superficial, propiedades del material y conformidad geométrica.

**Qué mide**: Tolerancias dimensionales (mm, μm), rugosidad superficial (Ra, Rz), índices de capacidad del proceso (Cp, Cpk), tasa de defectos (ppm, sigma), desviación respecto a la especificación nominal.

**Ejemplos de sistemas relevantes**:
- Industria aeroespacial: tolerancias de micras en componentes de turbinas.
- Semiconductores: la precisión de fabricación en litografía determina la densidad de transistores.
- Industria relojera: ajuste micrométrico de componentes mecánicos.
- Óptica de precisión: lentes y espejos con tolerancias de fracciones de longitud de onda.

**Contradicciones frecuentes en la Matriz**: Precisión de fabricación (29) vs. Facilidad de fabricación (32); Precisión de fabricación (29) vs. Pérdida de tiempo (25); Precisión de fabricación (29) vs. Complejidad del dispositivo (36).

---

## Parámetro 30 — Factores dañinos que actúan sobre el objeto desde el exterior

**Descripción**: Agentes, condiciones o influencias del entorno que afectan negativamente al objeto o sistema. Incluye factores ambientales (corrosión, radiación, temperatura extrema, vibraciones externas, contaminación), cargas accidentales, interferencias electromagnéticas y cualquier efecto externo no deseado.

**Qué mide**: Se cuantifica según la naturaleza del factor: tasa de corrosión (mm/año), nivel de vibración (g, mm/s²), dosis de radiación (Gy, Sv), concentración de contaminantes (ppm, mg/m³), nivel de interferencia electromagnética (dBm).

**Ejemplos de sistemas relevantes**:
- Plataformas marinas: corrosión por agua salada, oleaje, vientos extremos.
- Satélites: radiación cósmica, micrometeoritos, vacío y ciclos térmicos extremos.
- Equipos electrónicos en entornos industriales: interferencias electromagnéticas, polvo, vibraciones.
- Infraestructuras en zonas sísmicas: fuerzas de terremoto como factor dañino externo.
- Equipos médicos: la esterilización repetida (calor, radiación, químicos) degrada los materiales.

**Contradicciones frecuentes en la Matriz**: Factores dañinos externos (30) vs. Resistencia (14); Factores dañinos externos (30) vs. Estabilidad de la composición (13); Factores dañinos externos (30) vs. Fiabilidad (27).

---

## Parámetro 31 — Factores dañinos generados por el objeto

**Descripción**: Efectos nocivos, emisiones o influencias negativas que el propio sistema produce sobre su entorno, los operadores o otros sistemas. Incluye contaminación, ruido, vibraciones, radiación emitida, calor residual, residuos y cualquier efecto secundario perjudicial.

**Qué mide**: Niveles de emisión según el tipo: ruido (dB(A)), emisiones gaseosas (g/km, ppm), vibraciones transmitidas (mm/s), radiación emitida (W/m², Sv), residuos generados (kg/unidad producida), campos electromagnéticos (V/m, μT).

**Ejemplos de sistemas relevantes**:
- Motores de combustión: emisiones de CO₂, NOₓ, partículas.
- Maquinaria industrial: ruido y vibraciones que afectan a los operadores.
- Plantas nucleares: radiación y residuos radiactivos.
- Sistemas electrónicos: interferencias electromagnéticas generadas que afectan a equipos próximos.
- Procesos químicos: efluentes líquidos y gaseosos contaminantes.

**Contradicciones frecuentes en la Matriz**: Factores dañinos generados por el objeto (31) vs. Potencia (21); Factores dañinos generados por el objeto (31) vs. Productividad (39); Factores dañinos generados por el objeto (31) vs. Velocidad (9).

---

## Parámetro 32 — Facilidad de fabricación

**Descripción**: Grado de simplicidad, conveniencia y economía del proceso de manufactura del objeto o sistema. Incluye la fabricabilidad, el número de operaciones necesarias, la necesidad de procesos especiales, los requisitos de cualificación del personal y la accesibilidad de los materiales.

**Qué mide**: Número de operaciones de fabricación, tiempo de producción, coste de manufactura, nivel de cualificación requerido, tasa de rechazos en producción. No existe una unidad única; se evalúa de forma relativa o mediante indicadores compuestos (DFM — Design for Manufacturing).

**Ejemplos de sistemas relevantes**:
- Piezas de plástico moldeadas por inyección: la geometría debe facilitar el desmoldeo.
- Circuitos impresos: el diseño debe considerar las limitaciones del proceso de fabricación (ancho de pista mínimo, espaciados).
- Estructuras soldadas: la accesibilidad de las juntas y la selección del proceso de soldadura.
- Componentes mecanizados: la elección de tolerancias afecta directamente el número de operaciones y el coste.

**Contradicciones frecuentes en la Matriz**: Facilidad de fabricación (32) vs. Precisión de fabricación (29); Facilidad de fabricación (32) vs. Forma (12); Facilidad de fabricación (32) vs. Resistencia (14).

---

## Parámetro 33 — Facilidad de uso/operación

**Descripción**: Grado de comodidad, sencillez e intuitividad en la utilización del sistema. Incluye ergonomía, número de acciones requeridas para operar el sistema, necesidad de formación, accesibilidad de los controles, claridad de la interfaz y esfuerzo físico o cognitivo del operador.

**Qué mide**: Tiempo de aprendizaje, número de pasos para completar una tarea, tasa de errores del usuario, esfuerzo físico (escala de Borg, fuerzas de operación), puntuaciones de usabilidad (SUS — System Usability Scale), eficiencia del operador.

**Ejemplos de sistemas relevantes**:
- Teléfonos inteligentes: la facilidad de uso es un diferenciador competitivo clave.
- Maquinaria industrial: la interfaz hombre-máquina (HMI) determina la productividad y la seguridad.
- Electrodomésticos: los usuarios esperan una operación intuitiva sin necesidad de leer manuales extensos.
- Instrumentos quirúrgicos: la ergonomía afecta la precisión y la fatiga del cirujano.

**Contradicciones frecuentes en la Matriz**: Facilidad de uso (33) vs. Complejidad del dispositivo (36); Facilidad de uso (33) vs. Nivel de automatización (38); Facilidad de uso (33) vs. Peso del objeto móvil (1).

---

## Parámetro 34 — Facilidad de reparación

**Descripción**: Simplicidad y rapidez con que se puede diagnosticar un fallo, acceder al componente averiado, sustituirlo o repararlo y restablecer la función del sistema. Incluye la accesibilidad de los componentes, la disponibilidad de piezas de repuesto, la necesidad de herramientas especiales y la documentación técnica.

**Qué mide**: Tiempo medio de reparación (MTTR), coste de reparación, número de herramientas requeridas, nivel de cualificación del personal de mantenimiento, accesibilidad de componentes (indicadores DFMA — Design for Maintenance and Assembly).

**Ejemplos de sistemas relevantes**:
- Automóviles: el acceso al motor y a los componentes críticos afecta el tiempo y coste de mantenimiento.
- Equipos en plataformas petrolíferas remotas: la facilidad de reparación es vital por la dificultad logística.
- Servidores en centros de datos: los componentes críticos (discos, fuentes de alimentación) deben ser intercambiables en caliente (hot-swappable).
- Equipos militares en campaña: deben poder repararse con herramientas mínimas y personal no especializado.

**Contradicciones frecuentes en la Matriz**: Facilidad de reparación (34) vs. Fiabilidad (27); Facilidad de reparación (34) vs. Complejidad del dispositivo (36); Facilidad de reparación (34) vs. Peso del objeto estacionario (2).

---

## Parámetro 35 — Adaptabilidad/Versatilidad

**Descripción**: Capacidad del sistema para ajustarse, reconfigurarse o funcionar eficazmente bajo condiciones variadas, para distintos usos o con diferentes entradas. Incluye flexibilidad, modularidad, capacidad de reconfiguración, rango de operación y universalidad funcional.

**Qué mide**: Número de funciones o modos de operación, rango de condiciones operativas (temperatura, presión, materiales procesables), tiempo de reconfiguración, coste de adaptación, grado de modularidad.

**Ejemplos de sistemas relevantes**:
- Máquinas CNC: pueden fabricar piezas muy diversas cambiando el programa y las herramientas.
- Teléfonos inteligentes: un solo dispositivo integra decenas de funciones (cámara, GPS, comunicación, computación).
- Navajas multiusos: múltiples herramientas en un solo objeto.
- Robots colaborativos: reprogramables para distintas tareas de ensamblaje, inspección o manipulación.
- Vehículos anfibios: operan en tierra y agua.

**Contradicciones frecuentes en la Matriz**: Adaptabilidad (35) vs. Complejidad del dispositivo (36); Adaptabilidad (35) vs. Fiabilidad (27); Adaptabilidad (35) vs. Facilidad de fabricación (32).

---

## Parámetro 36 — Complejidad del dispositivo

**Descripción**: Número y diversidad de elementos que componen el sistema, así como la cantidad y naturaleza de sus interacciones. Incluye la complejidad estructural (número de piezas, tipos de materiales, número de interfaces), la complejidad funcional (número de funciones realizadas) y la complejidad organizativa (jerarquías, subsistemas).

**Qué mide**: Número de componentes, número de interfaces, número de materiales diferentes, número de grados de libertad, profundidad de la lista de materiales (BOM), índice de complejidad (diversas métricas propietarias).

**Ejemplos de sistemas relevantes**:
- Aviones comerciales: millones de piezas, cientos de sistemas interconectados.
- Relojes mecánicos de alta gama: cientos de componentes de alta precisión en un volumen muy reducido.
- Circuitos integrados: miles de millones de transistores, extrema complejidad en un espacio mínimo.
- Maquinaria agrícola moderna: combina sistemas mecánicos, hidráulicos, electrónicos y de software.

**Contradicciones frecuentes en la Matriz**: Complejidad del dispositivo (36) vs. Fiabilidad (27); Complejidad del dispositivo (36) vs. Facilidad de fabricación (32); Complejidad del dispositivo (36) vs. Facilidad de reparación (34).

---

## Parámetro 37 — Complejidad de control/monitorización

**Descripción**: Dificultad asociada a la medición, detección, regulación y supervisión del funcionamiento del sistema. Incluye la complejidad de los algoritmos de control, el número de variables a monitorizar, la dificultad de los diagnósticos, la cantidad de sensores e instrumentos necesarios y los requisitos de procesamiento de datos.

**Qué mide**: Número de variables controladas, número de sensores, complejidad algorítmica (orden de magnitud), ancho de banda del sistema de control, tiempo de respuesta, carga computacional (MIPS, FLOPS).

**Ejemplos de sistemas relevantes**:
- Plantas de proceso químico: cientos de variables (temperaturas, presiones, caudales, composiciones) deben controlarse simultáneamente.
- Vehículos autónomos: fusión de datos de múltiples sensores (LiDAR, cámaras, radar, ultrasonidos) y toma de decisiones en tiempo real.
- Sistemas de control de tráfico aéreo: monitorización simultánea de centenares de aeronaves.
- Redes eléctricas inteligentes (smart grids): equilibrio dinámico entre generación y demanda con múltiples fuentes distribuidas.

**Contradicciones frecuentes en la Matriz**: Complejidad de control (37) vs. Precisión de medición (28); Complejidad de control (37) vs. Nivel de automatización (38); Complejidad de control (37) vs. Fiabilidad (27).

---

## Parámetro 38 — Nivel de automatización

**Descripción**: Grado en que el sistema ejecuta sus funciones sin intervención humana directa. Va desde la operación completamente manual hasta la autonomía total, pasando por niveles intermedios de asistencia, supervisión y control compartido.

**Qué mide**: Nivel de automatización según escalas estándar (p. ej., niveles SAE para vehículos, niveles ISA-95 para industria), porcentaje de operaciones automatizadas, ratio operador/máquina, grado de autonomía decisional.

**Ejemplos de sistemas relevantes**:
- Fábricas automatizadas: líneas de producción con robots, AGV y sistemas de inspección automática.
- Vehículos autónomos: escala de niveles 0 (manual) a 5 (autonomía plena).
- Electrodomésticos inteligentes: programación, autoadaptación y respuesta a comandos de voz.
- Sistemas de riego automatizado: sensores de humedad que controlan el riego sin intervención humana.
- Pilotos automáticos en aviación: gestión del vuelo en crucero con supervisión humana.

**Contradicciones frecuentes en la Matriz**: Nivel de automatización (38) vs. Complejidad del dispositivo (36); Nivel de automatización (38) vs. Facilidad de reparación (34); Nivel de automatización (38) vs. Fiabilidad (27).

---

## Parámetro 39 — Productividad

**Descripción**: Cantidad de funciones útiles realizadas, operaciones completadas o producto generado por unidad de tiempo. Representa la eficiencia global del sistema en el cumplimiento de su función principal. Es el parámetro que resume el rendimiento operativo del sistema.

**Qué mide**: Unidades producidas por hora, operaciones por segundo, piezas por turno, toneladas por día, transacciones por minuto, o cualquier métrica de salida útil por unidad de tiempo. También la productividad relativa (output/input).

**Ejemplos de sistemas relevantes**:
- Líneas de ensamblaje: piezas producidas por hora; la productividad es la métrica fundamental de rendimiento.
- Impresoras 3D: volumen de material depositado por hora o piezas impresas por día.
- Servidores web: solicitudes procesadas por segundo.
- Procesos agrícolas: toneladas cosechadas por hectárea por temporada.
- Centros de mecanizado: tasa de arranque de material (cm³/min).

**Contradicciones frecuentes en la Matriz**: Productividad (39) vs. Precisión de fabricación (29); Productividad (39) vs. Pérdida de energía (22); Productividad (39) vs. Factores dañinos generados por el objeto (31); Productividad (39) vs. Pérdida de tiempo (25).

---

## Resumen: cómo utilizar los parámetros en la resolución de problemas

1. **Defina la función principal** del sistema y sus condiciones de operación.
2. **Identifique el parámetro que desea mejorar** — seleccione de la lista de 39 el que mejor describe la característica que quiere incrementar o reducir.
3. **Identifique el parámetro que empeora** como consecuencia no deseada de la mejora propuesta.
4. **Formule la contradicción técnica**: "Si mejoro [parámetro X], empeora [parámetro Y]."
5. **Consulte la [Matriz de Contradicciones](../04-matriz-contradicciones/)** en la celda (X, Y) para obtener los [principios inventivos](../02-principios-inventivos/00-indice-principios.md) recomendados.
6. **Aplique los principios** al contexto específico de su problema para generar soluciones inventivas.

Consulte el [índice de parámetros](00-indice-parametros.md) para una referencia rápida en formato de tabla.

---

**Navegación**: [← Índice de parámetros](00-indice-parametros.md) · [40 Principios Inventivos →](../02-principios-inventivos/00-indice-principios.md)
