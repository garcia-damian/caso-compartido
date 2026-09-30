---
date: 2026-09-30
source: real
opportunity: colaboracion-fuera-de-teams
guide: product/interview-guides/2026-09-23-2030-colaboracion-en-vivo-fuera-de-teams.md
cross-reference: product/insights/2026-09-30-1621-colaboracion-en-vivo-fuera-de-teams.md (encuesta, n=210)
sources:
  - product/interviews/interviews/2026-09-25-1000-tomas-aguirre.md (real · R-113)
  - product/interviews/interviews/2026-09-25-1100-andres-quintero.md (real · R-170, ver "Calidad de la evidencia")
  - product/interviews/interviews/2026-09-25-1600-lucia-fernandez.md (real · R-143)
  - product/interviews/interviews/2026-09-28-0900-javier-molina.md (real · R-097)
  - product/interviews/interviews/2026-09-28-0930-martina-rojas.md (real · R-224)
  - product/interviews/interviews/2026-09-28-1000-diego-paredes.md (real · R-036)
  - product/interviews/interviews/2026-09-28-1200-sofia-martinez.md (real · R-151)
  - product/interviews/interviews/2026-09-28-1400-paula-benitez.md (real · R-153, ver "Calidad de la evidencia")
  - product/interviews/interviews/2026-09-28-1500-valeria-castro.md (real · R-024)
  - product/interviews/interviews/2026-09-28-1700-ricardo-salinas.md (real · R-196)
---

# Insights: entrevistas sobre colaboración en vivo en reuniones grandes

Diez líderes que conducen reuniones de más de cinco personas en SaaS B2B de 650 a 2.000 empleados, con equipos en 3 o 4 países. Cinco de ellos trabajan afuera de Teams (Miro, FigJam, Slido, Jira, Confluence, Power BI) y cinco respondieron "En ninguna" o casi. La encuesta ya había mostrado **qué** pasa; estas entrevistas explican **por qué**. Los insights van ordenados por impacto. Entre corchetes, cuántos entrevistados lo mencionan, y si la encuesta lo respalda.

## 1. Lo que falla es el cierre: la decisión no llega intacta a quien la ejecuta, se trabaje donde se trabaje [10/10 · encuesta: 35% de las abiertas, 31% sin registro recuperable]

Los diez contaron un caso concreto en el que lo decidido se ejecutó mal o no se ejecutó. En todos, la falla estuvo entre el final de la reunión y la ejecución: un responsable ambiguo, una decisión enterrada o un registro que llegó tarde. Pasa igual en Teams, Miro, FigJam, Jira y Confluence, así que el problema no depende de dónde se trabaje. El costo es alto: 1 a 2 semanas de trabajo perdido, clientes esperando días y releases corridas. Hoy lo cubre el conductor a mano, con 10 a 60 minutos por reunión, y tres dicen textualmente que "nadie más lo hace". Esto implica cerrar la reunión con **decisión, responsable, fecha y el porqué**, que todos lo vean antes de cortar la llamada y que se publique donde se ejecuta (Jira, el canal o el correo).

> Evidencia: "Yo pensé que el arquitecto iba a hacer el ADR y él pensó que yo lo iba a mandar por correo" (2 días de arreglo y un fin de semana de guardia) — Ricardo · "el líder de Ecuador entendió que lo pasaba yo, y yo entendí que lo pasaba él. Nadie lo pasó" (el cliente esperó 4 días) — Andrés · SPEI descartado en un hilo de comentarios que, al marcarse como resuelto, quedó oculto: "Dos semanas de trabajo que hubo que sacar" — Sofía · "El qué queda en Jira. El problema es el por qué" (la historia de seguridad quedó postergada más de lo necesario) — Martina · otros casos: Javier (API 2 semanas tarde, release movida), Diego (campaña 3 días de más), Valeria (1 semana de un diseñador), Paula (1 semana de 2 devs), Lucía (1 semana sin dueño), Tomás (acuerdo rediscutido).

## 2. El recap de IA se conoce y se abandona porque resume la conversación, no las decisiones, y a veces inventa decisiones [6/10 · encuesta: 39% lo conoce y nunca lo usó, y el recap aparece espontáneamente en "Otro" con quejas]

Esto responde el "por qué" que dejó abierto la encuesta. El recap no se usa porque no se puede confiar en él para lo que importa, no por falta de licencia. Pone todo al mismo nivel, no dice quién se comprometió a qué, confunde ideas con decisiones y no ve lo que pasó fuera del audio: los votos en Miro o FigJam, el filtro del dashboard, el hilo de Slack. Dos errores del recap terminaron en trabajo perdido, y quien lo usa igual lo reescribe (Javier 30 min, Paula más de 10 min). Implica un recap que estructure decisión, responsable y fecha, marque lo dudoso ("¿idea o decisión?"), lo haga confirmar al conductor antes de publicarse y tome contexto del artefacto que se trabajó en pantalla.

