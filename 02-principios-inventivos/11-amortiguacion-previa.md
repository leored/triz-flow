# Principio 11. Amortiguación previa

## Definición

Compensar la baja fiabilidad de un objeto mediante contramedidas preparadas de antemano. Este principio establece que, ante la posibilidad de que un sistema falle o produzca efectos no deseados, se deben incorporar de forma anticipada mecanismos de protección, respaldo o compensación que actúen automáticamente cuando se presente la situación adversa.

## Subprincipios

a) **Preparar medios de emergencia para compensar la baja fiabilidad de un objeto.** Incorporar sistemas de respaldo, redundancias o mecanismos de seguridad que entren en funcionamiento cuando el componente principal falle o degrade su rendimiento.

b) **Preparar contramedidas de antemano para evitar efectos dañinos previsibles.** Anticipar los modos de fallo más probables y diseñar barreras, amortiguadores o sistemas de contención que neutralicen las consecuencias negativas antes de que se propaguen.

## Ejemplos técnicos

1. **Airbag en automóviles.** El airbag permanece oculto e inactivo durante el funcionamiento normal del vehículo. Sin embargo, está diseñado y posicionado de antemano para desplegarse en milisegundos ante una colisión, compensando la incapacidad del cinturón de seguridad por sí solo para proteger al ocupante en impactos severos.

2. **Sistemas UPS (alimentación ininterrumpida) en centros de datos.** Las baterías del UPS se mantienen cargadas permanentemente para compensar de forma inmediata cualquier interrupción del suministro eléctrico principal. El operador no necesita intervenir: la conmutación es automática y transparente.

3. **Fusibles y disyuntores en circuitos eléctricos.** Se instalan previamente en el circuito para interrumpir la corriente cuando esta supera un umbral peligroso, evitando daños en equipos o incendios antes de que la sobrecarga cause efectos irreversibles.

## Ejemplos cotidianos

1. **Botiquín de primeros auxilios.** Se prepara y almacena en casa, en el coche o en el lugar de trabajo antes de que ocurra cualquier accidente. No elimina el riesgo de lesiones, pero permite una respuesta inmediata que reduce la gravedad de las consecuencias.

2. **Copia de seguridad de archivos digitales.** Configurar copias de seguridad automáticas en la nube o en un disco externo compensa la posibilidad de que el disco duro principal falle, se pierda el dispositivo o un ransomware cifre los datos.

## Principios relacionados

- [Principio 9. Acción previa](./09-accion-previa.md) — La acción previa introduce cambios antes de que sean necesarios; la amortiguación previa se centra específicamente en preparar compensaciones ante fallos.
- [Principio 10. Acción anticipada](./10-accion-anticipada.md) — Complementa la amortiguación previa al disponer los objetos para que actúen sin demora cuando se requiera.
- [Principio 22. Convertir daño en beneficio](./22-convertir-dano-en-beneficio.md) — Mientras la amortiguación previa busca neutralizar el daño, este principio propone aprovecharlo.
- [Principio 35. Cambio de parámetros](./35-cambio-de-parametros.md) — Cambiar propiedades físicas puede ser una de las contramedidas preparadas de antemano.

---

| [← Principio 10. Acción anticipada](./10-accion-anticipada.md) | [Índice](./00-indice-principios.md) | [Principio 12. Equipotencialidad →](./12-equipotencialidad.md) |
|:---|:---:|---:|
