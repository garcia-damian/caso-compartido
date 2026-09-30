---
date: 2026-09-30
source: survey
survey: product/surveys/2026-09-23-1944-colaboracion-en-vivo-fuera-de-teams.md
results: product/surveys/2026-09-26-1800-respuestas-colaboracion-en-vivo-fuera-de-teams.csv
n: 210 completas (email 76 · panel 134); 182 trabajaron fuera de Teams, 28 "En ninguna"
opportunity: colaboracion-fuera-de-teams
---

# Análisis de encuesta: colaboración en vivo fuera de Teams

## Denominador y límites

- **Entradas:** 249 → 210 completas, 34 descalificadas, 5 parciales. Respuestas entre el 23/09 y el 25/09.
- **Por canal:** email 76 completas (alcance `unknown` → sin tasa de respuesta; se esperaban ≥150 de este canal). Panel 134 completas sobre cuota de 150.
- **Metas de n:** trabajaron afuera 182 (meta ≥150 ✓) · "En ninguna" 28 (meta ≥30 ✗ → **direccional**; el ajuste de cuota previsto para la revisión del 25/09 no se hizo) · ≥30 por canal ✓.
- **Calidad:** sin speeders (completa más corta: 75 s). 4 straightliners en la matriz Q10, todos del panel. Firmografía del panel autodeclarada (no verifica plan ni facturación).
- **Diferencias entre canales**, en la dirección que anticipaba el diseño (email sobrerrepresenta a los conformes con Teams):

| Indicador | Email | Panel |
|---|---|---|
| Trabajan afuera en más de la mitad o todas las reuniones | 21% | 40% |
| Hubo externos en la reunión | 17% | 24% |
| El artefacto ya existía | 43% | 59% |
| La decisión quedó registrada en Teams (chat, notas o recap) | 35% | 20% |
| La decisión quedó en un chat fuera de Teams | 18% | 26% |
| No sabía que existía el resumen de IA | 5% | 16% |

Ningún total representa al segmento: donde los canales difieren, se reporta el corte. Todo lo que sigue es lo **qué**; los **por qué** quedan para entrevistas.

Salvo O4, la base es n=182 (quienes trabajaron en una herramienta externa).

## O1. Origen del artefacto

- **Creíamos:** el tablero o documento se crea para la reunión (colaboración en vivo).
- **Muestra:** ya existía en el **54%** (51% siguió usándose, 3% no). Se creó para la reunión en el 39% (24% siguió, 15% no). 7% no sabe. El 75% siguió usándose después.
- **Es bimodal según la herramienta:**
  - **Sin pizarra (66%)** — Google Docs/Sheets/Slides 32%, Jira 29%, dashboards 16%, Confluence 14%, Notion 12%: el **74% ya existía**.
  - **Con pizarra (34%)** — Miro 20%, FigJam 12%, Mural 9%, Lucidspark 4%: entre el 7% y el 19% ya existía.
- **Decisión:** para la mayoría el problema es de **integración con los sistemas donde ya vive el trabajo**, no de colaboración en vivo. La pizarra de reunión es un caso minoritario (un tercio).

## O2. Costo de acceso

- **Creíamos:** entrar cuesta ~5 minutos; la hipótesis rival dice que la fricción se concentra en reuniones con externos.
- **Muestra:**
  - Tardó **5 minutos o más** en el 27% (sin externos: 18%). Menos de 2 minutos: 46%.
  - En el **50%** de las reuniones al menos un participante no entró y siguió mirando otra pantalla (27% uno, 18% dos o tres, 5% cuatro o más).
  - **Externos** en el 21% de las reuniones. Con externos, 62% tardó ≥5 min, contra 18% sin externos. Pero la mitad de las reuniones lentas (24 de 50) y dos tercios de las que dejaron a alguien afuera (63 de 92) **no tenían externos**.
  - **Artefacto creado para la reunión:** 39%–48% tardó ≥5 min, contra 13% si ya existía (permisos, enlaces nuevos).
  - **Cómo llegaron:** enlace en el chat 54%, ya la tenían abierta 22%, pantalla compartida y cada uno por su cuenta 15%, app dentro de Teams 8%. La telemetría (que ve solo enlaces pegados en el chat) **ve cerca de la mitad** de los casos.
  - App dentro de Teams: dejó a alguien afuera en 13 de 15 casos (n muy chico, direccional).
- **Decisión:** el umbral de 5 minutos **no describe la reunión interna típica**. El costo masivo es otro: alguien queda afuera en la mitad de las reuniones. Los externos son una fricción fuerte pero minoritaria: no alcanzan para cambiarle el segmento a la oportunidad.

## O3. Qué se hace afuera y dónde queda la decisión

