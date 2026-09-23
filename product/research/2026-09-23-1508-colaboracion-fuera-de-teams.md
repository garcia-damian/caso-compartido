---
source: secondary
method: web
date: 2026-09-23
question: ¿Cómo compiten Zoom, Meet y Slack en colaboración en vivo y qué cobran? ¿Qué evidencia pública hay de por qué la coordinación sale de Teams (fricción vs. hábito vs. externos)? ¿Qué hace subir de tier a IT (uso vs. precio/bundle/negociación)? ¿Dónde está saturado y dónde vacío el espacio de notas y decisiones con IA?
opportunity: colaboracion-fuera-de-teams
---

# Research: colaboración en vivo fuera de Teams

Método: búsqueda web con 4 agentes en paralelo, uno por pregunta. Cada dato lleva `[verificado: URL — fecha]` o `[conocimiento del modelo — verificar]`. Todo es evidencia sobre el **mercado**: no verifica nada sobre los usuarios del segmento.

**Los tres hallazgos que cambian decisiones:**

1. **La desventaja de Teams en colaboración en vivo es de empaquetado, no de capacidad.** Con Business Premium ($22) el equipo tiene notas colaborativas, pero el recap para ausentes exige Teams Premium (+$10) y el Facilitator (notas en vivo, decisiones, acciones) exige Copilot. Zoom Pro (~$14), Google Workspace Standard ($14) y Slack Pro ($7,25) incluyen notas, resumen para ausentes y acciones en el plan de entrada. Además, el Facilitator **no funciona en reuniones con externos**: la fricción (hipótesis A) y el acceso de externos (hipótesis C) se tocan justo ahí.
2. **La creencia de viabilidad tiene más evidencia en contra que a favor.** En enterprise, el paso de tier se decide por descuento, bundle y seguridad/cumplimiento. El ROI de uso de Copilot "sigue siendo esquivo" para IT. Microsoft declara que su upsell lo mueven Copilot, E5 y E7 (seguridad + IA), no la coordinación. Y el shadow IT que hoy preocupa es IA no aprobada, no chat.
3. **El resumen posterior a la reunión es un commodity. Decidir en la reunión y dejar un registro que encuentre quien no estuvo, no.** Al menos 10 de 13 productos venden transcripción, resumen y acciones, con plan gratis o de $8–20. Casi nadie cubre la decisión en vivo, un registro de decisiones consultable entre reuniones, traer al registro lo decidido en WhatsApp/Slack, ni analítica para IT sobre dónde se coordina la gente.

Alerta de encuadre: **todos los planes Business de Microsoft tienen tope de 300 usuarios** `[verificado: https://www.microsoft.com/en-us/microsoft-365/business/compare-all-microsoft-365-business-products — 2026-09-23]`. El segmento (Business Premium, 100+ licencias, promedio ~170 por cuenta) cabe, pero en el mundo real el "Max" de una cuenta Business Premium es Business Premium + Copilot ($32) o saltar a E3/E5/E7. Conviene confirmar con el caso qué es "Max".

---

## 1. Competidores directos: colaboración en vivo en la reunión

Precios en USD por usuario/mes, pago anual, consultados el 2026-09-23.

