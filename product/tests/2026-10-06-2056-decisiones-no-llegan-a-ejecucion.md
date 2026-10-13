---
opportunity: decisiones-no-llegan-a-ejecucion
solutions: product/solutions/2026-10-06-2019-decisiones-no-llegan-a-ejecucion.md
status: designed
---

# Tests de solución para: lo decidido en la reunión no llega intacto a quien lo ejecuta

## Por qué testear

Hay dos alternativas en test: A1 `tarjeta-de-cierre` y A3 `recap-de-decisiones`. Las dos tienen el dolor evidenciado (`real`*, aunque fuera del segmento por tamaño), pero a ninguna de las dos soluciones reaccionó nadie todavía. De A1, nadie vio una tarjeta confirmada en vivo. De A3, solo hay reacción negativa al recap **actual**: 6/10 lo abandonan. Eso no dice que un recap estructurado sí funcione. Primero va lo que mata más rápido a cada una: si el conductor sostiene el mecanismo (#7 y #9 en `product/overview.md`). La comparación a 2 semanas (#8) queda como siguiente paso.

Quedan fuera de este archivo: la factibilidad de extraer decisiones de la transcripción (A1 y A3 están en `to check with tech`, y el dueño es tech) y la viabilidad (#2, que necesita una conversación con IT).

Diseño común a T1 y T2: los mismos conductores hacen una reunión con A1 y otra con A3, en orden alternado (la mitad empieza por cada una), para no favorecer a ninguna. En los dos casos el mago de Oz trabaja **solo con la transcripción**: así no sale un borrador mejor del que saldría de la IA.

## T1. tarjeta-de-cierre: tarjeta confirmada en vivo en una reunión real (mago de Oz)
- **Test status:** designed
- **Belief under test:** "Con un borrador armado a partir de la transcripción, el conductor confirma la tarjeta frente al grupo en ≤ 3 min en al menos 7 de cada 10 reuniones con decisiones, y no vuelve a cerrar a mano después. Se cae si la confirmación supera los 3 min o se saltea en más de 3 de cada 10 reuniones." (#7, `[feature: tarjeta-de-cierre] [value]`)
- **Risk:** [value]
- **Test type:** wizard-of-oz
- **What we do:**
  1. El conductor elige una reunión de trabajo real de la semana en la que espera decisiones. Esa reunión tiene que tener la transcripción activada.
  2. El mago entra como participante silencioso, sigue la transcripción en vivo y arma la tarjeta: decisión, responsable, fecha y porqué. Lo que la transcripción no deja claro va marcado como dudoso, sin completarlo con criterio propio.
  3. Unos 5 minutos antes del final, le pasa la tarjeta al conductor, que la comparte y la confirma o corrige frente al grupo.
  4. El mago publica la versión confirmada donde se ejecuta (Jira, el canal o Planner, según el conductor).
  5. A las 48 h, el mago revisa si el conductor volvió a cerrar a mano (acta, tickets nuevos o edición de lo publicado) y se lo pregunta en un mensaje corto.
- **With whom:** 6 conductores reclutados para que completen al menos 5. Son los mismos que hacen T2. Salen del pool de la encuesta (64 candidatos en `product/insights/2026-09-30-1621-colaboracion-en-vivo-fuera-de-teams.md`), filtrados a cuentas Business Premium de 100 a 300 licencias, que conduzcan 2 o más reuniones de trabajo con decisiones por semana y tengan la transcripción disponible. R-170 queda excluido hasta verificar su identidad. Si el pool filtrado no llega a 6, se completa por email a organizadores de cuentas del segmento.
- **Material needed:**
  - **Plantilla de tarjeta**, con cuatro campos (decisión, responsable, fecha, porqué) y una marca de "dudoso".
  - **Reglas del mago:** usa solo la transcripción, no corrige ambigüedades, no agrega contexto que no esté en el audio y entrega a falta de 5 min.
  - **Guion breve** para el conductor y consentimiento del grupo para que haya un observador.
  - **Hoja de captura por reunión:** hora de inicio y fin de la confirmación, si se salteó o se postergó, campos que se corrigieron en vivo, dónde se publicó, y el chequeo a las 48 h (si volvió a cerrar a mano: sí o no, y qué hizo).
  - **Queda fuera a propósito:** resumen de la conversación, automatización, integración y diseño visual.
- **Material:** —
- **Duration:** 1 semana de reclutamiento y 1 semana de corridas (T1 y T2 juntos), más el chequeo a las 48 h.
- **Signal and threshold:** cada reunión **cumple** si se dan tres condiciones: (a) la confirmación frente al grupo se hace en esa reunión (no se saltea ni se pasa a "después"), (b) toma ≤ 3 min, cronometrada por el mago, y (c) a las 48 h el conductor no volvió a cerrar a mano. Un conductor que aceptó y después no lleva la tarjeta a la reunión cuenta como salteo. **Umbral: pasa si cumplen ≥ 4 de 5 reuniones.**
- **Decision rule:**
  - **continue** si cumplen ≥ 4 de 5.
  - **change** si cumplen 3 de 5, o si las fallas son solo de tiempo (se confirmó, pero en más de 3 min). En ese caso se reduce la tarjeta (por ejemplo, solo responsable y fecha) y se repite el test con la versión nueva.
  - **discard** si en ≥ 2 de 5 se saltea la confirmación o el conductor vuelve a cerrar a mano. Eso quiere decir que el mecanismo frente al grupo no se sostiene. Si se cumplen a la vez la condición de change y la de discard, prevalece **discard**.
- **Expected provenance:** real
- **Next step if it passes:** piloto de 2 semanas con mago de Oz y 4 a 6 conductores, alternando A1 y A3 en reuniones con decisiones, con seguimiento a 2 semanas de las decisiones ejecutadas distinto o no ejecutadas (creencia #8). Se diseña aparte, con su propio umbral.

## T2. recap-de-decisiones: recap estructurado revisado a solas, con un error sembrado (mago de Oz)
- **Test status:** ready
- **Belief under test:** "Un recap que ordena decisión, responsable, fecha y porqué, y marca lo dudoso, deja la revisión del conductor en < 5 min y no hace llegar a ejecución ninguna decisión inventada. Se cae si la revisión supera los 5 min o si alguna decisión inventada se ejecuta." (#9, `[feature: recap-de-decisiones] [value]`)
- **Risk:** [value]
- **Test type:** wizard-of-oz
- **What we do:**
  1. El conductor elige otra reunión de trabajo real con decisiones y con la transcripción activada. Es la que no usó para T1, en el orden que le haya tocado.
  2. Dentro de las 2 h posteriores, el mago le entrega un recap armado **solo con la transcripción**: la lista de decisiones con responsable, fecha y porqué, y las dudosas marcadas con "¿idea o decisión?".
  3. Antes de entregarlo, el mago siembra **exactamente una** idea de la conversación presentada como decisión firme, sin marca de dudosa. La anota en la clave de respuesta.
  4. El conductor revisa el recap a solas y lo publica donde se ejecuta.
  5. El mago revisa lo publicado **antes de que llegue al equipo**: si la decisión sembrada pasó, la intercepta y la retira.
  6. Después hay un debrief corto con el conductor. Al reclutarlo se le dijo que "el recap puede tener errores, como el de la IA", pero no que había uno sembrado.
- **With whom:** los mismos 6 conductores de T1 (al menos 5 completos), con el mismo reclutamiento y los mismos filtros.
- **Material needed:**
  - **Plantilla de recap:** lista de decisiones con responsable, fecha y porqué, y la marca "¿idea o decisión?".
  - **Reglas del mago:** usa solo la transcripción, siembra un error por recap y lo registra en la clave antes de entregar.
  - **Protocolo de intercepción** antes de que la decisión sembrada llegue al equipo.
  - **Texto de consentimiento** ("el recap puede tener errores") y guion de debrief.
  - **Una forma de medir la revisión** sin observar al conductor: un documento compartido con hora de apertura y hora de publicación, más el tiempo que reporta el conductor.
  - **Hoja de captura por reunión:** hora de entrega, apertura y publicación, minutos de revisión, ítems corregidos o borrados, si detectó el error sembrado (sí o no), si publicó algo dudoso sin resolver, y notas del debrief.
  - **Queda fuera a propósito:** resumen de la conversación, integración y diseño visual.
- **Material:** [`product/tests/materials/t2-recap-de-decisiones/`](materials/t2-recap-de-decisiones/README.md)
- **Duration:** corre en la misma semana que T1. Cada conductor hace sus 2 reuniones en unos 7 días.
- **Signal and threshold:** (a) la revisión dura < 5 min, medida entre la apertura y la publicación; (b) la decisión sembrada no llega publicada. **Umbral: pasa si la revisión dura < 5 min en ≥ 4 de 5 reuniones y el conductor detecta el error sembrado en 5 de 5.** La creencia es de tolerancia cero: una sola decisión inventada que llega a ejecución la hace caer.
- **Decision rule:**
  - **continue** si se cumplen las dos condiciones.
  - **change** si se detectan todos los errores pero la revisión supera los 5 min en 2 o más reuniones (se ajusta el formato y se repite el test), o si pasa exactamente 1 error sembrado (se refuerza la marca de lo dudoso o se exige confirmar cada decisión, y se repite el test).
  - **discard** si pasan ≥ 2 errores sembrados de 5: la revisión a solas no frena los inventos.
- **Expected provenance:** real
- **Next step if it passes:** el mismo piloto de 2 semanas que T1, que mide la #8 con A3 como comparación. Si A1 se descarta y A3 pasa, el siguiente paso es un piloto de A3 solo, con el umbral de mala ejecución a 2 semanas.

## Resultados

## Decisión
