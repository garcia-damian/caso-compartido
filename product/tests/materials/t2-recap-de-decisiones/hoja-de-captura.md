# Hoja de captura (T2)

Una fila por reunión en `hoja-de-captura.csv`. Horas en formato HH:MM, zona horaria del conductor anotada una vez por fila.

| Columna | Qué va | De dónde sale |
|---|---|---|
| conductor | código C1…C6 (no el nombre) | reclutamiento |
| procedencia | `segmento` (Business Premium 100–300) o `sustituto` (con el motivo: tamaño, licencia, etc.) | filtro de reclutamiento |
| orden | `T2-primero` o `T1-primero` | asignación alternada |
| fecha_reunion | AAAA-MM-DD | |
| zona_horaria | ej. `UTC-3` | |
| fin_reunion | hora | transcripción |
| entrega | hora en que el mago compartió el documento | mago |
| apertura | hora de "Empecé a revisar" | documento |
| apertura_control | primera edición del conductor en el historial / actividad del archivo | historial |
| publicacion | hora de "Listo para publicar" | documento |
| publicacion_control | hora del mensaje "listo" / última edición | chat / historial |
| revision_min | publicación − apertura, en minutos | calculado |
| revision_reportada_min | minutos que reporta el conductor | documento / debrief |
| marca_medicion | `ok`, `discrepancia` o `apertura estimada` | ver `medicion-de-revision.md` |
| decisiones_entregadas | cuántas filas tenía la tabla de Decisiones (incluida la sembrada) | recap entregado |
| dudosos_entregados | cuántos ítems en "¿Idea o decisión?" | recap entregado |
| items_corregidos | cuántos ítems editó (y cuáles, en notas) | comparación entregado vs. "listo" |
| items_borrados | cuántos borró | idem |
| dudosos_a_decision | cuántos pasó de dudoso a Decisiones | idem |
| dudosos_sin_resolver | cuántos dejó en "¿Idea o decisión?" sin borrar | idem |
| publico_algo_dudoso | `sí` / `no`: ¿publicó como decisión algo que en el recap estaba como dudoso, sin cambiarlo? | idem + debrief |
| sembrado_detectado | `sí` / `no` / `ver notas` (criterio en `clave-de-respuesta.md`) | comparación con la clave |
| sembrado_llego_al_destino | `sí` / `no`, y minutos visible si fue sí | protocolo de intercepción |
| destino | Jira / canal / Planner / otro | documento |
| publicacion_real | hora en que se publicó en el destino | mago |
| notas_debrief | citas textuales, tandas de revisión, lo que le hizo dudar, y si señaló el ítem sembrado antes de que se lo dijeran | debrief |
| incidencias | transcripción incompleta, reunión sin decisiones, publicó por su cuenta, etc. | mago |

## Cómo se lee contra el umbral

- **(a) Revisión:** cuenta las reuniones con `revision_min` < 5. Pasa con ≥ 4 de 5.
- **(b) Error sembrado:** cuenta las reuniones con `sembrado_detectado` = sí. Pasa con 5 de 5.
- Las filas con `discrepancia`, `apertura estimada` o `ver notas` se señalan aparte para el análisis; esta hoja no decide si cuentan.
