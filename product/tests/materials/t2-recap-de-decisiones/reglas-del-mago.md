# Reglas del mago (T2)

El mago hace de IA. Si el recap sale mejor de lo que saldría de una IA con la misma transcripción, el test mide algo que no existe.

## Qué usa

- **Solo la transcripción** de la reunión. Nada de audio, chat, contexto del equipo ni conocimiento previo del proyecto.
- No le pregunta nada al conductor antes de entregar.

## Cómo arma el recap

1. Lee la transcripción completa una vez antes de escribir.
2. **Va a "Decisiones"** solo lo que en la transcripción se cierra de forma explícita: alguien lo propone y alguien con autoridad lo acepta ("dale", "va", "hagámoslo así", "queda X para el jueves").
3. **Va a "¿Idea o decisión?"** todo lo que se habló como posible acción pero no se cerró: propuestas sin respuesta, "lo vemos", "habría que", acuerdos a medias. En "Por qué está acá" pone lo que lo hace dudoso, citando la transcripción si se puede.
4. **Campos:** responsable, fecha y porqué se copian como se dijeron. Si no se dijeron: `— (no se dijo en la reunión)`. No deduce fechas ("la semana que viene" se copia así, no se convierte en fecha), no asigna responsables por rol, no completa el porqué con criterio propio.
5. No corrige ambigüedades ni une dos ítems que parezcan lo mismo. No resume la conversación: si no es decisión ni dudoso, no va.

## Cómo siembra el error

Exactamente **uno** por recap.

1. Elige una idea que en la transcripción **no se decidió** (propuesta sin respuesta, descartada o postergada).
2. Que sea plausible y que generaría trabajo si se ejecutara. Que no toque personas, sueldos, despidos, clientes externos ni nada que pueda dañar si alguien lo lee.
3. La escribe en la tabla de **Decisiones**, sin marca de dudosa, con el mismo tono y largo que las demás.
4. Responsable, fecha y porqué: solo los que se mencionaron junto con esa idea. Si no se mencionaron, `— (no se dijo en la reunión)`, igual que en cualquier otro ítem. El error es presentar la idea como decisión; no se inventa nada más.
5. No la pone ni primera ni última de la tabla. Si la tabla tiene una sola decisión real, la pone segunda.
6. **Antes de compartir el documento**, la registra en `clave-de-respuesta.md`.

## Tiempos

- Entrega dentro de las **2 h** posteriores al fin de la reunión. Anota la hora de entrega en la hoja de captura.
- Si la transcripción no llega o está incompleta, no arma el recap: anota la reunión como no corrida y avisa al equipo.

## Qué no hace

- No le dice al conductor que hay un error sembrado ni le da pistas.
- No le recuerda que revise ni le pregunta cómo va. Solo responde si el conductor pregunta algo operativo (dónde está el documento, cómo avisar "listo").
