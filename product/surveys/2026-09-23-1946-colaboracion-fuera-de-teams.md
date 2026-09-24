---
opportunity: colaboracion-fuera-de-teams
research: product/research/2026-09-23-1508-colaboracion-fuera-de-teams.md
personas: andres-quintero, patricia-oliveira
status: draft
---

# Encuesta: decisiones de equipo que se toman fuera de Teams

- **Objetivos de aprendizaje:**
  1. **Cuál de las tres explicaciones sobrevive** —fricción para decidir y dejar registro (A), hábito del equipo (B), gente de afuera (C)— para la creencia #2 del overview. Decide: abrir la oportunidad a ideas, cambiarle la forma (acceso externo) o bajarla (si gana el hábito).
  2. **Cuánto pesa el problema**: en cuántos canales se coordina, con qué frecuencia una decisión sale de Teams, qué le pasa a quien no estuvo, cuántas horas se van en rearmar minutas. Decide: prioridad de la oportunidad frente a las demás.
  3. **Si usar las funciones de registro con IA (recap de Teams Premium, Copilot/Facilitator) cambia la migración**, es decir, si la fricción A es de empaquetado. Decide: a qué tier apuntar cualquier solución, e insumo para la creencia #3.
  4. **Reclutar entrevistados** para `/design-interview`, priorizando a quienes contradicen la creencia #2.
- **Respondentes:** Team Leads y mandos medios que convocan 3+ reuniones por semana, en empresas de tecnología de 100+ personas con operación en 3+ países, que usan Microsoft Teams provisto por la empresa. Personas de referencia: Andrés Quintero y Patricia Oliveira, que tienen el rol y la firmografía del segmento. El filtro igual es por firmografía, no por parecido a ellos.
- **Largo estimado:** 4 de filtro + 11 preguntas + 3 de reclutamiento, ~5 minutos.
- **Idioma:** español. Si el panel entrega respondentes fuera de LatAm/España, traducir antes de publicar ese link.

## Filtro

S1. ¿En qué industria trabaja tu empresa? [opción única]
   - Software / SaaS
   - Servicios de tecnología o consultoría IT
   - Hardware, telecomunicaciones o semiconductores
   - Otra industria
   → descalificar si "Otra industria"

S2. ¿Cuántas personas trabajan en tu empresa, aproximadamente? [opción única]
   - Menos de 100 · 100–300 · 301–1.000 · Más de 1.000 · No sé
   → descalificar si "Menos de 100" o "No sé"
   > Nota: el segmento es Business Premium (tope 300 licencias). Se acepta >300 personas porque la empresa puede tener más gente que licencias; se corta en el análisis.

S3. ¿En cuántos países tiene operaciones tu empresa? [opción única]
   - 1 · 2 · 3 a 5 · Más de 5 · No sé
   → descalificar si "1", "2" o "No sé"

S4. En una semana típica, ¿cuántas reuniones convocás vos (no solo a las que te invitan)? [opción única]
   - Ninguna · 1–2 · 3–5 · 6–10 · Más de 10
   → descalificar si "Ninguna" o "1–2"
   > Nota: en el link del panel, agregar antes "¿Tu empresa te da Microsoft Teams para trabajar? [sí / no]" → descalificar si "no". En el link in-product no hace falta.

## Preguntas

Q1. En la última semana laboral, ¿por cuáles de estos medios coordinaste trabajo con tu equipo? [opción múltiple, orden aleatorio salvo las dos últimas]
   - Chat o canales de Teams
   - Reuniones de Teams
   - WhatsApp
   - Slack
   - Correo electrónico
   - Zoom
   - Google Meet
   - Llamada telefónica
   - Otro: ___
   > Objetivo: 2 (cuántos canales conviven)

Q2. En las últimas 2 semanas, ¿cuántas veces se tomó una decisión sobre el trabajo de tu equipo por un medio que no fue Teams (WhatsApp, Slack, correo, Zoom, Meet, teléfono o en persona)? [opción única]
   - Ninguna · 1–2 · 3–5 · 6–10 · Más de 10 · No sé
   → si "Ninguna" o "No sé", saltar a Q7
   > Objetivo: 2 (frecuencia) y condición para 1

Q3. Pensá en **la última vez** que eso pasó. ¿Por dónde se tomó esa decisión? [opción única]
   - WhatsApp · Slack · Correo electrónico · Zoom · Google Meet · Llamada telefónica · En persona · Otro: ___
   > Objetivo: 1 (Zoom/Meet apunta a C; WhatsApp/Slack a B o A)

Q4. En esa conversación, ¿participaba alguien de fuera de tu empresa (cliente, proveedor, socio)? [opción única]
   - Sí · No · No me acuerdo
   > Objetivo: 1 (dato de hecho que separa C, independiente de la razón declarada)

Q5. ¿Cuál fue la razón principal de que esa decisión se tomara ahí y no en Teams? [opción única, orden aleatorio salvo las dos últimas]
   - Había gente de fuera de la empresa y así era más fácil que participaran *(C)*
   - La conversación ya estaba pasando en ese medio *(B)*
   - Ahí la gente responde más rápido *(B)*
   - Ahí era más fácil trabajar juntos sobre algo (un archivo, una pantalla, una pizarra) *(A)*
   - Ahí era más fácil dejar escrito qué se decidió y quién hace qué *(A)*
   - Otra: ___
   - No hubo una razón, simplemente pasó ahí *(B)*
   > Objetivo: 1. Las etiquetas A/B/C son internas: no van en la herramienta. Se cruza con Q3 y Q4; si la razón declarada y el hecho no coinciden (p. ej. "gente de afuera" con Q4 = No), manda el hecho.

