---
opportunity: colaboracion-fuera-de-teams
status: chosen
chosen: cierre-de-decisiones
---

# Soluciones para: la colaboración en vivo se hace fuera de Teams

## Qué dice hoy la evidencia

- **[value] de la oportunidad: `weakened`, y además reencuadrada.** El dolor principal es el **cierre**: la decisión no llega intacta a quien la ejecuta. Aparece en 10/10 entrevistas (`real`, `product/insights/2026-09-30-1630-entrevistas-colaboracion-en-vivo.md`, insight 1), en el 35% de las respuestas abiertas y en el 31% de casos sin registro recuperable (`survey`, `product/insights/2026-09-30-1621-colaboracion-en-vivo-fuera-de-teams.md`). Pasa igual dentro y fuera de Teams. Lo que sale de Teams es sobre todo trabajo que ya vivía afuera: el 74% de los artefactos sin pizarra ya existía (`survey`, O1).
- **Hipótesis rivales.** Los externos son minoría: 4% de las quejas y 1 de 10 entrevistas. El hábito explica en parte la elección de Miro ("costumbre"), pero no explica el dolor del cierre.
- **[viability]: abierta, con evidencia en contra.** En enterprise, el upgrade se decide por descuento, seguridad e IA en bundle, y el ROI por uso es esquivo (`secondary`, `product/research/2026-09-23-1508-colaboracion-fuera-de-teams.md`, §3). Esto todavía no está anotado en el overview. Faltan las entrevistas con IT y no está definido qué es "Max".
- **Calidad de la evidencia.** Falta verificar la identidad de R-170 (Andrés Quintero) y las fechas de la entrevista de Paula Benítez. Ningún juicio de este archivo se apoya solo en ellos.

## Línea de base: lo que se hace hoy

El conductor cierra a mano: escribe el acta y pasa las tareas a Jira, con un costo de 10 a 60 min por reunión. Tres conductores dicen textualmente que "nadie más lo hace" (`real`, insight 1). El recap de IA se conoce y se abandona o se reescribe: Javier tarda 30 min, Paula más de 10 (`real`, insight 2), y el 39% de los encuestados lo conoce pero nunca lo usó (`survey`, O4). Los ejercicios con estructura se hacen en Miro o FigJam, con 5 a 10 min de acceso por sesión. Los demás le dictan al conductor y votan a mano alzada (`real`, insights 4 y 5). Cuando nadie cierra, la decisión queda en un chat fuera de Teams o en ningún lado: 31% de los casos (`survey`, O3).

## Alternativas

### A1. Cierre de decisiones confirmado (`cierre-de-decisiones`)

Antes de cortar la llamada, Teams arma una tarjeta con **decisión, responsable, fecha y porqué**. La arma con el audio y con el artefacto que estuvo en pantalla, y marca lo dudoso ("¿idea o decisión?"). El conductor la confirma con todos presentes y la tarjeta se publica donde se ejecuta: Jira, el canal o el correo.

- **Qué ataca:** el cierre y el recap que no sirve.
- **Para quién:** Lucía Ferreyra y Andrés Quintero (primarias, conductores). También le sirve a Raúl Méndez (secundaria), que se entera tarde.
- **Qué reemplaza:** el acta manual y el recap reescrito.
- Absorbe la idea en pausa "notas en vivo que dejen decisiones y responsables asentados".

### A2. Capa de interacción sobre lo compartido (`interaccion-en-vivo`)

Cualquiera puede señalar, votar (con votos limitados) y agrupar sobre el contenido compartido: una fila de Jira, un gráfico, una pizarra con plantillas. Los votos se cuentan solos.

- **Qué ataca:** que el conductor sea el único que toca el contenido, y que haya gente que no opina.
- **Para quién:** conductores y participantes.
- **Qué reemplaza:** dictar al conductor, la mano alzada, salir a Miro o Slido.
- Absorbe tres ideas en pausa: el pedido original (herramientas colaborativas integradas), la pizarra compartida y la agenda viva con votación.

### A3. Artefactos anclados a la serie (`continuidad-de-artefactos`)

Lo más chico que podría funcionar. Las notas y la pizarra que ya existen dejan de colgar del chat de una reunión y pasan a vivir en la serie o el canal, con historial entre sesiones.

- **Qué ataca:** la razón por la que se abandona lo nativo.
- **Para quién:** conductores, sobre todo en cuentas con compliance.
- **Qué reemplaza:** el tablero trimestral de Miro.

### A4. Ritual de cierre con plantilla, sin software (`ritual-de-cierre`)

En los últimos 5 minutos se leen en voz alta decisión, responsable, fecha y porqué, sobre una plantilla de Loop fijada en el canal. Se acompaña con una campaña para dar a conocer lo nativo.

