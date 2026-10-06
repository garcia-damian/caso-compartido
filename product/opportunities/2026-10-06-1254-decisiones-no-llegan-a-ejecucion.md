---
status: framed
segment: Cuentas Business Premium con 100 o más licencias, del sector tecnología, con operación en 3 o más países y facturación de más de USD 100M anuales (12.400 cuentas y 2,1 M de licencias, unverified). Equipos distribuidos, remotos o híbridos. Dentro de la cuenta, el rol afectado es quien conduce reuniones de trabajo (5 o más personas, reuniones donde se decide): Team Leads y mandos medios.
personas: lucia-ferreyra, andres-quintero, patricia-oliveira, raul-mendez, martin-sosa, sofia-paz
---

# Oportunidad: lo decidido en la reunión no llega intacto a quien lo ejecuta

En equipos distribuidos de cuentas Premium grandes de tecnología, lo que se decide en una reunión de trabajo se ejecuta mal o no se ejecuta, porque el responsable, la fecha o el porqué quedan ambiguos. El conductor tapa ese hueco a mano después de cada reunión. Pasa igual si se trabaja en Teams, en Miro o en Jira. Importa ahora por dos razones: este es el dolor que la investigación de septiembre encontró en 10 de 10 entrevistas, y es justo el espacio que el mercado deja vacío. En el segmento, solo el 3,1% de las cuentas sube a Max.

Esta oportunidad reemplaza a `colaboracion-fuera-de-teams`, que se descartó porque el dolor no depende de dónde se trabaje.

## Segmento y personas

- **Lucía Ferreyra** (primary): sufre el problema. "Si la reunión termina y nadie sabe quién hace qué, fue una hora perdida para ocho personas."
- **Andrés Quintero** (primary): sufre el problema. "Una decisión que no está escrita donde el equipo la encuentra… es una conversación que alguien va a tener que repetir."
- **Patricia Oliveira** (primary): sufre el problema, del lado del cliente: necesita saber "qué se prometió, quién lo prometió y si se cumplió".
- **Raúl Méndez** (secondary): sufre el efecto. Ejecuta tarde porque se entera tarde.
- **Martín Sosa** (tertiary): no sufre el problema. Es quien responde la creencia de viabilidad.
- **Sofía Paz** (negative): no sufre el problema. Trabaja sola.
- **Falta:** nadie para el problema. Sí falta evidencia `real` **dentro del segmento por tamaño** (ver Señales).

## Señales

| Señal | Procedencia | Fuente |
|---|---|---|
| 10 de 10 conductores cuentan un caso concreto en el que lo decidido se ejecutó mal o no se ejecutó. La falla estuvo entre el final de la reunión y la ejecución, con un costo de 1 a 2 semanas de trabajo, clientes esperando días y releases corridas | `real`* | `product/insights/2026-09-30-1630-entrevistas-colaboracion-en-vivo.md`, insight 1 |
| El conductor cierra a mano: acta, pase a Jira, dueños y fechas. Le lleva de 10 a 60 min por reunión, y 3 de ellos dicen "nadie más lo hace" | `real`* | ídem, insight 1 |
| El recap de IA resume la conversación, no las decisiones, y a veces inventa decisiones: 2 casos terminaron en trabajo perdido. Quien lo usa lo reescribe (de 10 a 30 min) | `real`* | ídem, insight 2 |
| Lo decidido pasa igual en Teams, Miro, FigJam, Jira y Confluence | `real`* | ídem, insight 1 y "Recurrencia" |
| "Registro y continuidad" es el tema nº 1 de las respuestas abiertas: 35% (n=95) | `survey` | `product/insights/2026-09-30-1621-colaboracion-en-vivo-fuera-de-teams.md`, O3 |
| El 31% de las decisiones queda sin registro recuperable (en ningún lado, o solo en un chat fuera de Teams), n=182 | `survey` | ídem, O3 |
| El 39% conoce el resumen de IA y nunca lo usó. El recap aparece de forma espontánea en "Otro", con quejas | `survey` | ídem, O4 y O3 |
| 4 conductores no lo viven como problema de herramienta: lo atribuyen a disciplina o a exceso de reuniones, aunque tienen el mismo dolor | `real`* | entrevistas, "Recurrencia y contrapuntos" |
| Decidir durante la reunión y dejar un registro consultable entre reuniones es un espacio casi vacío. El resumen posterior es commodity | `secondary` | `product/research/2026-09-23-1508-colaboracion-fuera-de-teams.md`, §4 |
| Los registros automáticos de IA producen un "registro con apariencia de autoridad", a menudo erróneo | `secondary` | ídem, §4 |
| Lucía rearma minuta y pendientes a mano unas 4 h por semana | `synthetic` | `product/personas/lucia-ferreyra.md` |
| Segmento de 12.400 cuentas y 2,1 M de licencias. Upgrade Premium → Max del 3,1% en 12 meses | `unverified` | brief del caso |