| Oferta | Para quién | Colaboración en vivo (qué plan la incluye) | Precio | Fortalezas / debilidades |
|---|---|---|---|---|
| **Microsoft Teams** (M365 Business Premium) | Empresas con M365, máx. 300 usuarios `[verificado: https://www.microsoft.com/en-us/microsoft-365/business/microsoft-365-business-premium — 2026-09-23]` | Base: notas colaborativas con Loop (agenda, notas, tareas) `[verificado: https://techcommunity.microsoft.com/blog/microsoft_365blog/how-microsoft-teams--microsoft-loop-can-make-your-meetings-better/4092390 — 2026-09-23]`; Whiteboard y encuestas con Forms `[conocimiento del modelo — verificar]`. **Teams Premium:** intelligent recap, notas con IA `[verificado: https://www.microsoft.com/en-us/microsoft-teams/premium — 2026-09-23]`. **Copilot:** Facilitator `[verificado: https://learn.microsoft.com/en-us/microsoftteams/facilitator-teams — 2026-09-23]` | Business Premium $22; + Teams Premium $10; Business Premium with Copilot $32 `[verificado: páginas de Microsoft citadas — 2026-09-23]` | + Todo queda en el tenant. − Lo "en vivo" está repartido en 3 licencias. − Facilitator no funciona con externos |
| **Zoom Workplace** | Empresas centradas en la videollamada, multiplataforma | Pro: AI Companion sin límite (resúmenes, notas, Docs), encuestas. Business: Whiteboard sin límite `[verificado: https://zoom.us/pricing — 2026-09-23]` | Pro $14,16; Business $18,33; Enterprise a cotizar | + IA incluida sin costo extra. + Toma notas también en reuniones de Teams y Meet `[verificado: https://news.zoom.com/zoomtopia2025/ — 2026-09-23]`. − Duplica la suite de M365 |
| **Google Workspace / Meet** | Empresas nativas de Google | Business Standard+: encuestas, Q&A, transcripción, Gemini `[verificado: https://knowledge.workspace.google.com/admin/meet/compare-meet-features-across-google-workspace-editions — 2026-09-23]`. "Take notes for me": Doc con acciones, decisiones y un "Summary so far" para quien llega tarde `[verificado: https://support.google.com/meet/answer/14754931 — 2026-09-23]` | Starter $7; Standard $14; Plus $22 `[verificado: fuente secundaria emailtooltester.com — 2026-09-23]` | + Buena relación precio/IA. − Sin pizarra propia desde el cierre de Jamboard (31/12/2024) `[verificado: https://workspaceupdates.googleblog.com/2023/09/the-next-phase-of-digital-whiteboarding-for-google-workspace.html — 2026-09-23]`. − Un idioma por reunión |
| **Slack** | Equipos técnicos con cultura de chat asíncrono | Pro+: huddles, canvas, lists y notas de IA del huddle (decisiones, acciones) guardadas en el hilo `[verificado: https://slack.com/pricing y https://slack.com/help/articles/31377193680019 — 2026-09-23]`. No funcionan con invitados externos | Pro $7,25; Business+ $15 | + El registro queda donde el equipo ya conversa. − Huddles informales, no reemplazan una reunión estructurada |

**Qué prueba y qué no:** que todos incluyan notas y resumen para ausentes prueba que hay demanda de dejar registro. **No prueba** que los Team Leads del segmento salgan de Teams por eso: puede pesar más el hábito, los externos o que el otro canal sea gratis.

**Cambios 2025–2026:**

- Slack reorganizó sus planes en 2025: la IA de huddles pasó a todos los planes de pago `[verificado: https://slack.com/help/articles/39264531104275 — 2026-09-23]`.
- Zoom AI Companion 3.0 (nov./dic. 2025), incluido en planes de pago; versión suelta ~$10 según prensa `[verificado: reworked.co — 2026-09-23; sin confirmar en la página de Zoom]`.
- Google subió 17–22% al incluir Gemini (2025) `[fuente secundaria — verificar]`.
- Microsoft subió Business Basic/Standard, E3 y E5 desde el 1/07/2026 y lanzó Business Premium with Copilot ese mismo día `[verificado: https://www.microsoft.com/en-us/licensing/news/2026-m365-packaging-pricing-updates-faq — 2026-09-23]`.
- El Facilitator deja de generar archivos Loop el 31/07/2026 y pasa a Word `[verificado: Microsoft Learn, arriba]`: Microsoft está cambiando dónde vive el registro de la reunión.

## 2. Alternativas y no consumo: por qué migra la coordinación

**No hay ninguna fuente que mida nuestro caso** (quien convoca, en tecnológicas distribuidas, sacando la coordinación en vivo de Teams) **ni que ponga a competir las tres explicaciones.** Lo que hay es de otros segmentos.

**Prevalencia de canales paralelos:**

