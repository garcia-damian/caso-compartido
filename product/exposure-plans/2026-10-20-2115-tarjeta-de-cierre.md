---
spec: product/specs/2026-10-13-2115-tarjeta-de-cierre.md
feature: tarjeta-de-cierre
mechanism: feature flags (recomendado)
---

# Plan de exposición: Tarjeta de cierre

## Hipótesis

Creemos que los conductores de reuniones de trabajo en cuentas Business Premium del segmento van a confirmar la tarjeta frente al grupo antes de cortar, en la mayoría de las reuniones con decisiones, y van a dejar de cerrar a mano después, porque el cierre a mano les cuesta tiempo y no resuelve la ambigüedad: cuando escriben el acta, el grupo ya no está.

Estamos equivocados si la confirmación se saltea o se pasa a "después" en más de 3 de cada 10 reuniones con decisiones, si toma más de 3 minutos, o si a las 2 semanas la proporción de decisiones ejecutadas distinto o no ejecutadas no es menor que con el recap estructurado posterior.

## Secuencia de creencias

1. **Los conductores reconocen en el borrador las decisiones de su reunión y lo usan como base del cierre.** Si el borrador no es confiable, no tiene sentido llevarlo frente al grupo.
2. **Los conductores confirman la tarjeta frente al grupo antes de cortar, en ≤ 3 min.** Es el corazón de la #7. Si no se sostiene, no hay nada confirmado que publicar.
3. **Los conductores dejan de cerrar a mano cuando lo confirmado se publica donde se ejecuta.** Es la segunda mitad de la #7 y cierra la parte de comportamiento de la hipótesis.