- **Creíamos:** la actividad es de pizarra (ideas, agrupar) y la decisión se pierde.
- **Actividades (Q5, respuesta múltiple):** votar o priorizar 40% · editar un documento entre varios 35% · revisar datos o métricas 34% · anotar decisiones 33% · aportar ideas 29% · actualizar tareas 25% · agrupar ideas 22% · diagramar 13%. "Otro" 5% (lista completa).
- **Registro (Q9, respuesta múltiple):** no quedó en ningún lado 24% · chat fuera de Teams 23% · Jira 23% · la misma herramienta externa 15% · recap/transcripción/resumen de IA 14% · chat o notas de la reunión de Teams 13% · acta 12% · correo 10% · no hubo decisiones 7%.
  - **31%** sin registro recuperable (nada, o solo un chat fuera de Teams). **25%** quedó en Teams (chat, notas o recap).
  - **"Otro" = 18%**, por encima del límite de 15% del diseño: **a la lista le falta la opción "recap, transcripción o resumen de IA"**. Casi todas esas menciones vienen con una queja: *"En el recap de Copilot, que resume todo pero no distingue lo decidido de lo conversado"*, *"En el resumen de IA, que nadie leyó"*, *"En el recap automático, pero después lo tuve que corregir"*.
- **Lo más difícil (Q11, abierta, 95 respuestas; una respuesta puede tener más de un código):**

| Tema | Menciones | % | Cita |
|---|---|---|---|
| Registro y continuidad (suma de los tres siguientes) | 33 | 35% | |
| · Lo decidido se pierde, no se encuentra, no se retoma | 22 | 23% | *"Cada reunión es una isla. Lo que se trabajó en la anterior está en otro lado."* · *"Muchas veces creemos que decidimos y en realidad cada uno entendió algo distinto."* |
| · Trabajo manual del conductor (acta, pasar a Jira, dueños y fechas) | 8 | 8% | *"Termino escribiendo el acta yo después de cada reunión y pasando las tareas a Jira a mano. Es trabajo que nadie ve."* |
| · El resumen de IA no separa lo decidido de lo conversado | 3 | 3% | *"El resumen automático sirve para saber de qué se habló pero no para saber qué quedó decidido."* |
| Participación y facilitación | 13 | 14% | *"Hay 12 personas y opinan 3."* |
| Limitaciones de lo nativo | 13 | 14% | *"Probamos la whiteboard de Teams… no tenía plantillas ni votación y a la retro siguiente no la encontramos. Desde ahí todo en Miro."* |
| Converger y decidir en el momento | 12 | 13% | *"Divergir es fácil… Ordenarlas y elegir es lo que nos cuesta."* |
| Acceso interno (permisos, SSO, enlace en el chat, licencias por filial) | 7 | 7% | *"Los permisos del Miro. Siempre hay alguien que no puede editar y pierde los primeros 10 minutos."* |
| Husos horarios, países e idioma | 4 | 4% | |
| Acceso de externos | 4 | 4% | *"Cuando vienen externos es un desastre."* |
| Compliance o seguridad limita las herramientas externas | 3 | 3% | *"Compliance no nos deja meter datos de clientes en Miro, así que o lo hacemos en Teams o no se hace."* |
| Otros (demasiadas reuniones, problemas técnicos, sin problema, no aplica) | 10 | 11% | |

- **Decisión:** cualquier solución tiene que cubrir la **continuidad entre reuniones** y **separar lo decidido (con dueño y fecha) de lo conversado**, además de votar o priorizar. Una pizarra sola no cubre la actividad dominante.

## O4. Conocimiento y uso de lo nativo (n=210)

| Función | No sabía | Sabe, nunca la usó | La usó y dejó | La usa (algunas + mayoría) | Lectura |
|---|---|---|---|---|---|
| Whiteboard | 8% | 27% | **43%** | 21% | "No me sirve" |
| Notas de la reunión (Loop) | **31%** | 28% | 14% | 27% | "No sé que existe" |
| Apps de terceros en la reunión | **40%** | 28% | 9% | 23% | "No sé que existe" |
| Resumen o asistente de IA | 12% | **39%** | 13% | 36% | Lo conocen y no lo usan: ¿por qué? |

- Whiteboard tiene el abandono más alto. Las razones aparecen en Q11: no tiene votación ni plantillas, a la semana no se encuentra, se traba con más de 8 personas, está escondida en un menú.
- IA: "sabe y nunca la usó" llega al 47% en email (34% en panel).
- El grupo "En ninguna" (n=28, direccional) contesta parecido a los demás. En Q12 (16 respuestas) lo resuelven hablando mientras alguien anota en el chat, OneNote o un Excel compartido (6), votando a mano alzada, con reacciones o con Forms (4), con la pizarra o las notas de Teams (4) o decidiendo fuera de la reunión (3). En 2 casos, compliance prohíbe las herramientas externas.
- **Decisión:** separa dos problemas distintos. Whiteboard es "no me sirve" (hay que resolver funciones y persistencia). Notas y apps son "no sé que existe" (descubrimiento).