Q6. Después de esa decisión, ¿cómo se enteraron las personas del equipo que no participaron? [opción única]
   - Se la conté o reenvié yo después
   - Quedó escrita en un lugar donde el resto la ve sin que se la pasen
   - Se enteraron cuando preguntaron o cuando hizo falta
   - Alguien no se enteró a tiempo y hubo que corregir algo
   - Estaban todos los que tenían que estar
   - No sé
   > Objetivo: 2 (costo para quien no estuvo, el efecto que sufre Raúl) y 1 (si "quedó escrita", la fricción A no aplica en ese caso)

Q7. De las reuniones que convocaste en las últimas 2 semanas, ¿cuántas incluyeron a alguien de fuera de tu empresa? [opción única]
   - Ninguna · Menos de la cuarta parte · Entre la cuarta parte y la mitad · Más de la mitad · Todas · No sé
   > Objetivo: 1 (peso de la hipótesis C en el trabajo de cada respondente, no solo en el último caso)

Q8. En la última semana, ¿cuánto tiempo en total dedicaste, después de tus reuniones, a pasar en limpio lo decidido y mandar los pendientes? [opción única]
   - Nada · Menos de 30 min · 30 min a 1 h · 1 a 2 h · 2 a 4 h · Más de 4 h
   > Objetivo: 2 (horas perdidas; las señales sintéticas son ~3 h de Andrés y ~4 h de Lucía)

Q9. ¿Cuáles de estas funciones usaste en tus reuniones de Teams en el último mes? [opción múltiple]
   - Resumen de la reunión generado por IA (recap inteligente)
   - Copilot durante o después de la reunión
   - Notas de reunión compartidas (Loop / notas colaborativas)
   - Pizarra (Whiteboard)
   - Encuestas o votaciones (Forms)
   - Ninguna de estas
   - No sé
   > Objetivo: 3. Se pregunta uso, no licencia: el Team Lead suele no saber qué licencia tiene. En el link in-product, cruzar además con la licencia real del tenant vía campo oculto.

Q10. ¿Qué es lo más difícil hoy de coordinar decisiones con tu equipo? [abierta, opcional]
   > Objetivo: 1 y 2. Codificar por A / B / C / otra; es la que sostiene o desarma lo que dicen Q3–Q5 con palabras propias.

Q11. ¿Cuántas personas tiene el equipo que conducís? [opción única]
   - 1–4 · 5–9 · 10–15 · Más de 15
   > Objetivo: corte del análisis (el costo de Q6 y Q8 puede escalar con el tamaño)

## Filtro + opt-in (reclutamiento para entrevistas)

R1. ¿Trabajás en Microsoft, Zoom, Google, Slack/Salesforce o en una consultora de investigación de mercado o UX? [sí / no]
   → no es candidato si "sí"
   > Condición adicional, sin pregunta: no es candidato si Q2 = "Ninguna" o "No sé" (la entrevista reconstruye un caso real y hace falta tener uno).

R2. ¿Aceptarías una conversación de 30 minutos por videollamada sobre cómo coordina decisiones tu equipo? [sí / no] {agregar incentivo si lo hay}

R3. Si respondiste que sí, ¿cómo te contactamos? [abierta, opcional: correo o LinkedIn]
   > En el link del panel, reemplazar R3 por el ID del panel: la re-invitación se hace desde el panel (suelen prohibir pedir contacto directo).

## Distribución

| Canal | A quién llega y su sesgo | Alcance aprox. | Link |
|---|---|---|---|
| Encuesta in-product en Teams, dirigida a organizadores de reuniones en cuentas del segmento | Team Leads que siguen abriendo Teams. **Canal propio: sobre-representa a quien todavía coordina en Teams y está conforme**, y sub-representa justo a quien migró. Firmografía conocida por el tenant | unknown (pool del segmento: 12.400 cuentas, 2,1 M licencias `[unverified]`; cuántos organizadores ven el aviso, sin dato) | `?canal=inproduct` + campo oculto con la licencia del tenant (Premium / Teams Premium / Copilot) |
| Panel B2B pago (p. ej. Respondent o User Interviews), filtrado por cargo, industria tecnología, tamaño y multi-país | Team Leads del segmento sin depender de que abran Teams: llega a quien ya se fue. Sesgo: gente que responde encuestas por incentivo; firmografía autodeclarada (por eso S1–S4 se repiten) | unknown: pedir el feasibility count al panel antes de comprar | `?canal=panel` + ID del respondente del panel |

- **n objetivo:** ≥100 completas por canal (≥150 en total según la agenda). Dentro del total: ≥100 con al menos una decisión fuera de Teams (Q2 ≥ 1–2), que son las que responden al objetivo 1; y ≥30 que usan recap o Copilot (Q9) contra ≥30 que no, para el objetivo 3. Con menos de 30 en una celda, ese corte es direccional.
- **Riesgo de n:** el filtro combinado (tecnología + 100+ personas + 3+ países + convoca 3+ reuniones) es angosto; en panel es esperable que pase una minoría de los que entran. Si el feasibility count del panel no da para ~100 completas, decidirlo antes de publicar: abrir S3 a 2+ países o subir presupuesto, no descubrirlo en el análisis. El grupo de uso de recap/Copilot puede no llegar a 30 si la adopción de Teams Premium es baja (no publicada).
- **Lanzamiento:** ~12 de octubre de 2026.
- **Primera revisión:** 26 de octubre de 2026 (deja margen para reclutar las entrevistas de las semanas 6–8).
- **Cierre:** abierta hasta el n objetivo.