- **Qué ataca:** el cierre, con herramientas que ya existen.
- **Qué reemplaza:** el acta posterior.

### A5. Panel de coordinación para IT (`panel-it-coordinacion`)

Muestra a IT cuánta coordinación ocurre dentro de Teams y cuánta se desplaza afuera.

- **Qué ataca:** la viabilidad, no el dolor del usuario.
- **Para quién:** Martín Sosa (terciaria, comprador).
- Viene de la idea en pausa del mismo nombre.

### A6. Entrada de externos en un click (`externos-un-click`)

- **Qué ataca:** el acceso de gente de afuera.
- **Para quién:** Patricia Oliveira (primaria).
- Se descartó antes de evaluar (ver *Descartadas o en pausa*).

## Comparación

| Alternativa | Deseable | Factible | Viable | Creencia más riesgosa |
|---|---|---|---|---|
| A1 `cierre-de-decisiones` | **strong**. Insight 1: 10/10 cuentan un cierre que falló, con 1 a 2 semanas perdidas (`real`). Insight 2: 6/10 abandonan el recap (`real`). O3: 35% de las abiertas y 31% sin registro (`survey`) | **to check with tech**. Facilitator ya extrae decisiones, pero exige Copilot y no funciona con externos (`secondary`, research §1). Usar el contexto del artefacto y publicar en Jira: sin evidencia | **mixed**. El upsell lo mueve la IA en bundle (`secondary`, research §3). La creencia de viabilidad tiene evidencia en contra (`secondary`, enterprise). "Max" sin definir (`assumption`) | En reuniones de trabajo, el conductor confirma la tarjeta antes de cortar y la corrige en menos tiempo del que le llevaba escribir el acta |
| A2 `interaccion-en-vivo` | **mixed**. Insight 4: 8/10 dictan o votan a mano alzada (`real`). O3: votar o priorizar 40% (`survey`). Miro ya lo resuelve | **to check with tech**. Interactuar en tiempo real sobre contenido de terceros, con impacto mínimo en el rendimiento de la reunión (restricción del brief) | **unknown** (`assumption`) | Quienes no controlan la pantalla actúan sobre el contenido cuando pueden. En contra: la app dentro de Teams dejó a alguien afuera en 13 de 15 casos (`survey`, n chico) |
| A3 `continuidad-de-artefactos` | **mixed**. Insight 3: 4 perdieron acuerdos al reprogramar (`real`). O4: 43% dejó la pizarra (`survey`). Sin votación ni plantillas no alcanza. Es fuerte con compliance | **to check with tech**. Residencia y retención de datos multi-país | **weak**. Es un arreglo de base, como mucho sirve para retención (`assumption`) | Perder el artefacto es la razón por la que se abandona lo nativo |
| A4 `ritual-de-cierre` | **mixed**. Lleva el cierre a la vista de todos (`real`, insight 1). 4 lo leen como problema de disciplina (`real`). Pero la carga sigue en el conductor y no arregla el recap | **strong**. Las notas de Loop ya vienen en Business Premium base (`secondary`, research §1) | **weak** (`assumption`) | Los conductores sostienen el ritual sin una herramienta nueva |
| A5 `panel-it-coordinacion` | **weak**. No alivia al conductor. La evidencia es solo `synthetic` (Martín Sosa) | **to check with tech**. Hay límites de privacidad, y la telemetría ve cerca de la mitad de los casos (`survey`, O2) | **weak**. Upgrade por descuento y seguridad, el shadow IT que preocupa es la IA (`secondary`, research §3) | IT usa datos de coordinación para justificar el upgrade ante finanzas |

## Decisión

**Damián eligió A1 `cierre-de-decisiones`, el 2026-10-06. Coincide con la recomendación.** En el medio consideró probar A1 y A4 en paralelo, y volvió a A1 sola.

**Por qué A1:**

- Es la única alternativa que ataca el dolor presente en 10/10 entrevistas y en el tema principal de la encuesta.
- Le gana a la línea de base con números concretos: semanas de trabajo perdidas y entre 10 y 60 min de acta por reunión.
- Ocupa un espacio que el mercado deja casi vacío: decidir durante la reunión y dejar un registro consultable (`secondary`, research §4).
- La confirmación del conductor responde al riesgo de un "registro con apariencia de autoridad".

**Qué cambiaría la decisión:**

- Que tech diga que una tarjeta confiable, armada con el contexto del artefacto, no llega antes de CollabCon. En ese caso, A4 + A3.
- Que "Max" no incluya Copilot. Entonces la viabilidad pasa a `weak` y antes de construir hay que volver a research para resolver la creencia de viabilidad.