- México, trabajadores de primera línea: 76% coordina por WhatsApp, 80% se niega a instalar apps de la empresa en su teléfono (Ozaru/Púrpura AI, jun. 2026, muestra no publicada) `[verificado: https://www.xataka.com.mx/empresas-y-economia/whatsapp-oficina-millones-mexicanos-mayoria-trabajadores-usa-para-coordinar-su-trabajo — 2026-09-23]`. Segmento distinto al nuestro.
- Reino Unido, 1.261 trabajadores (2020): 41% usa WhatsApp para trabajar `[verificado: https://guild.co/blog/study-whatsapp-professional-use/ — 2026-09-23]`.
- SEC: más de 100 entidades y más de USD 3.000 M en multas por canales no autorizados desde 2021; CFTC, más de USD 1.000 M `[verificado: https://www.hklaw.com/en/insights/publications/2024/12/a-long-winters-nap-sec-off-channel-communications y https://www.cftc.gov/PressRoom/SpeechesTestimony/romerostatement080823 — 2026-09-23]`. Sector financiero, no tecnológico: muestra que el canal paralelo persiste aun con prohibición y multas.
- Porcentaje de empresas donde coexisten Teams y Zoom: **desconocido** (solo agregadores SEO sin fuente primaria).

**(A) Fricción: decidir y dejar registro cuesta más en Teams**

- Microsoft Work Trend Index 2025 (telemetría + 31.000 trabajadores): 57% de las reuniones son llamadas improvisadas sin invitación; 30% cruza husos horarios `[verificado: https://www.microsoft.com/en-us/worklab/work-trend-index/breaking-down-infinite-workday — 2026-09-23]`. Mucha coordinación ocurre sin estructura que deje registro, incluso dentro de Teams.
- Atlassian State of Teams 2025: 25% del tiempo se va en buscar respuestas `[verificado: https://www.atlassian.com/blog/state-of-teams-2025 — 2026-09-23]`. Costo de la información perdida en general, no de Teams en particular.
- HBR (137 usuarios de 3 empresas Fortune 500): ~4 h/semana perdidas en cambiar de app `[verificado: https://hbr.org/2022/08/how-much-time-and-energy-do-we-waste-toggling-between-applications — 2026-09-23]`. **Juega en contra de A:** el multicanal también cuesta.
- Búsqueda en Teams: quejas en foros de Microsoft (señal) y un blog de G2 que dice lo contrario. Contradictorio.
- Empaquetado (sección 1): a nivel Business Premium, lo que hace barato "dejar registro" en Teams está detrás de licencias extra. Apoyo indirecto a A.

**(B) Hábito social: el equipo ya vive en WhatsApp/Slack**

- México, primera línea: la app ya está instalada, es más rápida, los supervisores la usan, hay desconfianza a las apps corporativas `[verificado: Xataka arriba y https://www.fayerwayer.com/moviles/2026/07/08/trabajadores-mexicanos-ya-usan-whatsapp-para-laborar-pero-muchas-empresas-aun-no-lo-formalizan/ — 2026-09-23]`.
- Computerworld (2015–2018): simple, familiar, "súper rápida"; entrar a apps corporativas es menos eficiente `[verificado: https://www.computerworld.com/article/1709323/whatsapp-at-work-companies-grapple-with-a-popular-ad-hoc-tool.html — 2026-09-23]`. Apoya B y en parte A.
- La participación de la alta dirección en canales prohibidos (CFTC) sugiere una norma social más que fricción puntual (inferencia).
- Que las respuestas lleguen más rápido por WhatsApp que por Teams entre trabajadores del conocimiento: **desconocido**.

**(C) Externos: Zoom/Meet en un clic**

- Microsoft tiene guías de troubleshooting para externos bloqueados y para cambiar de organización `[verificado: https://learn.microsoft.com/en-us/troubleshoot/microsoftteams/meetings/external-participants-join-meeting-blocked — 2026-09-23]`. La fricción existe; su frecuencia es desconocida.
- Facilitator y las notas de IA de Slack no funcionan con externos (sección 1): las herramientas de registro de Teams fallan justo en la reunión con gente de afuera.
- Proporción de reuniones con externos que se mueven a Zoom/Meet por esto: **desconocido**.

**Balance:** la evidencia pública apoya más a **B**, A tiene apoyo indirecto y C solo señales. Pero casi todo viene de primera línea, finanzas o encuestas viejas, no de Team Leads de tecnología distribuida.

## 3. Precios y modelo de compra: qué hace subir de tier

**Precios de lista Microsoft** (USD por usuario/mes, anual, 2026-09-23):

