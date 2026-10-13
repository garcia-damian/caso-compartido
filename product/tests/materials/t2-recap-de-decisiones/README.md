# Material de T2 · recap-de-decisiones (mago de Oz)

Test: `product/tests/2026-10-06-2056-decisiones-no-llegan-a-ejecucion.md` → T2.
Creencia #9: un recap estructurado deja la revisión del conductor en < 5 min y no hace llegar a ejecución ninguna decisión inventada.

**Lo que este material tiene que hacer observable:** (a) los minutos entre que el conductor abre el recap y lo publica; (b) si la decisión sembrada sale publicada como firme. Lo ve el equipo de producto en la hoja de captura; el conductor no sabe que hay un error sembrado.

## Piezas

| Archivo | Para quién | Cuándo |
|---|---|---|
| `mensaje-de-reclutamiento.md` | conductores (compartido con T1) | semana de reclutamiento |
| `consentimiento.md` | conductor + aviso al grupo | antes de la reunión |
| `plantilla-recap.md` | el mago arma el recap; lo ve el conductor | dentro de las 2 h posteriores |
| `reglas-del-mago.md` | el mago | antes y durante el armado |
| `clave-de-respuesta.md` | solo el mago y el equipo | antes de entregar cada recap |
| `medicion-de-revision.md` | el mago | entrega → publicación |
| `protocolo-de-intercepcion.md` | el mago | entre "listo" y la publicación real |
| `guion-de-debrief.md` | quien hace el debrief | dentro de las 24 h |
| `hoja-de-captura.md` + `hoja-de-captura.csv` | el equipo | una fila por reunión |

## Flujo por reunión

1. El conductor confirma la reunión elegida (la que no usó en T1) y que la transcripción va a estar activa. Avisa al grupo con el texto de `consentimiento.md`.
2. Terminada la reunión, el conductor comparte la transcripción con el mago.
3. El mago arma el recap con `plantilla-recap.md` siguiendo `reglas-del-mago.md`, siembra un error y lo anota en `clave-de-respuesta.md` **antes** de entregar.
4. Entrega dentro de las 2 h, como documento compartido (ver `medicion-de-revision.md`).
5. El conductor revisa a solas y marca "Listo para publicar". El mago publica su versión en el destino elegido, aplicando `protocolo-de-intercepcion.md`.
6. Debrief de 10 a 15 min con `guion-de-debrief.md`.
7. Se completa la fila de `hoja-de-captura.csv`.

## Fuera a propósito

Resumen de la conversación, integración real con Jira, Planner o el canal, automatización y diseño visual. El recap es un documento de texto plano.