> Evidencia: "En el recap quedó como 'se habló de la API de geocercas'. El equipo de México leyó el recap… Entregaron dos semanas tarde" — Javier · "marca como decisión cosas que eran solo ideas… Perdimos más o menos una semana de dos desarrolladores" — Paula · "Me resumió la conversación, no las decisiones… La primera vez lo pegué en el ticket. Nadie lo leyó" — Martina · "no me dice quién se comprometió a qué" — Lucía · "no sabe qué número estábamos mirando" — Diego · "decía algo como 'se discutieron prioridades'. Pues sí, gracias" — Valeria

## 3. La pizarra se abandona porque se pierde: queda atada a una reunión y desaparece al reprogramar; la continuidad es lo que retiene a Miro [6/10 · encuesta: 43% la probó y la dejó]

Seis probaron la pizarra de Teams y ninguno siguió usándola por gusto. Lucía la usa porque compliance no le deja otra opción. En vivo le falta votar, tener plantillas y agrupar, y con 9 a 14 personas se traba. La razón que la saca definitivamente es otra: la pizarra, y también las notas, cuelgan del chat de esa reunión. Cuando la serie se recrea o se reprograma, desaparecen, y cuatro perdieron así los acuerdos. Quienes se quedan en Miro lo hacen justamente por continuidad: un tablero por trimestre y un frame por sesión, para revisar lo acordado la vez anterior. Implica anclar los artefactos a la serie, el equipo o el canal, con historial entre sesiones. Votar y agrupar son condición de entrada. Pesa más en cuentas con compliance, donde lo nativo es lo único disponible.

> Evidencia: "Quedó colgada del chat de esa reunión… Perdí los acuerdos, así de simple. Ahí dije: listo, volvemos a Miro" y "Esa continuidad es la razón por la que estamos en Miro" — Tomás · "queda atada al chat de esa reunión… No la encontré" y "lo nativo es lo único que tengo. Necesito que funcione mejor" — Lucía · "la quise volver a buscar para el seguimiento y no supe dónde había quedado" — Sofía · "se creó otra invitación y las notas quedaron en la otra" — Paula · "No tenía forma de votar… A los veinte minutos volvimos a Miro" — Javier · "no encontré cómo agruparlas. Perdimos quince minutos" — Ricardo

## 4. El conductor es el único que toca el contenido: los demás dictan, señalan con palabras y votan a mano alzada, y quien no habla objeta después [8/10 · encuesta: alguien queda afuera en el 50% de las reuniones; "Hay 12 personas y opinan 3"]

Aunque todos vean lo mismo, todo pasa por el conductor. Le dictan lo que quieren poner (5 casos), intentan señalar sobre la pantalla compartida con palabras ("la de abajo, no, la otra") (4) y votan con la manito o con reacciones que él cuenta sin confiar en el número (3). Eso alarga la reunión y produce errores caros: Andrés cerró el ticket equivocado y al cliente le llegó la notificación. En seis reuniones hubo gente que no opinó (nuevos, juniors, otro huso horario o sin acceso) y su objeción apareció días después, con la decisión ya tomada. En los empates decide el líder (6/10). Implica que cualquiera pueda señalar, marcar y votar sobre el contenido compartido (una fila, un gráfico o un ticket), con votos limitados y contados solos, y una forma de recoger la posición de quien no habló antes de cerrar.

> Evidencia: "Me dijeron 'ese ciérralo', yo lo marqué cerrado, y era el de la fila de al lado. Al cliente le llegó la notificación de cierre" — Andrés · Gloria "nunca logró entrar… No dijo casi nada" y a la semana objetó la decisión principal; "en casi todas hay alguien mirando desde afuera, y esa gente no opina. Eso me preocupa más que los minutos" — Valeria · "Me dicta, literalmente" — Tomás · "el pico de marzo… no, el otro" — Diego · "no te fías del todo del número" — Lucía · "dos devs se quedaron con cara de no" — Martina

## 5. El trabajo en vivo se hace donde ya vive el artefacto; se sale a Miro o FigJam por capacidad o costumbre, y eso cuesta de 5 a 10 minutos de acceso y el cambio constante de ventana [7/10 · encuesta: el 74% de los artefactos sin pizarra ya existía; los externos son el 4% de las quejas]