| Plan | Con Teams | Sin Teams | Fuente |
|---|---|---|---|
| Business Basic | $7,00 | $5,40 | `[verificado: página de comparación Business — 2026-09-23]` |
| Business Premium | $22,00 | desconocido | `[verificado: microsoft.com Business Premium — 2026-09-23]` |
| Business Premium with Copilot | $32,00 | $28,80 | `[verificado: microsoft.com/en-us/microsoft-365/business/microsoft-365-business-premium-with-copilot — 2026-09-23]` |
| E3 | $39 (antes $36) | $30,45 | `[verificado: microsoft.com enterprise plans — 2026-09-23]` |
| E5 | $60 (antes $57) | $51,45 | ídem |
| E7 "Frontier Suite" (E5 + Copilot + Agent 365 + Entra Suite), desde 1/05/2026 | $99 | $90,45 | `[verificado: https://blogs.microsoft.com/blog/2026/03/09/introducing-the-first-frontier-suite-built-on-intelligence-trust/ — 2026-09-23]` |
| Teams Premium (add-on) | $10 | — | `[verificado: microsoft.com/en-us/microsoft-teams/premium — 2026-09-23]` |
| Copilot Business (add-on) | $21 lista ($18 con promoción) | — | `[verificado: microsoft.com/en-us/microsoft-365/copilot/business — 2026-09-23]` |
| Copilot Enterprise (add-on) | $30 | — | `[verificado: microsoft.com/en-us/microsoft-365/copilot/enterprise — 2026-09-23]` |

**Qué mueve el upgrade en empresas:**

- **Negociación más que uso.** El paso E3 → E5 depende sobre todo del descuento de entrada que Microsoft retira en la renovación; solo seguridad y cumplimiento tienen peso real `[verificado: https://www.directionsonmicrosoft.com/microsofts-e5-step-up-does-it-make-sense-for-your-org/ — 2026-09-23]`.
- **El ROI de uso es difícil de demostrar.** Gartner 2025 (187 líderes de IT): solo 5% de quienes terminaron el piloto de Copilot pasó a despliegue amplio; el valor "remained elusive" `[verificado: https://www.techpartner.news/news/gartner-microsoft-copilot-hype-offset-by-roi-and-readiness-realities-618118 — 2026-09-23]`.
- **Presión de costo.** Inflación SaaS del 13,2% (Vertice) `[verificado: https://www.vertice.one/l/saas-inflation-index-report — 2026-09-23]`; 36% de las licencias infrautilizadas (Zylo 2026) `[verificado: https://zylo.com/news/2026-saas-management-index — 2026-09-23]`. Un CFO que ve licencias sin usar desconfía de un upsell "por uso".
- **Los datos de uso existen, pero para recortar.** Flexera 2026: optimizar gasto es la prioridad nº 1; se recomienda cruzar uso con costo `[verificado: https://www.flexera.com/blog/it-asset-management/state-of-itam-2026-saas-sprawl/ — 2026-09-23]`. Es la única fuente cercana al lado "uso", y apunta a bajar licencias, no a subir de tier (inferencia).
- **Microsoft, Q4 FY2026 (jul. 2026):** "Premium offerings, including Copilot, E5, and early traction in E7, drove ARPU growth"; más de 30 M de puestos de Copilot `[verificado: https://www.microsoft.com/en-us/investor/events/fy-2026/earnings-fy-2026-q4 — 2026-09-23]`. El motor declarado del upsell es seguridad + IA en bundle.
- Encuestas que midan el peso del uso frente al precio en upgrades de suites de colaboración: **desconocido**.

**Shadow IT:**

- Gartner: 41% de los empleados adquirió o creó tecnología fuera de IT en 2022; predice 75% en 2027 `[verificado: vía valencesecurity.com — 2026-09-23]`.
- Zylo 2026: 81% del gasto SaaS lo manejan las áreas de negocio; el gasto por notas de gastos creció 267% y ChatGPT es la app más pagada por esa vía `[verificado: zylo.com — 2026-09-23]`.
- **Implicación:** el shadow IT que hoy preocupa es IA, no chat ni reuniones. El argumento "baja el shadow IT" encaja mejor con Copilot/E7 que con funciones de reunión.
- Evidencia directa de que bajar el shadow IT dispara compras de suite: **desconocido**.

