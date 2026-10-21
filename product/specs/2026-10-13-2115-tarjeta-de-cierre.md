---
feature: tarjeta-de-cierre
status: draft (decisiones de detalle cerradas 2026-10-13)
opportunity: product/opportunities/2026-10-06-1254-decisiones-no-llegan-a-ejecucion.md
solutions: product/solutions/2026-10-06-2019-decisiones-no-llegan-a-ejecucion.md
tests: product/tests/2026-10-06-2056-decisiones-no-llegan-a-ejecucion.md
---

# Tarjeta de cierre

## Problema

En las reuniones de trabajo, lo que se decide se ejecuta mal o no se ejecuta, porque el responsable, la fecha o el porqué quedan ambiguos. Se descubre días después y cuesta de 1 a 2 semanas de trabajo, clientes esperando y releases corridas. Hoy el conductor tapa el hueco a mano después de la reunión (de 10 a 60 min), cuando el grupo ya no está para aclarar nada. El recap de IA no lo resuelve: resume la conversación, no las decisiones, y a veces inventa decisiones.

> Evidencia: "el líder de Ecuador entendió que lo pasaba yo, y yo entendí que lo pasaba él. Nadie lo pasó" — Andrés (R-170, identidad sin verificar), insights/2026-09-30-1630, insight 1
> Evidencia: "Yo pensé que el arquitecto iba a hacer el ADR y él pensó que yo lo iba a mandar por correo" — Ricardo, insight 1
> Evidencia: el recap "no me dice quién se comprometió a qué" — Lucía Fernández, insight 2
> Evidencia: el 31% de las decisiones queda sin registro recuperable (n=182) — encuesta, insights/2026-09-30-1621, O3