Cuando el artefacto es el sistema de registro (Jira, Confluence, Power BI o un Excel en SharePoint), nadie lo saca de ahí y con SSO se entra al instante. Se sale a Miro, FigJam o Slido para ejercicios con estructura (retro, planning, priorización), por capacidad (votar, plantillas, continuidad) o por costumbre ("lo trajo mi antecesor", "siempre se hace ahí"). En esos casos, cada sesión pierde de 5 a 10 minutos en licencias de invitado, en otra instancia de Miro por filial o en gente logueada con su cuenta personal de Google. Además, durante toda la reunión se pierde el hilo al saltar entre ventanas. Los externos aparecieron una sola vez (una agencia, una vez al mes). Implica llevar la capa de interacción (señalar, votar, decidir, registrar) a la llamada sobre esos artefactos en lugar de reemplazarlos, y resolver de forma nativa los ejercicios estructurados.

> Evidencia: "la filial de Francia tiene otra instancia de Miro… Diez minutos largos, más" y "perder el hilo cada vez que cambias de herramienta es durante las dos horas" — Javier · "Entramos todos con SSO… Cero fricción" y "Si hacemos el planning en otro lado después hay que pasarlo a Jira igual" — Martina · "Varios entran con la cuenta personal de Google… Seis, ocho minutos así" — Valeria · "entre cinco y siete minutos se van en eso" — Tomás

## Recurrencia y contrapuntos

- **Más fuerte:** los insights 1 y 2 aparecen en entrevistados que trabajan dentro y fuera de Teams, y coinciden con el tema principal de la encuesta. El problema no es de un solo tipo de usuario.
- **No toda reunión grande es para decidir.** Paula y Ricardo deciden a propósito entre 3 o 4 personas: la reunión grande es para informar ("dar la sensación de que todos participaron" no es decidir). Aun así, Ricardo sufrió el insight 1 en una sync de 16. Conviene segmentar por tipo de reunión (informativa o de trabajo), no solo por rol.
- **"A mí no me falta nada en Teams"** (Diego, Ricardo, Paula, Martina): atribuyen el problema a disciplina o al exceso de reuniones (Ricardo tiene 27 h por semana). Tienen el dolor del insight 1, pero lo leen como falla de proceso.
- **Descubrimiento:** Andrés, Valeria y Ricardo no sabían que había notas, pizarra o apps dentro de la reunión. Diego conoce Loop solo por un correo de IT. Coincide con el "no sé que existe" de la encuesta.

## Preguntas de la encuesta que las entrevistas responden

| Pregunta abierta | Respuesta en entrevistas |
|---|---|
| ¿Por qué no usan el resumen de IA quienes lo conocen? | Calidad y confianza: no separa lo decidido, inventa decisiones y no ve el artefacto (insight 2). Ninguno mencionó la licencia. |
| ¿Por qué la decisión termina en un chat fuera de Teams? | Solo 2 casos (Javier y Martina): alguien abre un hilo de Slack durante la reunión para consultar a quien no está. Sigue abierta. |
| ¿Por qué una pizarra por reunión en lugar de continuar la anterior? | Parcial: la de Teams no se puede continuar porque se pierde (insight 3). En Miro o FigJam depende de la costumbre del conductor (Tomás y Javier continúan; Valeria y Martina duplican). |
| ¿Por qué la app dentro de Teams deja gente afuera? | Sin evidencia. Nadie usó apps dentro de la reunión. |
| ¿Qué hace el conductor con el recap y cuánto le lleva? | Lo corrige o lo reescribe (Paula más de 10 min, Javier 30 min) o lo abandona (Martina). |

## Calidad de la evidencia

- **Andrés Quintero (R-170):** tiene el mismo nombre que una persona sintética del repo (`product/personas/andres-quintero.md`), en la misma industria (SaaS de facturación electrónica) y el mismo país. La encuesta ya había marcado su respuesta Q12 como casi idéntica a la de R-046. El contenido de la entrevista es distinto al de la persona (otro rol, otro dolor), pero conviene verificar la identidad antes de citarlo como evidencia real. Sin él, el insight 4 queda en 7/10 y pierde el ejemplo del ticket cerrado por error.
- **Paula Benítez:** la entrevista es del 28/09, pero describe "el review de octubre" y unas notas "del lunes 13" como ya ocurridos. Probablemente sea un error de transcripción. Revisar las fechas.
- **Autodeclaración en la encuesta:** Tomás (R-113) admitió que respondió "salgo de Teams en todas" y no es así. El resto de los cruces entre encuesta y entrevista coincide.
- La muestra es solo de conductores: no hay participantes ni IT.
