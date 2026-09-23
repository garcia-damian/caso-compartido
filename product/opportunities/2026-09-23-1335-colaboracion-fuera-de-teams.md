---
status: framed
segment: Cuentas Business Premium, 100+ licencias, sector tecnología, operación en 3+ países, facturación >USD 100M anuales. 12.400 cuentas y 2,1 millones de licencias. Equipos distribuidos, trabajo remoto o híbrido. Dentro de la cuenta, el rol afectado es quien convoca y conduce reuniones: Team Leads y mandos medios.
personas: lucia-ferreyra, raul-mendez, martin-sosa, sofia-paz
---

# Oportunidad: la colaboración en vivo se hace fuera de Teams

En equipos distribuidos de cuentas Premium grandes de tecnología, el trabajo real de una reunión —decidir, compartir, dejar constancia— se hace en canales paralelos (WhatsApp, mail, Zoom/Meet) y en Teams queda un registro incompleto, así que quien no estuvo en el canal paralelo se entera tarde o nunca. Importa ahora porque en este segmento solo el 3,1% de las cuentas subió de Premium a Max en 12 meses, y una herramienta que el equipo esquiva no sostiene un upgrade.

## Segmento y personas

- **Lucía Ferreyra** (primaria, convoca) — **sufre el problema**. Advertencia: tiene el rol correcto pero no la firmografía del segmento (logística, ~400 licencias, un país, híbrido con oficina).
- **Raúl Méndez** (secundaria, participa) — **sufre el efecto**, no la causa: se entera tarde, no encuentra los archivos. No elige el canal.
- **Martín Sosa** (terciaria, comprador) — **no sufre el problema del usuario**, pero paga el costo (shadow IT sin visibilidad) y es quien responde la creencia de viabilidad.
- **Sofía Paz** (negativa) — fuera de foco. Su dolor de invitada externa se usa solo como señal de la hipótesis rival, nunca como razón para construir.
- **Falta una persona:** Team Lead de una empresa de tecnología distribuida en 3+ países, 100+ licencias, equipo remoto. Nadie del set vive esa realidad. Conviene generarla después de `/research-market`, para que salga anclada en evidencia y no en la imaginación.

## Señales

| Señal | Procedencia | Fuente |
|---|---|---|
| El equipo contesta más rápido por WhatsApp que por Teams; una decisión tomada ahí no llega a quien no estaba, y termina en errores de despacho | `synthetic` | `product/personas/lucia-ferreyra.md` |
| ~4 h/semana rearmando minuta y pendientes a mano, sobre 10–15 reuniones semanales | `synthetic` | `product/personas/lucia-ferreyra.md` |
| El seguimiento de pendientes vive en un Excel que circula por mail, no en Teams | `synthetic` | `product/personas/lucia-ferreyra.md` |
| Aviso importante perdido por estar en un canal que no mira; archivos de reunión que después pide por mail | `synthetic` | `product/personas/raul-mendez.md` |
| Los equipos coordinan y comparten datos de clientes por WhatsApp, sin visibilidad ni control de IT | `synthetic` | `product/personas/martin-sosa.md` |
| Los reportes de uso del admin center no le sirven a IT para demostrar valor ante el CFO | `synthetic` | `product/personas/martin-sosa.md` |
| Un externo invitado pierde ~15 min por reunión para entrar a Teams (señal de la hipótesis rival "gente de afuera") | `synthetic` | `product/personas/sofia-paz.md` |
| Segmento: 12.400 cuentas, 2,1 millones de licencias | `unverified` | brief del caso |
| Upgrade Premium → Max en el segmento: 3,1% de las cuentas en 12 meses | `unverified` | brief del caso |
| "Si IT les dejara elegir, la mayoría no usaría Teams; ya usan canales paralelos" | `unverified` | `product/overview.md`, creencia [product] #1 |

Nada `real` todavía. El brief se sostiene en personas sintéticas y números sin fuente primaria: por eso la agenda de research es larga y arranca por lo gratis.

## Resultado de negocio

**Tasa de upgrade Premium → Max** en el segmento, hoy 3,1% en 12 meses. La dirección mira además retención en la renovación e ingresos por licencia. Tensión conocida y asumida: el problema lo sufre el Team Lead, el upgrade lo firma IT.