La comparación a 2 semanas contra el recap (#8) no agrega ninguna capa visible, así que va en *Validaciones en paralelo*.

## Nivel 1. Borrador privado para el conductor

- **Qué se revela:** a 5 minutos del final programado, el conductor ve solo para él un borrador con decisión, responsable, fecha y porqué, con lo dudoso vacío y marcado. También puede pedirlo antes y agregar decisiones a mano. Todavía están apagados compartir en la reunión, confirmar y publicar.
- **Creencia:** los conductores reconocen en el borrador las decisiones de su reunión y lo usan como base de su cierre en vez de escribirlo desde cero.
- **Audiencia:** conductores de cuentas piloto del segmento (Business Premium de 100 a 300 licencias, tecnología, 3 o más países) con transcripción habilitada, que conducen 2 o más reuniones de trabajo con decisiones por semana.
- **Duración:** 2 semanas.
- **Validación:**
  - **Avanzar si** el conductor abre el borrador en ≥ 7 de cada 10 reuniones con decisiones, conserva (tal cual o corregidos) ≥ 2 de cada 3 ítems y ≤ 1 de cada 10 ítems es una idea presentada como decisión.
  - **Detener si** más de 1 de cada 10 ítems es una idea presentada como decisión, o si en la segunda semana el conductor abre el borrador en menos de la mitad de las reuniones.

## Nivel 2. Confirmar frente al grupo

- **Qué se revela:** todo lo del Nivel 1, más compartir la tarjeta dentro de la reunión, editarla con el grupo presente, confirmar o descartar cada decisión y el bloqueo de las decisiones con campos dudosos sin resolver. Si la reunión termina sin confirmar, la tarjeta queda como borrador en el chat. La publicación sigue apagada.
- **Creencia:** los conductores confirman la tarjeta frente al grupo antes de cortar, en ≤ 3 min, en la mayoría de las reuniones con decisiones.
- **Audiencia:** la misma del Nivel 1, ampliada a otros conductores de las mismas cuentas piloto.
- **Duración:** 2 semanas.
- **Validación:**
  - **Avanzar si** la confirmación se hace frente al grupo en ≥ 7 de cada 10 reuniones con decisiones y la mediana es ≤ 3 min.
  - **Detener si** se saltea o queda como borrador en más de 3 de cada 10 reuniones, o si la mediana supera los 3 min. Si las fallas son solo de tiempo, se reduce la tarjeta (por ejemplo, solo responsable y fecha) y se repite el nivel.

## Nivel 3. Publicar donde se ejecuta

- **Qué se revela:** todo lo del Nivel 2, más la publicación de las decisiones confirmadas en el canal, Planner o Jira, con responsable y fecha asignados, el porqué y un enlace a la reunión. El destino se elige una vez por serie. Si el responsable no se puede asignar, la decisión se publica con su nombre en texto y queda marcada para el conductor.
- **Creencia:** cuando lo confirmado se publica donde el equipo ejecuta, los conductores dejan de cerrar la reunión a mano.
- **Audiencia:** los conductores de los niveles anteriores en cuentas cuyo IT habilitó el destino que usa el equipo.
- **Duración:** 3 semanas. Así entra el seguimiento a 2 semanas de la #8.
- **Validación:**
  - **Avanzar si**, en ≥ 7 de cada 10 reuniones confirmadas, el conductor no vuelve a cerrar a mano en las 48 h siguientes: no hay acta aparte, no hay tareas nuevas de esa reunión creadas a mano y no hay reescritura de lo publicado.
  - **Detener si** el conductor vuelve a cerrar a mano en más de 3 de cada 10 reuniones confirmadas. Eso quiere decir que la tarjeta se agrega al cierre manual en vez de reemplazarlo.

## Mecanismo de revelado

Se recomienda **feature flags**. Cada nivel apunta a una audiencia acotada: cuentas piloto del segmento, el rol de conductor y, en el Nivel 3, cuentas con el destino habilitado por IT. Con desarrollo incremental no se puede segmentar así. Ingeniería tiene la decisión final.

## Validaciones en paralelo

- **#8, comparación con el recap estructurado:** durante el Nivel 3, seguir a 2 semanas una muestra de decisiones de la tarjeta y otra del recap-de-decisiones (A3) en reuniones comparables, y contar cuántas se ejecutaron distinto o no se ejecutaron. Requiere seguimiento manual y un grupo de comparación, no una capa de producto.
- **#10, factibilidad de la extracción:** antes del Nivel 1, evaluar sin usuarios el borrador sobre transcripciones reales (cuántas ideas aparecen presentadas como decisiones, cuántos campos inventados, si llega a tiempo). Si falla, el Nivel 1 no tiene qué revelar.
- **#11, publicación con asignación:** antes del Nivel 3, una prueba técnica que confirme que se puede asignar responsable y fecha en Planner, Jira y el canal desde la reunión.
- **#13 y #2, viabilidad:** confirmar con IT de cuentas piloto qué licencia exige la tarjeta (sin licencia por participante), si sirve en reuniones con externos y si "las decisiones llegan a ejecutarse" pesa en la decisión de pasar a Max.
- **#3, el problema en el segmento:** durante el Nivel 1, registrar cuántas reuniones tienen decisiones y cuánto tarda hoy el cierre a mano, para tener la línea base dentro del segmento que las entrevistas no dieron.
- **Cumplimiento multi-país:** validar retención y residencia de las transcripciones y de lo publicado en las cuentas piloto, sobre todo las de la UE.

## Preguntas abiertas para el equipo de producto

- **T1 sigue sin correr.** Es un mago de Oz de una semana sobre la misma creencia que el Nivel 2. Si se descarta, este plan no aplica. ¿Se corre antes de construir?
- **Reclutamiento:** ¿alcanza el pool filtrado de la encuesta (64 candidatos) para sumar cuentas piloto del segmento, o hace falta ir por IT?
- **Cómo detectar el cierre a mano** sin observar al conductor: ¿alcanza con la telemetría de tareas creadas y ediciones más una pregunta corta a las 48 h?
- **Calendario:** los tres niveles suman unas 7 semanas, más la construcción. ¿Entra antes de CollabCon (≈ 22/02/2027)?
- **Reuniones con externos:** ¿quedan fuera del piloto hasta resolver la #13?