**Teams:** último MAU oficial, 320 M (oct. 2023) `[verificado: techcommunity.microsoft.com — 2026-09-23]`. Adopción de Teams Premium: no publicada.

## 4. Tendencias y posicionamiento: notas y decisiones con IA

| Producto | Cómo se posiciona | Precio | En vivo vs. después | Multiplataforma | Tracción |
|---|---|---|---|---|---|
| Copilot en Teams (Facilitator, recap) | Notas en tiempo real editables, Q&A, acciones | Copilot $21–30 | **Ambas**: la única apuesta fuerte por lo en vivo | Solo Teams; sin externos | — |
| Zoom AI Companion 3.0 | "Orquestación del trabajo" | Incluido en planes de pago | Sobre todo después | Sí: Teams y Meet | — |
| Gemini en Meet | Notas, próximos pasos, decisiones en Docs | Workspace que califica | Después (captura en tiempo real) | Solo Meet | — |
| Otter.ai | "Base de conocimiento corporativa" | Gratis; Pro $8,33; Business $19,99 | Mixto | Sí | USD 100 M ARR, 35 M+ usuarios `[verificado: otter.ai — 2026-09-23]` |
| Fireflies.ai | "Compañero de IA n.º 1 para reuniones" | Gratis; $10–39 | Después | Sí | Valuación > USD 1.000 M, 20 M+ usuarios `[verificado: fireflies.ai — 2026-09-23]` |
| Fathom | "Never take notes again" | Gratis individual | Después | Sí, sin bot | Comprada por Superhuman el 14/09/2026 `[verificado: techcrunch.com — 2026-09-23]` |
| Read.ai | Copiloto en reuniones, correo y chat | Gratis; $15–22,50 | Después + métricas | Sí, incluye Slack y Gmail | USD 81 M levantados `[verificado: read.ai — 2026-09-23]` |
| Granola | App de IA empresarial, sin bot | Gratis; $14–35 | Después | Sí | Valuación USD 1.500 M (mar. 2026) `[verificado: techcrunch.com — 2026-09-23]` |
| Notion AI Meeting Notes | Notas y seguimientos sin bot | Business $20+ | Después | Sí | desconocido |
| Fellow | Agenda, notas y grabación sin bot | Gratis; $7–25 | **Antes, durante y después** | Sí | desconocido |
| tl;dv, Avoma, Krisp | Ventas / audio | $8–30 | Después | Sí | desconocido |

Precios de Otter, Fireflies, Read, Granola, Notion, Fellow, Avoma y Krisp: `[verificado: páginas de precios de cada uno — 2026-09-23]`. tl;dv: `[conocimiento del modelo — verificar]`.

**Espacio saturado:** resumen, transcripción y acciones después de la reunión. Competir ahí no diferencia a Teams.

**Espacio vacío o poco atendido:**

- Decidir **durante** la reunión (agenda viva, votación, marcar "esto quedó decidido"): solo Facilitator y Fellow, y el Facilitator no funciona con externos.
- Un **registro de decisiones consultable entre reuniones** para quien no estuvo: Gemini detecta decisiones pero las deja en un Doc por reunión `[conocimiento del modelo — verificar que nadie lo ofrece]`.
- **Traer al registro lo decidido en WhatsApp/Slack:** ningún producto; Read.ai es lo más cercano.
- **Analítica para IT sobre dónde se coordina la gente:** ningún proveedor de colaboración. Solo herramientas de seguridad que detectan cuentas no aprobadas (Nudge Security: 800 cuentas nuevas de notetakers en 90 días en un cliente) `[verificado: nudgesecurity.com — 2026-09-23]`.

**Tendencias:**

- **Rechazo a los bots en reuniones.** Microsoft detecta bots externos en Teams, los manda al lobby y permite bloquearlos `[verificado: https://www.computerworld.com/article/4191798 — artículo del 01/07/2026, consultado 2026-09-23]`. El mercado responde con captura sin bot (Granola, Notion, Fathom, Krisp), aún más difícil de controlar para IT. Teams puede posicionarse como la opción gobernable.
- **Consolidación:** tomar notas pasa a ser una función de las suites, no una empresa. Los independientes se reposicionan como "contexto para agentes".
- **Riesgo del registro automático:** un analista advierte que los resúmenes de IA producen un registro "con apariencia de autoridad", a menudo erróneo `[verificado: computerworld, arriba]`. Una idea de notas que asienten decisiones solas necesitaría confirmación de los participantes.
- Tamaño de mercado de asistentes de reunión con IA: orden de miles de millones de USD hacia 2035; las fuentes no coinciden `[verificado: precedenceresearch.com — 2026-09-23]`.