## Restricciones

- Presupuesto máximo USD 5M.
- CollabCon en 5 meses (≈ 22 de febrero de 2027): ahí se presentan los features.
- El empleado recibe Teams instalado y no elige: nada que dependa de que el usuario instale o contrate algo aparte.
- Cumplimiento multi-país: residencia de datos, retención y políticas de invitados externos.
- Límites de cualquier solución: facilidad de uso, accesibilidad, compatibilidad con Microsoft 365, privacidad y seguridad corporativas, tiempo real, impacto mínimo en el rendimiento de la reunión.

## Creencias

Registradas en `product/overview.md`, que es el único registro. Acá se referencian:

- `[opportunity: colaboracion-fuera-de-teams] [value]` En cuentas Premium grandes de tecnología distribuida, quien convoca saca el trabajo en vivo fuera de Teams porque decidir en el momento y dejar registro que encuentre quien no estuvo le cuesta más ahí que en el canal paralelo. Se cae si, al reconstruir su última reunión importante, la razón dominante resulta ser el hábito del equipo o el acceso de gente de afuera.
- `[opportunity: colaboracion-fuera-de-teams] [viability]` IT de esas cuentas sube a Max cuando puede demostrar ante finanzas que la coordinación volvió adentro y que baja el shadow IT. Se cae si IT declara que el upgrade se decide por precio, bundle o negociación, sin relación con el uso.
- Referencia: `[product] [value]` #1 del overview. Esta oportunidad es esa creencia acotada a un segmento y puesta a prueba.

## Agenda de research

| Creencia | Instrumento | Decisión que desbloquea | Para cuándo |
|---|---|---|---|
| viability | Datos que ya existen: qué tienen en común las cuentas del 3,1% que sí upgradearon | Si el uso no separa a las que upgradean, cambiar el resultado a retención antes de gastar en research | semana 1–2 |
| value | Datos que ya existen: telemetría del segmento (reuniones sin archivos ni notas, actividad posterior a la reunión) y tickets de soporte | Si el problema no se ve en datos propios, bajar la prioridad de la oportunidad | semana 1–2 |
| value | `/research-market` — cómo compiten Zoom, Meet y Slack en colaboración en vivo y qué se paga por eso | Descartar o sostener la hipótesis de fricción frente a la de externos; acotar la encuesta | semana 2–3 |
| value | `/design-survey` a Team Leads del segmento (n ≥ 150): cuántos canales usan, para qué, cuántas horas, y por qué el último caso salió de Teams | Cuál de las tres explicaciones rivales sobrevive. Recluta los opt-in para entrevistas | semana 4–6 |
| viability | Entrevistas con 6–8 admins de IT del segmento, incluyendo cuentas que upgradearon y cuentas que no | Si el upgrade es palanca alcanzable o hay que cambiar de resultado | semana 4–6 |
| value | `/design-interview` con 8–12 Team Leads, priorizando a quienes contradicen la creencia | Abrir o no la oportunidad a ideas | semana 6–8 |

Discovery tiene que cerrar alrededor de la semana 8 para que quede margen hasta CollabCon.

## Hipótesis rivales descartadas como foco (no como posibilidad)

Las dos explicaciones alternativas de por qué migra la colaboración quedan anotadas, porque la encuesta tiene que poder distinguirlas:

- **Hábito social del equipo:** migran porque el equipo ya vive en WhatsApp o Slack y ahí la respuesta llega en minutos. Si gana, ninguna función de reunión lo revierte.
- **Gente de afuera en la reunión:** migran a Zoom o Meet porque el externo entra en un click. Si gana, el problema es de acceso externo y esta oportunidad cambia de forma.

## Ideas candidatas (no evaluadas)

- Herramientas colaborativas integradas en la reunión (el pedido original con el que llegó esta oportunidad).
- Notas en vivo que dejen decisiones y responsables asentados solos.
- Pizarra compartida en la reunión.
- Agenda viva y votación rápida para decidir en el momento.
- Panel para IT que muestre coordinación recuperada y shadow IT desplazado.
- Entrada de externos en un click.

Ninguna evaluada. Están ahí para no perderlas, no para elegir.