Toda la evidencia `real` es de empresas de 650 a 2.000 empleados, fuera del tope de 300 de Business Premium. Es señal fuerte del problema, no prueba para el segmento (ver *Supuestos*, #3).

## Para quién

- **Lucía Ferreyra** (primaria): conduce de 10 a 15 reuniones por semana y hoy cierra cada una a mano. Es quien confirma la tarjeta.
- **Andrés Quintero y Patricia Oliveira** (primarias): conducen reuniones donde se decide; Patricia necesita saber "qué se prometió, quién lo prometió y si se cumplió" del lado del cliente.
- **Raúl Méndez** (secundaria): no usa la tarjeta, pero recibe su efecto. Hoy ejecuta tarde porque se entera tarde.

## Recorrido del usuario (Lucía)

1. **Disparador:** Lucía conduce una reunión de trabajo de 8 o 9 personas con la transcripción activada. Se toman dos o tres decisiones mientras ella comparte el Excel de seguimiento y dicta lo que le piden. *(insight 4: el conductor es el único que toca el contenido)*
2. **A unos 5 minutos del final programado**, Teams le muestra solo a ella un borrador de tarjeta armado con la transcripción: cada decisión con responsable, fecha y porqué. Lo que la transcripción no deja claro aparece marcado como dudoso, vacío.
3. **Comparte la tarjeta** en la reunión, sin salir de la llamada, y la lee en voz alta. *(momento donde cae el valor: el grupo todavía está)*
4. **El grupo corrige en vivo:** "eso lo paso yo, no él", "la fecha es el jueves". Lucía edita los campos y resuelve cada dudoso, o descarta lo que era una idea y no una decisión. *(insight 1: responsable ambiguo; insight 2: ideas confundidas con decisiones)*
5. **Confirma y publica** antes de cortar. Las decisiones confirmadas se publican donde el equipo ejecuta: el canal del equipo, Planner o Jira.
6. **Resultado:** Lucía corta la llamada sin acta pendiente. Cada responsable escuchó que la decisión es suya y la encuentra donde trabaja. No hay cierre a mano después.

Supuesto, no evidencia: que la tarjeta lista a 5 minutos del final alcance para confirmar dentro del tiempo de la reunión (#7) y que el grupo corrija en vivo en vez de dejarlo "para después".

## Historias críticas

### Borrador de tarjeta listo antes del final
Como Lucía, quiero ver antes de que termine la reunión un borrador con cada decisión, su responsable, su fecha y su porqué, para no tener que armar el acta después.

Criterios de aceptación:
- [ ] A 5 minutos del final programado, el borrador aparece solo para el conductor, sin que nadie más lo vea hasta que lo comparta.
- [ ] El conductor puede pedir el borrador antes, en cualquier momento de la reunión.
- [ ] Cada decisión tiene cuatro campos: decisión, responsable, fecha y porqué.
- [ ] Un campo que la transcripción no deja claro queda vacío y marcado como dudoso; nunca se completa con un valor que no esté en la transcripción.
- [ ] Si no se detectan decisiones, la tarjeta lo dice y permite agregar una a mano.
- [ ] La tarjeta no incluye un resumen de la conversación.

Traza a: insight 1 (cierre a mano, 10 a 60 min) e insight 2 (el recap confunde ideas con decisiones y las inventa).

### Confirmar frente al grupo
Como Lucía, quiero compartir la tarjeta en la reunión y corregirla con el grupo presente, para que la ambigüedad se resuelva mientras todavía están todos.

Criterios de aceptación:
- [ ] La tarjeta se comparte dentro de la reunión, sin abrir otra app ni otra ventana.
- [ ] Todos los participantes de la organización ven la tarjeta compartida mientras el conductor la edita.
- [ ] El conductor puede editar cualquier campo, marcar cada decisión como confirmada o descartarla.
- [ ] No se puede confirmar una decisión que tenga un campo marcado como dudoso sin resolverlo antes.
- [ ] Si la reunión termina sin confirmar, la tarjeta queda como borrador, no se publica nada y el conductor la encuentra en el chat de la reunión.

Traza a: insight 1 ("que todos lo vean antes de cortar la llamada") e insight 4 (el conductor es el único que toca el contenido).

### Publicar donde se ejecuta
Como Lucía, quiero que lo confirmado se publique en el canal del equipo, Planner o Jira, para que cada responsable lo encuentre donde trabaja sin que yo lo pase a mano.

Criterios de aceptación:
- [ ] Solo se publican las decisiones confirmadas.
- [ ] El conductor elige el destino una vez por serie de reuniones, y la serie lo recuerda.
- [ ] En Planner o Jira, cada decisión se publica como una tarea con el responsable asignado y la fecha.
- [ ] Cada decisión publicada incluye el porqué y un enlace a la reunión.
- [ ] Si el responsable no se puede asignar en el destino (no tiene cuenta en Jira o es externo), la decisión se publica con su nombre como texto y queda marcada para el conductor.

Traza a: insight 1 ("que se publique donde se ejecuta: Jira, el canal o el correo") e insight 5 (el registro vive donde ya vive el artefacto).

## Hipótesis

Creemos que los conductores de reuniones de trabajo en cuentas Business Premium del segmento van a confirmar la tarjeta frente al grupo antes de cortar, en la mayoría de las reuniones con decisiones, y van a dejar de cerrar a mano después, porque el cierre a mano les cuesta tiempo y no resuelve la ambigüedad: cuando escriben el acta, el grupo ya no está.

Estamos equivocados si la confirmación se saltea o se pasa a "después" en más de 3 de cada 10 reuniones con decisiones, si toma más de 3 minutos, o si a las 2 semanas la proporción de decisiones ejecutadas distinto o no ejecutadas no es menor que con el recap estructurado posterior.

## Deliberadamente no

- No resume la conversación.
- No reemplaza a Jira ni a Planner: publica ahí.
- No publica nada sin la confirmación del conductor.
- No pide aceptación al responsable (eso es A5, en espera).

## Alternativas consideradas

Exploradas en: product/solutions/2026-10-06-2019-decisiones-no-llegan-a-ejecucion.md
- A2 ritual-de-cierre — descartada: el ritual sin herramienta ya falla hoy (4 de 10 conductores lo leen como disciplina y aun así sufren el problema) y no mueve el upgrade.
- A3 recap-de-decisiones — en test en paralelo (T2), como comparación para la #8.
- A4 artefactos-de-la-serie — en espera: ataca la minoría de los casos (registro perdido, no responsable ambiguo).
- A5 acuse-del-responsable — en espera: posible paso 2 de esta tarjeta.
- Recoger la posición de quien no habló — en espera: ataca la legitimidad de la decisión; puede ser su propia oportunidad.
- Notas en vivo que dejan decisiones asentadas solas — integrada en esta tarjeta, con confirmación.

## Probado antes del spec

Probado en: product/tests/2026-10-06-2056-decisiones-no-llegan-a-ejecucion.md
- La creencia más riesgosa no se probó (declarado): T1 (tarjeta confirmada en vivo, mago de Oz) está diseñado pero no corrió. La #7 sigue abierta.
- T1 y la #8 (comparación a 2 semanas) quedan como próximos pasos.

## Supuestos

Registrados en `product/overview.md`:
- #7 [feature: tarjeta-de-cierre] [value] Con un borrador armado a partir de la transcripción, el conductor confirma la tarjeta frente al grupo en ≤ 3 min en al menos 7 de cada 10 reuniones con decisiones, y no vuelve a cerrar a mano después. **No probado.**
- #8 [feature: tarjeta-de-cierre] [value] Confirmar en vivo deja menos decisiones ejecutadas distinto o no ejecutadas a las 2 semanas que el recap estructurado posterior.
- #3 [opportunity: decisiones-no-llegan-a-ejecucion] [value] El problema ocurre en el segmento (≥ 1 de cada 4 reuniones con decisiones, ≥ 10 min de cierre a mano).
- #2 [opportunity: decisiones-no-llegan-a-ejecucion] [viability] IT usa "las decisiones llegan a ejecutarse" para justificar Max.
- #10 [feature: tarjeta-de-cierre] [feasibility] Se puede extraer de la transcripción, en vivo, decisión, responsable, fecha y porqué, a tiempo y sin confundir ideas con decisiones en más de 1 de cada 10 ítems.
- #11 [feature: tarjeta-de-cierre] [feasibility] Desde una reunión en Business Premium se puede publicar en Planner, Jira y el canal con responsable y fecha asignados.
- #12 [feature: tarjeta-de-cierre] [usability] El conductor comparte la tarjeta y corrige un campo con el grupo sin ayuda.
- #13 [feature: tarjeta-de-cierre] [viability] Funciona con lo que trae Max, sin licencia por participante, y sirve en reuniones con externos.