## Propuesta de valor: `cierre-de-decisiones`

Escrita para el conductor de reuniones de trabajo (Lucía Ferreyra y Andrés Quintero, primarias).

- **Dolor que alivia:** la decisión no llega intacta a quien la ejecuta. Hay responsables ambiguos, decisiones enterradas y registros que llegan tarde, con 1 a 2 semanas de trabajo perdidas (`real`, insight 1). El conductor escribe el acta a mano, de 10 a 60 min por reunión (`real`). El recap resume la conversación, no las decisiones, y a veces las inventa (`real`, insight 2).
- **Ganancia:** todos ven y aceptan lo decidido (quién, qué, cuándo y por qué) antes de cortar. Quien no estuvo lo encuentra donde ejecuta. El conductor deja de escribir el acta después de la reunión.
- **Qué reemplaza:** el acta manual, el pase a Jira a mano y el recap reescrito o ignorado. El conductor cambiaría porque obtiene lo mismo dentro de la reunión, sin trabajo posterior, y con la confirmación de los demás, algo que el acta enviada después no tiene.
- **Lo que deliberadamente no hace:**
  - No resume la conversación.
  - No incluye pizarra, votación ni señalar sobre el contenido (eso es A2).
  - No captura lo decidido en WhatsApp o Slack.
  - No reemplaza Jira ni el sistema donde se ejecuta: publica ahí.
  - No cubre reuniones con externos en la primera versión.
  - No publica nada sin la confirmación del conductor.

## Creencias

Las de la oportunidad, referenciadas tal como están registradas en `product/overview.md`:

- [opportunity: colaboracion-fuera-de-teams] [value] En cuentas Premium grandes de tecnología distribuida, quien convoca saca el trabajo en vivo fuera de Teams porque decidir en el momento y dejar registro que encuentre quien no estuvo le cuesta más ahí que en el canal paralelo. (#2, `weakened`)
- [opportunity: colaboracion-fuera-de-teams] [viability] IT de esas cuentas sube a Max cuando puede demostrar ante finanzas que la coordinación volvió adentro y que baja el shadow IT. (#3)

Propuestas para el registro (pendientes de aprobación):

- [feature: cierre-de-decisiones] [value] En reuniones de trabajo donde hubo decisiones, el conductor confirma la tarjeta antes de cortar la llamada. Se cae si en un piloto más de la mitad de las tarjetas se publica sin confirmar o se reescribe por completo.
- [feature: cierre-de-decisiones] [value] Con la tarjeta confirmada y publicada donde se ejecuta, bajan las decisiones ejecutadas distinto de lo decidido. Se cae si, a dos semanas, la tasa de decisiones mal ejecutadas no baja frente a la línea de base del mismo equipo.
- [feature: cierre-de-decisiones] [feasibility] El borrador separa decisión de idea y asigna responsable con precisión suficiente para que el conductor confíe en él. Se cae si, en reuniones grabadas del piloto, más de 1 de cada 5 decisiones propuestas era una idea o no tenía responsable. (Lo juzga tech.)
- [feature: cierre-de-decisiones] [viability] IT de cuentas del segmento considera el cierre confirmado una razón para el tier que lo incluye. Se cae si en las entrevistas con IT el cierre no aparece entre las razones de compra, o si "Max" no incluye la capa de IA.

## Descartadas o en pausa

- **A2 `interaccion-en-vivo`, en pausa.** La participación es un dolor real, pero secundario al cierre, y Miro ya cubre votar y agrupar. Vuelve si el piloto de A1 muestra que las objeciones de quienes no hablaron siguen apareciendo después de confirmar la tarjeta. En ese caso, recoger la posición de quien no habló podría sumarse a A1.
- **A3 `continuidad-de-artefactos`, en pausa.** Es condición de entrada para lo nativo, no una razón para elegirlo. Vuelve como requisito si la tarjeta de A1 tiene que vivir en la serie, o como primera opción para el subsegmento con compliance (España/UE).
- **A4 `ritual-de-cierre`, en pausa.** Es la alternativa que A1 tiene que superar. Vuelve si tech dice que A1 no es factible antes de CollabCon, o como grupo de control en el piloto de A1.
- **A5 `panel-it-coordinacion`, descartada.** No alivia el dolor del usuario, y su creencia de viabilidad es la misma que tiene evidencia `secondary` en contra.
- **A6 `externos-un-click`, descartada antes de evaluar, por decisión de Damián.** Los externos son el 4% de las quejas y aparecen en 1 de 10 entrevistas. Además, es el dolor de la persona negativa (Sofía Paz).
