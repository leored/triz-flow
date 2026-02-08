# Principio 23. Retroalimentación

## Definición

Introducir retroalimentación (feedback) para mejorar un proceso o una acción. Este principio establece que la información sobre el resultado de una operación debe utilizarse para ajustar y corregir la propia operación en tiempo real o en ciclos sucesivos. Si ya existe retroalimentación, se puede invertir su sentido o modificar su naturaleza para obtener mejores resultados o resolver contradicciones que el lazo de control original no puede resolver.

## Subprincipios

a) **Introducir retroalimentación.** Incorporar un mecanismo que capture información sobre la salida o el estado del proceso y la devuelva a la entrada, permitiendo el ajuste automático del comportamiento del sistema sin intervención externa.

b) **Si ya existe retroalimentación, invertirla o cambiarla.** Cuando el lazo de retroalimentación existente no es suficiente o genera nuevos problemas, modificar su polaridad (de positiva a negativa o viceversa), su magnitud, su velocidad de respuesta o la variable que se mide, para alcanzar un nuevo punto de equilibrio o un comportamiento más deseable.

## Ejemplos técnicos

1. **Control PID en procesos industriales.** Un controlador PID (Proporcional-Integral-Derivativo) mide continuamente la variable de proceso (temperatura, presión, caudal) y compara su valor con el punto de ajuste. La diferencia (error) se retroalimenta al actuador, que modifica su acción para minimizar la desviación. Sin esta retroalimentación, el proceso operaría en lazo abierto y sería vulnerable a cualquier perturbación.

2. **Sistemas antibloqueo de frenos (ABS).** Los sensores de velocidad en cada rueda detectan cuándo una rueda está a punto de bloquearse durante la frenada. Esa información se retroalimenta al módulo de control, que libera y aplica la presión de frenado varias decenas de veces por segundo. La retroalimentación rápida evita la pérdida de adherencia y acorta la distancia de frenado.

3. **Circuitos de retroalimentación negativa en amplificadores electrónicos.** En un amplificador operacional, parte de la señal de salida se devuelve a la entrada inversora. Esta retroalimentación negativa reduce la ganancia pero mejora drásticamente la linealidad, el ancho de banda y la estabilidad del circuito. Si se invierte a retroalimentación positiva, el mismo circuito se convierte en un oscilador, generando un comportamiento completamente distinto.

## Ejemplos cotidianos

1. **Termostato doméstico.** El termostato mide la temperatura de la habitación y activa o desactiva la calefacción para mantener la temperatura deseada. Es un ejemplo clásico de retroalimentación negativa: cuando la temperatura sube por encima del umbral, el sistema se apaga; cuando baja, se enciende.

2. **Revisión de exámenes en el estudio.** Un estudiante que revisa sus errores en un examen y ajusta su método de estudio está aplicando retroalimentación. Si sus notas no mejoran con el método actual, puede invertir la estrategia (por ejemplo, pasar de memorización a resolución de problemas), modificando la naturaleza del lazo de retroalimentación.

## Principios relacionados

- [Principio 22. Convertir daño en beneficio](./22-convertir-dano-en-beneficio.md) — La retroalimentación puede revelar efectos dañinos que luego se aprovechan como recurso.
- [Principio 25. Autoservicio](./25-autoservicio.md) — Un sistema que se retroalimenta a sí mismo realiza funciones de autoservicio sin intervención externa.
- [Principio 28. Reemplazo del sistema mecánico](./28-reemplazo-mecanico.md) — La retroalimentación mecánica puede sustituirse por señales eléctricas, ópticas o electromagnéticas para mejorar la velocidad y precisión del lazo de control.
- [Principio 35. Cambio de parámetros](./35-cambio-de-parametros.md) — Cambiar el parámetro que se mide en el lazo de retroalimentación puede transformar el comportamiento del sistema.

---

| [← Principio 22. Convertir daño en beneficio](./22-convertir-dano-en-beneficio.md) | [Índice](./00-indice-principios.md) | [Principio 24. Mediador →](./24-mediador.md) |
|:---|:---:|---:|
