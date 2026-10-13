---
opportunity: decisiones-no-llegan-a-ejecucion
status: testing-several
chosen: tarjeta-de-cierre, recap-de-decisiones
tests: product/tests/2026-10-06-2056-decisiones-no-llegan-a-ejecucion.md
---

# Soluciones para: lo decidido en la reunión no llega intacto a quien lo ejecuta

Oportunidad: `product/opportunities/2026-10-06-1254-decisiones-no-llegan-a-ejecucion.md`

## Qué dice hoy la evidencia

- Las dos creencias de la oportunidad (#2 viability y #3 value en `product/overview.md`) siguen abiertas: ninguna tiene anotación y ninguna está `contradicted`.
- **[value]** La evidencia más fuerte es `real`: 10 de 10 conductores contaron un caso concreto, y el cierre a mano les lleva de 10 a 60 min por reunión (E, insight 1). Pero los entrevistados están **fuera del segmento por tamaño**: trabajan en empresas de 650 a 2.000 empleados, y Business Premium tiene un tope de 300. La encuesta lo respalda: el 31% de las decisiones queda sin registro recuperable y "registro y continuidad" es el tema nº 1 de las respuestas abiertas, con el 35% (S, O3).
- **[viability]** Sin evidencia: todavía no se definió qué es "Max" y no hubo conversación con IT.
- Esta exploración se adelantó a la agenda de research: el brief pedía llegar con evidencia `real` dentro del segmento (semanas 4 a 6). Además, la identidad de R-170 (Andrés) sigue sin verificar.

Fuentes: **E** = `product/insights/2026-09-30-1630-entrevistas-colaboracion-en-vivo.md` · **S** = `product/insights/2026-09-30-1621-colaboracion-en-vivo-fuera-de-teams.md` · **R** = `product/research/2026-09-23-1508-colaboracion-fuera-de-teams.md`. El asterisco (`real`*) marca evidencia real de fuera del segmento por tamaño.

## Baseline: qué se hace hoy

El conductor cierra a mano después de la reunión: arma el acta, pasa las decisiones a Jira y asigna dueños y fechas. Le lleva de 10 a 60 min por reunión, y 3 de los entrevistados dicen que "nadie más lo hace" (`real`*, E 1). Si usa el recap de IA, lo reescribe (de 10 a 30 min) o lo abandona (`real`*, E 2). El 24% de las decisiones no queda registrado en ningún lado (`survey`, S O3).

## Alternativas

### A1. Tarjeta de cierre confirmada en vivo (`tarjeta-de-cierre`)
La IA arma un borrador con la decisión, el responsable, la fecha y el porqué. En los últimos minutos, el conductor lo confirma frente a todos y se publica donde se ejecuta (Jira, el canal o Planner). Ataca la ambigüedad en el único momento en que todavía se puede resolver con el grupo presente. Es para Lucía Ferreyra, Andrés Quintero y Patricia Oliveira (primary), y reemplaza el acta a mano. Absorbe la idea candidata "notas en vivo que dejan decisiones asentadas solas": comparten el mecanismo, pero esa idea no tenía confirmación, y la evidencia dice que la IA sin confirmar inventa decisiones (E 2).

### A2. Ritual de cierre con plantilla de Loop (`ritual-de-cierre`)
No requiere software nuevo: una plantilla fijada en el canal y 5 minutos al final de la reunión para leer y completar en voz alta la decisión, el responsable, la fecha y el porqué. Es la más chica que podría funcionar. Es para Lucía y Andrés, y reemplaza el acta posterior.

### A3. Recap que separa lo decidido de lo conversado (`recap-de-decisiones`)
Después de la reunión, el recap ordena las decisiones con responsable, fecha y porqué, y marca lo dudoso ("¿idea o decisión?"). El conductor lo revisa a solas antes de publicarlo. Ataca la calidad del registro, no el momento en que se hace. Es para Lucía y Andrés, y reemplaza la reescritura del recap actual.

### A4. Notas y pizarra ancladas a la serie o al canal (`artefactos-de-la-serie`)
Lo decidido sobrevive a la reprogramación y se retoma en la sesión siguiente. Ataca la decisión enterrada o perdida (E 3), no la ambigüedad sobre el responsable. Es para Lucía (que trabaja con compliance) y Patricia, y reemplaza la vuelta a Miro para tener continuidad.

### A5. Acuse del responsable (`acuse-del-responsable`)
Cada decisión que tiene dueño le llega a esa persona, que la acepta, la rechaza o pide el porqué. Lo que nadie acepta en 24 h vuelve al conductor. Así, el cierre pasa del conductor a quien ejecuta. Ataca el "yo pensé que lo hacía él" (los casos de Andrés y Ricardo). Es para Raúl Méndez (secondary), y le saca carga a Lucía y Andrés.

## Comparación

| Alternativa | Desirable | Feasible | Viable | Creencia más riesgosa |
|---|---|---|---|---|
| A1 tarjeta-de-cierre | mixed (`real`*, E 1 y 2: pain evidenced, relief not tested) | to check with tech (Facilitator ya hace notas en vivo, pero no funciona con externos y la publicación en Jira o Planner está sin confirmar; `secondary`, R §1) | mixed (`secondary`, R y brief: el upsell lo mueve la IA en bundle, pero "Max" no está definido) | Con un borrador de IA, el cierre frente al grupo toma ≤ 3 min y se hace en la mayoría de las reuniones con decisiones |
| A2 ritual-de-cierre | mixed (`real`*, E: 4/10 lo leen como disciplina y aun así fallan; `survey`, S O4: el 31% no sabe que Loop existe) | strong (`secondary`, R §1: Loop ya está en el plan base) | weak (`assumption`: está en el plan base y no empuja a Max) | El conductor sostiene los 5 min en ≥ 3 de cada 4 reuniones sin una herramienta que lo empuje |
| A3 recap-de-decisiones | mixed (`real`*, E 2: 6/10 abandonan el recap; `survey`, S O4: el 39% lo conoce y nunca lo usó. Pero llega con el grupo ya disperso) | to check with tech | mixed (`secondary`, R §1 y §4: está detrás de Teams Premium o Copilot, pero el resumen posterior es commodity) | Un recap estructurado deja la revisión en < 5 min y no hace llegar a ejecución ninguna decisión inventada |
| A4 artefactos-de-la-serie | mixed (`real`*, E 3: 6/10 dejan la pizarra porque se pierde; pero solo 2 o 3 de los 10 casos de E 1 son de registro perdido) | to check with tech | weak (`assumption`) | La mayoría de las fallas vienen de un registro perdido, no de un responsable ambiguo |
| A5 acuse-del-responsable | mixed (`real`* para el dolor; `assumption` para la adopción) | to check with tech | unknown (`assumption`) | Los responsables aceptan o rechazan en < 24 h y no lo ignoran como un mail más |

## Decisión

**Recomendación de la IA:** probar A1 + A2 en paralelo. A2 funcionaba como piso barato que el software tiene que superar, y A1 es la única alternativa que conecta con la palanca de IA en bundle.

**Decisión de Damián (2026-10-06):** probar **A1 + A3** en paralelo. Motivo: A2 ya se sabe que falla. 4 de 10 conductores leen el problema como falta de disciplina y aun así lo sufren, así que el ritual sin herramienta ya está refutado. La pregunta que queda es si confirmar en vivo le gana a un recap posterior mejor hecho. La diferencia con la recomendación quedó registrada en `product/corrections.md`.

**Test:** ver `product/tests/2026-10-06-2056-decisiones-no-llegan-a-ejecucion.md` (T1 para A1 → creencia #7, T2 para A3 → creencia #9; el piloto de 2 semanas que mide la #8 queda como siguiente paso si pasan).

## Propuesta de valor: tarjeta-de-cierre (A1)

- **Dolor que alivia:** el responsable, la fecha o el porqué quedan ambiguos y se descubre días después. Cuesta de 1 a 2 semanas de trabajo, clientes esperando y releases corridas, y además el cierre a mano le lleva al conductor de 10 a 60 min (`real`*, E 1).
- **Ganancia que crea:** Lucía corta la llamada con la decisión ya publicada en Jira o en el canal, y cada responsable sabe que es suyo porque lo escuchó confirmar.
- **Reemplaza:** el acta y el pase a Jira después de la reunión. La gente cambiaría porque el workaround cuesta tiempo después de la reunión y no resuelve la ambigüedad: cuando el conductor escribe el acta, el grupo ya no está.
- **Deliberadamente no:** no resume la conversación, no reemplaza a Jira ni a Planner (publica ahí) y no publica nada sin la confirmación del conductor.

## Propuesta de valor: recap-de-decisiones (A3)

- **Dolor que alivia:** el recap actual resume la conversación, no las decisiones, y a veces las inventa: 2 casos terminaron en trabajo perdido. El conductor lo reescribe (de 10 a 30 min) o lo abandona (`real`*, E 2; `survey`, S O3 y O4).
- **Ganancia que crea:** Andrés revisa en pocos minutos una lista de decisiones con responsable y fecha, con lo dudoso marcado, en lugar de reescribir un resumen.
- **Reemplaza:** la reescritura del recap o el acta a mano. La gente cambiaría porque no le pide nada al grupo durante la reunión.
- **Deliberadamente no:** no interviene durante la reunión y no publica nada sin la revisión del conductor.

## Creencias

Referencias:
- `[opportunity: decisiones-no-llegan-a-ejecucion] [value]` #3 en `product/overview.md`.
- `[opportunity: decisiones-no-llegan-a-ejecucion] [viability]` #2 en `product/overview.md`.

Propuestas (las que resuelve el test; pendientes de aprobación para el registro):
- `[feature: tarjeta-de-cierre] [value]` Con un borrador armado a partir de la transcripción, el conductor confirma la tarjeta frente al grupo en ≤ 3 min en al menos 7 de cada 10 reuniones con decisiones, y no vuelve a cerrar a mano después. Se cae si la confirmación supera los 3 min o se saltea en más de 3 de cada 10 reuniones.
- `[feature: tarjeta-de-cierre] [value]` Confirmar en vivo deja menos decisiones ejecutadas distinto o no ejecutadas a las 2 semanas que el recap estructurado posterior. Se cae si la tasa no es menor que con `recap-de-decisiones`.
- `[feature: recap-de-decisiones] [value]` Un recap que ordena decisión, responsable, fecha y porqué, y marca lo dudoso, deja la revisión del conductor en < 5 min y no hace llegar a ejecución ninguna decisión inventada. Se cae si la revisión supera los 5 min o si alguna decisión inventada se ejecuta.

## Descartadas o en espera

- **A2 ritual-de-cierre — discarded:** el ritual sin herramienta ya falla hoy, porque 4 de 10 conductores lo atribuyen a disciplina y aun así sufren el problema (`real`*, E). Además, no mueve el upgrade. Decisión de Damián, en contra de la recomendación (ver *Decisión*).
- **A4 artefactos-de-la-serie — parked:** ataca la minoría de los casos (registro perdido, no responsable ambiguo). Vuelve si codificar los casos muestra que la pérdida pesa más, o como mejora de continuidad en cuentas con compliance.
- **A5 acuse-del-responsable — parked:** depende de que el responsable ya esté cargado. Es un posible paso 2 de A1 o A3.
- **Recoger la posición de quien no habló — parked:** ataca la legitimidad de la decisión (E 4), no que llegue intacta. Puede ser su propia oportunidad.
- **Notas en vivo que dejan decisiones asentadas solas — merged** en A1: es el mismo mecanismo sin confirmación, y la evidencia dice que la IA sin confirmar inventa decisiones.