---

## Impacto en creencias

| Creencia (de overview.md) | Veredicto | Evidencia |
|---|---|---|
| **#2** `[opportunity: colaboracion-fuera-de-teams] [value]` Quien convoca saca el trabajo en vivo de Teams porque decidir y dejar registro cuesta más ahí | **No la resuelve; las señales se inclinan hacia la rival B (hábito)** | Las fuentes de prevalencia citan rapidez, familiaridad y norma social (Xataka, Computerworld, CFTC: `[verificado]`, otros segmentos). A tiene apoyo indirecto: el registro para ausentes está detrás de licencias extra en Business Premium, mientras la competencia lo incluye (sección 1, `[verificado]`); 57% de reuniones improvisadas sin estructura (WTI, `[verificado]`). HBR muestra que el multicanal también cuesta (en contra de A). C se cruza con A: el Facilitator no funciona con externos. Ninguna fuente es del segmento |
| **#3** `[opportunity: colaboracion-fuera-de-teams] [viability]` IT sube a Max cuando puede demostrar que la coordinación volvió adentro y baja el shadow IT | **Contradice** (segmento de la fuente: enterprise E3/E5, no Business Premium) | El upgrade se decide por descuento y seguridad/cumplimiento (Directions on Microsoft, `[verificado]`); el ROI de uso es esquivo (Gartner, `[verificado]`); el upsell de Microsoft lo mueven Copilot/E5/E7 (earnings Q4 FY26, `[verificado]`); el shadow IT que preocupa hoy es IA (Zylo, `[verificado]`). La condición de caída ("se decide por precio, bundle o negociación") tiene más apoyo que la creencia |
| **#1** `[product] [value]` Si IT les dejara elegir, la mayoría no usaría Teams; ya usan canales paralelos | **Apoya a medias** | La parte "ya usan canales paralelos" tiene apoyo de prevalencia (41% UK, 76% primera línea MX, multas SEC/CFTC, `[verificado]`). Sobre qué elegirían si pudieran: nada |
| **#4** `[product] [value]` Quienes convocan le sacan más valor que quienes participan | **No dice nada** | Ninguna fuente distingue organizadores de participantes |

Un contradicho no mata la creencia #3: las fuentes hablan de enterprise, y el segmento es Business Premium ≤300 puestos. Pero sube su prioridad: la fila de la agenda "qué tienen en común las cuentas del 3,1% que upgradearon" y las entrevistas a IT pasan a ser lo primero.

## Qué sigue necesitando research primario

**Encuesta a Team Leads del segmento** (`/design-survey`, cuánto y con qué frecuencia):

- Qué porcentaje de sus reuniones incluye externos (separa C).
- En cuántos canales coordinan y cuántas veces por semana sacan una decisión de Teams.
- Qué licencias tienen activas (Teams Premium, Copilot): si la fricción A es de empaquetado, quien tiene Facilitator debería migrar menos.
- Horas por semana rearmando minutas y pendientes.

**Entrevistas con Team Leads** (`/design-interview`, por qué y qué hacen hoy):

- Reconstruir la última reunión cuya decisión salió de Teams: qué pasó, dónde se decidió, cómo se enteró quien no estuvo. Es lo único que separa A de B.
- Cómo encuentra hoy una decisión vieja quien no estuvo.

**Entrevistas con IT** (6–8 admins del segmento, upgradearon y no):

- Cómo se decidió el último cambio de tier: precio, bundle, negociación, seguridad o uso.
- Qué pide finanzas para aprobar un upgrade, y si "coordinación que volvió adentro" sería un argumento válido.
- Qué entienden por shadow IT hoy: ¿chat y reuniones, o IA?

**Datos internos** (fuera del alcance de este research): qué tienen en común las cuentas del 3,1% que upgradearon, y telemetría de reuniones sin notas ni actividad posterior.