## Insights (por impacto)

1. **El dolor principal es la continuidad y el registro, no el acceso.** Es el 35% de las respuestas abiertas, contra 4% de externos; 31% queda sin registro recuperable; el conductor hace el acta a mano. → Priorizar capacidades que dejen la decisión encontrable y conectada con la reunión siguiente.
2. **Lo que sale de Teams es sobre todo trabajo que ya vive afuera.** El 74% de los artefactos sin pizarra ya existía (Jira, Docs, dashboards). → Evaluar integración con esos sistemas antes que una pizarra propia.
3. **El resumen de IA existe y no alcanza.** El 14% lo nombró sin que se lo ofrecieran, casi siempre para quejarse de que no separa lo decidido. El 39% lo conoce y nunca lo usó. → Candidato fuerte: decisiones con dueño y fecha extraídas del recap.
4. **Whiteboard fue abandonada por razones concretas** (43% la probó y dejó): votación, plantillas, persistencia entre reuniones.
5. **Alguien queda afuera en la mitad de las reuniones**, con o sin externos, y más cuando el artefacto es nuevo.
6. **Compliance en España/UE:** 4 de las 5 menciones de compliance vienen de España. Ahí lo nativo es la única opción: un subsegmento donde una mejora nativa no compite con Miro.

## Por qué abiertos (para entrevistas)

- ¿Por qué quienes conocen el resumen de IA no lo usan: licencia, confianza, calidad?
- ¿Por qué la decisión termina en un chat fuera de Teams y no en el chat de la reunión?
- ¿Por qué se crea una pizarra por reunión en lugar de continuar la anterior?
- ¿Por qué la app abierta dentro de Teams deja gente afuera (13 de 15)?
- ¿Qué hace el conductor con el recap después de la reunión, y cuánto tiempo le lleva?

## Limitaciones del instrumento

- Q9 necesita la opción "recap, transcripción o resumen de IA" si la encuesta se repite.
- La encuesta mide qué pasó en la última reunión, no por qué el trabajo salió de Teams: no distingue por sí sola entre las explicaciones rivales de la creencia #2.
- Respuestas abiertas casi idénticas entre respondentes distintos: R-046/R-170 (Q12), R-207/R-224 y R-077/R-196 (Q11). No invalidan el análisis, pero conviene revisarlas.

## Pool de reclutamiento

77 aceptaron una conversación; **64 son candidatos** (no son IT y conducen 2+ reuniones de más de 5 por semana): 48 del panel y 16 del email. **47 contradicen al menos una señal de la creencia.** Los contactos están en la columna R4 del CSV; acá solo van los IDs.

**Contradicen dos señales (Q4 ya existía + Q6 < 2 min) — entrevistar primero (17):**
R-036 (email, Perú) · R-057 (panel, México) · R-094 (panel, EE. UU.) · R-102 (panel, Colombia) · R-128 (panel, Argentina) · R-131 (email, España) · R-144 (panel, Chile) · R-151 (panel, México) · R-176 (panel, Argentina) · R-180 (email, Argentina) · R-194 (panel, Chile, sin contacto) · R-224 (panel, Chile) · R-229 (panel, Colombia) · R-234 (panel, Chile) · R-235 (panel, Colombia) · R-240 (panel, EE. UU.) · R-247 (panel, México)

**Q1 "En ninguna" (12):**
R-009 (email, Colombia, compliance) · R-046 (email, Argentina) · R-085 (panel, Colombia) · R-088 (panel, Argentina) · R-110 (panel, España, sin contacto) · R-120 (panel, Colombia) · R-135 (email, Brasil) · R-143 (email, España, compliance) · R-153 (email, Argentina) · R-170 (panel, Colombia — **verificar**: el contacto coincide con el nombre de una persona sintética del repo y la respuesta de Q12 es casi idéntica a la de R-046) · R-196 (panel, México) · R-242 (panel, México)

**Q4 ya existía (11):** R-042 · R-065 · R-086 · R-132 (sin contacto) · R-159 · R-171 · R-201 · R-227 (sin contacto) · R-228 · R-238 · R-244

**Q6 < 2 min (7):** R-013 · R-074 · R-089 · R-090 · R-093 · R-173 · R-230

**Confirman (17):** R-006 · R-011 · R-019 · R-024 · R-031 · R-038 · R-070 · R-076 · R-077 · R-097 · R-099 · R-101 · R-103 · R-113 · R-204 · R-205 · R-245