\* **Fuera del segmento por tamaño.** Los entrevistados son de SaaS B2B, distribuidos en 3 o 4 países, pero trabajan en empresas de 650 a 2.000 empleados, y Business Premium tiene un tope de 300 usuarios (`secondary`, research). Sirven como señal fuerte del problema, no como prueba para el segmento. Además, la firmografía de la encuesta es autodeclarada, y hay que verificar la identidad de R-170 y las fechas de la entrevista de Paula Benítez.

## Resultado de negocio

**Tasa de upgrade Premium → Max** en el segmento: hoy 3,1% en 12 meses (`unverified`). La evidencia `secondary` (enterprise) dice que el upsell de Microsoft lo mueven la IA en bundle y la seguridad, no el uso, y que el ROI por uso es esquivo para IT. Todavía no está definido qué es "Max" para una cuenta Business Premium: puede ser Business Premium + Copilot o el salto a E3/E5/E7.

## Restricciones

- Presupuesto máximo: USD 5M.
- CollabCon en unos 20 semanas (≈ 22/02/2027): ahí se presentan los features.
- El empleado recibe Teams instalado y no elige: nada que dependa de que el usuario instale o contrate algo aparte.
- Cumplimiento multi-país: residencia de datos, retención y políticas de invitados externos. En España/UE, compliance limita las herramientas externas (`survey`, insight 6).
- Límites de cualquier solución: facilidad de uso, accesibilidad, compatibilidad con Microsoft 365, privacidad y seguridad corporativas, tiempo real e impacto mínimo en el rendimiento de la reunión.
- Hecho de producto: hoy, en Business Premium, el recap y Facilitator están detrás de Teams Premium o Copilot, y Facilitator no funciona con externos (`secondary`, research §1).

## Creencias

Registradas en `product/overview.md`, que es el único registro (pendientes de aprobación):

- `[opportunity: decisiones-no-llegan-a-ejecucion] [value]` En el segmento, en al menos 1 de cada 4 reuniones de trabajo con decisiones, alguna se ejecuta distinto de lo decidido o no se ejecuta porque el responsable, la fecha o el porqué quedaron ambiguos, y el conductor dedica 10 min o más por reunión a cerrarlas a mano. Se cae si una medición en el segmento da menos que eso.
- `[opportunity: decisiones-no-llegan-a-ejecucion] [viability]` IT del segmento usa "las decisiones de reunión llegan a ejecutarse" como argumento ante finanzas para justificar Max. Se cae si IT declara que el tier se decide por precio, bundle, negociación o seguridad, sin que eso pese.
- Referencias: `[product] [value]` #4 del overview (quienes convocan le sacan más valor a Teams). Esta oportunidad es la primera que pone el foco en el conductor.

## Agenda de research

| Creencia | Instrumento | Decisión que desbloquea | Para cuándo |
|---|---|---|---|
| viability | Datos internos: definir qué es "Max" para Business Premium y ver qué tienen en común las cuentas del 3,1% que subieron | Si "Max" no incluye la capa de IA o el uso no separa a quienes suben, cambiar el resultado a retención antes de seguir | semana 1 (≈ 13/10) |
| value | Datos internos: telemetría del segmento (recaps generados y abiertos, reuniones con decisiones sin tareas creadas después) y tickets de soporte sobre recap y notas | Si en datos propios no se ve el hueco entre la reunión y la ejecución, bajar la prioridad de la oportunidad | semana 1–2 |
| viability | 6 a 8 entrevistas con admins de IT del segmento, de cuentas que subieron de tier y de cuentas que no | Si el upgrade es una palanca alcanzable con este problema o si hay que cambiar de resultado | semana 2–4 |
| value | Encuesta corta (`/design-survey`) a conductores del segmento, filtrada a Business Premium de 100 a 300 licencias (n ≥ 150): en la última reunión de trabajo, cuántas decisiones hubo, cuántas se ejecutaron distinto, cuántos minutos llevó el cierre a mano. Sumar la opción "recap de IA" a la pregunta de registro | Si se cumple el umbral de 1 de cada 4 reuniones y 10 min dentro del segmento | semana 2–4 |
| value | 6 a 8 entrevistas (`/design-interview`) con conductores del segmento por tamaño, reclutados de la encuesta, priorizando a quienes no sienten el dolor o lo atribuyen a disciplina | Abrir la oportunidad a `/explore-solutions` con evidencia `real` dentro del segmento | semana 4–6 |

Discovery tiene que cerrar alrededor de la semana 6 (mediados de noviembre) para dejar margen hasta CollabCon.

## Ideas candidatas (no evaluadas)

Surgieron de la exploración hecha sobre la oportunidad anterior (2026-10-06, sin guardar). Acá quedan sin evaluar, para competir en `/explore-solutions`.

- Tarjeta de cierre con decisión, responsable, fecha y porqué, armada por IA y confirmada por el conductor antes de cortar, publicada donde se ejecuta.
- Ritual de cierre de 5 minutos con plantilla de Loop fijada en el canal, sin software nuevo.
- Recap de IA que separe lo decidido de lo conversado y marque lo dudoso.
- Notas y pizarra ancladas a la serie o al canal, con historial entre sesiones.
- Recoger la posición de quien no habló antes de cerrar.
- Notas en vivo que dejen decisiones y responsables asentados solos (heredada del brief anterior).
