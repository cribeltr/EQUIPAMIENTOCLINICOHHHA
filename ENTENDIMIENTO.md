# Entendimiento del Proceso — Sistema de Gestión MP 2026

> **Documento vivo.** Aquí se acumula el entendimiento de **mi trabajo** (el del encargado de
> Equipamiento Clínico del HHHA), el **porqué** de cada cosa que pido y cómo la aplicación me
> apoya. Se actualiza con **cada ajuste**. Cuando ya no haya más ajustes, esto es lo que define
> la **aplicación oficial final** que se adapta a mi día a día.
>
> *Está escrito en primera persona, tal como lo expliqué, para poder leerlo y confirmar que se
> entendió todo. Si algo no calza con la realidad, se corrige aquí primero.*

_Última actualización: 2026-06-16 · App build 2026-06-16.49_

---

## 1. Quién soy y cuál es mi foco

Soy el encargado del **Equipamiento Clínico del HHHA** y gestiono el **Programa de Mantenciones
Preventivas 2026 (MP 2026)** de ~966 equipos.

**Mi foco real no es llenar planillas: es saber en todo momento el estado de cada equipo y
asegurar su operatividad.** El último estado de un equipo vale más que el detalle histórico. Todo
lo que hago (preventivos, reprogramaciones, correctivos, pendientes) existe para que los equipos
estén operativos y para dejar constancia oficial de lo que se hizo.

---

## 2. La idea central: dos mundos que se complementan

Trabajo con **dos soportes**, y entender la diferencia es la clave de todo:

| | **La carta (Excel)** | **La aplicación** |
|---|---|---|
| Qué es | El **documento oficial** | El **detalle y el borrador** |
| Qué guarda | **Solo resultados** (códigos: `Si`, `C1–C8`, `FS`, `No`, `NU`, `Baja`, `Si-RA`) | **Todo el detalle** que la carta no guarda (ejecutor, fechas reales, observaciones, gestiones, documentos, firmas, expedientes…) |
| Estado | Lo que está en la carta es **oficial**; lo no oficial lo marco **en rojo** | Lo que registro en la app es **borrador** hasta que lo oficializo |

- **La carta solo registra resultados, no detalles.** Por eso la aplicación me ayuda: ahí pongo
  el detalle, hago seguimiento y veo qué falta.
- **Qué significa «oficial» para mí:** un registro es oficial **cuando archivo los documentos en la
  carpeta física del equipo y escribo el resultado en la carta**. Antes de eso, no es oficial.
- **El rojo de la carta es binario; el borrador de la app es el detalle.** En la carta, sin el
  programa, yo completo lo que tengo y lo marco **en rojo** para saber que aún no es oficial. Pero el
  rojo no dice **qué falta**: por ejemplo, una causal **C6 en rojo** que no está en la carpeta —
  ¿falta generar el reporte de reprogramación?, ¿falta imprimirlo?, ¿faltan las firmas? *No se sabe.*
  El concepto de **borrador** en la app es ese mismo «no oficial», **pero con todo el detalle**: me
  dice exactamente en qué etapa está y qué falta para oficializarlo.
- **El puente entre los dos mundos** es la regla **Borrador → Oficial**: lo que registro en la app
  como *Borrador* pasa a *Oficial* cuando **recargo la carta** y esa mantención ya aparece con su
  resultado. Si no aparece, sigue como borrador.

> En una frase: **la app es donde trabajo y acumulo el detalle; la carta es donde queda lo oficial.**
> El rojo de la carta dice «esto no es oficial»; el borrador de la app dice además **«y esto es lo que falta»**.

---

## 3. El flujo de documentos (el corazón de mi día a día)

Este es el ciclo que repito todo el tiempo:

1. **Recibo un documento** (un informe, un reporte, una orden, un reporte de reprogramación…).
2. **Lo ingreso en la aplicación** con todo su detalle (la carta no guarda ese detalle).
3. **Hago seguimiento hasta tenerlo completo** ("hasta la fecha"): la app me ayuda a ver qué le
   falta a ese documento/gestión.
4. Cuando el documento **ya no le falta nada**:
   - lo **agrego a la carpeta física del equipo** (cada equipo tiene su **N° de Carpeta**),
   - lo **actualizo en la carta (Excel)** escribiendo el resultado,
   - y al **recargar la carta** en la app, **queda oficial**.

La aplicación, entonces, es mi **mesa de trabajo**: me ordena los documentos en curso, me dice qué
falta para cerrar cada uno, y cuando lo oficializo en la carta, todo queda consistente.

---

## 4. Mantenimiento Preventivo (MP)

- Cada equipo tiene su **programación anual** por mes (`X` programada, `R` reprogramada,
  `RA` reprogramada de año anterior, `PM` puesta en marcha).
- Cuando ejecuto un preventivo registro el detalle en la app: fecha, ejecutor, resultado,
  observaciones, **estado del equipo** y el **tipo de mantenimiento: Interno o Externo**.
- Cuando la MP es **Externa**, registro además el **ingeniero externo y la empresa** (los datos del
  protocolo de mantenimiento externo). Esos datos viajan al pendiente del protocolo.
- Si queda una **gestión pendiente**, la app me crea un **pendiente** con su lista de trabajo:
  - **Interno** → protocolo de mantenimiento interno (ejecutor interno + el checklist).
  - **Externo** → protocolo interno **y** externo (con el ingeniero/empresa externos).
  - Cada protocolo se marca **Sí / No / Imprimir / Gestión**, admite comentarios, y cuando lo dejo
    en **Gestión** puedo abrir **subtareas** para detallar qué hay que gestionar.

**Por qué:** el resultado va a la carta, pero el *cómo* y el *qué falta* viven en la app.

---

## 5. Reprogramaciones (cuando una preventiva no se puede hacer)

Cuando una MP no se puede ejecutar, se **reprograma** con una **causal C1–C8** (p. ej. *C6: no
disponibilidad de horas del servicio técnico externo*). Esto **no es solo escribir un código**:
detrás hay un **documento (reporte de reprogramación) que debo tramitar**.

**El ciclo del reporte de reprogramación (y el porqué de cada paso):**

1. **Generar el documento** — el reporte lo genero yo; lleva la **causal** (p. ej. C6) y la
   **fecha** de la mantención reprogramada (p. ej. 30‑04‑2026).
2. **Imprimirlo.**
3. **Firmas** — lleva **dos**: la del **supervisor del servicio clínico** y la del **jefe de
   equipos médicos**. *(Por eso me conviene agrupar las reprogramaciones por servicio: junto las
   de cada servicio para conseguir la firma de su supervisor de una sola vez.)*
4. **Oficializar** — recién cuando el documento está **firmado**, escribo el código (C6) en la
   **carta (Excel)**, en el Resultado del mes que corresponde, y lo recargo. Ahí pasa de borrador
   a **oficial**.
5. **Cerrar el pendiente.**

**Por qué este orden:** mientras no esté firmado, no es oficial. La app me sirve para tener el
borrador, ver en qué etapa va cada reporte (por generar / por imprimir / por firmar / por
oficializar / oficializado) y, cuando está firmado, me indica **exactamente qué código y en qué
columna del Excel** escribir. Cuando recargo la carta con ese código, la app lo detecta y me
recuerda **cerrar** el pendiente.

> Esta es exactamente la diferencia con el **rojo de la carta** (sección 2): donde el Excel solo
> dice «esta C6 no es oficial», la app responde **«está por generar / por imprimir / le faltan
> firmas / lista para oficializar»**. Ese es el «borrador con mucho más detalle» que necesito.

---

## 6. Mantenimiento Correctivo

Cuando un equipo falla, se abre **mantenimiento correctivo**:

- Una **Orden de Trabajo (OT)** con su **Folio SIGEM** agrupa todo el **expediente** (la OT, sus
  reportes de servicio y los envíos a servicio técnico).
- El expediente avanza por etapas: **Apertura → (cotización) → Informe técnico → Orden de Compra →
  Ejecución → Cierre**, con **Trato Directo** o **Compra Ágil**.
- Lo crítico es la **operatividad**: si el equipo queda **No Operativo** o **en Servicio Técnico**,
  cuento los **días detenido**; si siguió operativo, es el ciclo administrativo.
- Los **envíos a servicio técnico** se registran como un **documento de envío** con su **N° de
  envío**, su **responsable**, su **fecha** y la **OT** a la que se asocian (el expediente). Debo
  poder **buscar por ese número** ("¿tienes el envío 166?").
- Cuando el equipo **es reparado o diagnosticado por personal externo**, lo registro como un
  **Reporte de Servicio**: **fecha, ingeniero externo, empresa y N° de reporte de servicio**, y si
  fue **reparación o diagnóstico** (+ cómo quedó el equipo). No lleva tipo de compra y se engancha al
  expediente abierto. La **reparación** y el **diagnóstico** externos registran los mismos datos.
- Cuando **el equipo llega** (retorno), registro la **fecha**, el **N° de guía de despacho** y **si
  viene o no con su reporte de reparación**. Si **no viene**, la app me deja un **pendiente** para
  gestionarlo; también puede ser que **ya había llegado antes por correo**.
- Los **ingenieros externos** son una **lista reutilizable** (como las empresas): los elijo rápido y
  puedo agregar nuevos al vuelo.
- Puedo registrar una **Visita diagnóstica** como tipo de evento del correctivo: una visita técnica
  para diagnosticar. **No implica compra** (no pide tipo de compra) y su folio es **opcional** —si el
  equipo ya tiene un expediente abierto, la visita se **engancha sola** a ese folio; si no, queda
  como un evento suelto. Igual que el resto, puede quedar **Borrador** hasta archivar su documento.

---

## 7. Pendientes y gestión

Los **pendientes** son las gestiones que quedan asociadas a un equipo (reprogramaciones,
protocolos, monitoreos, documentos por imprimir, etc.). Para cada uno llevo: fecha de compromiso,
responsables, tareas y una **bitácora de gestión**. La **fecha de compromiso de un pendiente que
nace de un evento** (una mantención o una reprogramación) es **la fecha de ese evento**.

Necesito **encontrarlos rápido** y **trabajarlos por lote** (p. ej. "todos los reportes por firmar
de tal servicio"), y poder **ver/exportar las columnas del equipo** que me sirvan en cada caso.

---

## 8. Operatividad (el tablero que responde "¿en qué está cada equipo?")

De todo lo anterior, la app deriva **una sola verdad por equipo**: su **estado** (Operativo / No
Operativo / Servicio Técnico), su **criticidad** y la **siguiente acción** recomendada para
asegurar la operatividad. Así, en una mirada, sé qué equipos necesitan atención y qué hacer con
cada uno, sin tener que reconstruirlo a mano.

En la **ficha de cada equipo** tengo además su **bitácora**: una fila por evento con su fecha y
estado, en orden cronológico (órdenes de trabajo, reprogramaciones, mantenciones, envíos, retornos,
cierres, pendientes). Es el relato de *qué le ha pasado y cuándo* — el complemento histórico del
estado actual.

Como apoyo a la operatividad existe también el **panel de Verificación**: la app revisa sola la
**consistencia de los datos** y me lista las situaciones que merecen una mirada (equipos detenidos
sin OT que los respalde, expedientes sin avance hace semanas, reportes de reprogramación vencidos o
firmados sin oficializar, MP de meses pasados sin resultado, FS/NU sin resolución, envíos sin
retorno, pendientes muy atrasados). Cada hallazgo lleva directo a la ficha del equipo. **No inventa
ni descarta nada**: solo señala lo que no calza para que yo decida.

Desde la ficha puedo **imprimir una hoja limpia del equipo** («🖨 Imprimir ficha») para archivar en
su **carpeta física**: lleva la identificación completa, el estado actual con la siguiente acción y
la **bitácora completa** en orden cronológico, más la fecha de generación y una línea de firma. Es
el puente entre la app y el papel que vive en la carpeta de cada equipo.

---

## 9. Principios que deben guiar la aplicación final

1. **La app no reemplaza a la carta; la complementa.** La carta manda en lo oficial (resultados);
   la app manda en el detalle y el seguimiento.
2. **Nada se da por oficial hasta que está en la carta.** Borrador hasta que se recarga con su
   resultado.
3. **El foco es la operatividad**, no el papeleo: todo debe ayudar a saber el estado y la
   siguiente acción.
4. **Cada documento tiene su ciclo** (recibir → detallar → completar → carpeta + carta → oficial),
   y la app debe acompañar ese ciclo, no entorpecerlo.
5. **Lo que hago a diario debe ser rápido**: buscar, filtrar por servicio/mes, trabajar por lote,
   ver/exportar solo lo que necesito.
6. **Mi trabajo no se pierde en silencio.** La app guarda en **IndexedDB** (cuota amplia, fiable
   también al abrir el archivo localmente) con localStorage como respaldo; cuida primero los datos
   irrecuperables, avisa de forma visible solo si **ningún** almacén pudo guardar, y tolera respaldos
   antiguos o parciales sin caerse. Ante la duda, siempre puedo descargar un respaldo.

---

## 10. Registro acumulativo de ajustes (qué pedí y por qué)

> Cada entrada deja constancia del **ajuste** y, sobre todo, del **porqué** (mi necesidad real).

| Fecha | Ajuste | Por qué lo necesito |
|------|--------|---------------------|
| 2026‑06‑15 | Columnas de equipo (ID, N° Carpeta, Unidad, Ubicación, Procedencia, Marca, Modelo, Serie…) y **Carta Gantt** filtrable tipo Excel en el Plan | Ver el plan como lo veo en la carta y ubicar equipos por sus datos reales |
| 2026‑06‑15 | Búsqueda de Pendientes por tarea, inventario, serie y cualquier campo | Encontrar un pendiente por cualquier dato, no solo por el equipo |
| 2026‑06‑16 | **Tipo de mantenimiento (Interno/Externo)** y **protocolo de tareas** (Sí/No/Imprimir/Gestión + comentarios) | El resultado va a la carta, pero el detalle del protocolo lo llevo en la app |
| 2026‑06‑16 | El **tipo de pendiente** arma su checklist; no perder texto sin agregar | Que al elegir "Protocolo…" aparezca la lista sola, también en pendientes existentes |
| 2026‑06‑16 | **Motor de estado integral**: estado + criticidad + **siguiente acción** por equipo, conectando todo | Saber de una el estado de cada equipo y qué hacer, sin rearmarlo a mano |
| 2026‑06‑16 | **Subtareas** cuando un protocolo queda en **Gestión** | Desglosar qué hay que gestionar (p. ej. generar documento, firmas) |
| 2026‑06‑16 | **Reprogramación con ciclo de reporte** (generar → imprimir → 2 firmas) + columna y chips por etapa | Tramito un documento con firmas, no solo escribo un código; necesito ver en qué etapa va cada uno |
| 2026‑06‑16 | El reporte conserva su **causal y su fecha** (la de la MP) | El documento lleva esa causal y esa fecha; debo verlas sin buscarlas |
| 2026‑06‑16 | **Envíos buscables** por N° (global y en Correctivos) + columna N° Envío | Me preguntan "¿tienes el envío 166?" y debo encontrarlo al instante |
| 2026‑06‑16 | **Selector de columnas en Pendientes** (todas las del equipo, ver y exportar) y **orden** ID→…→Clasificación | Armar y exportar la vista de pendientes con las columnas que me sirvan |
| 2026‑06‑16 | **Compromiso = fecha del evento** (mantención/reprogramación) | Que el pendiente refleje la fecha real del evento que lo originó |
| 2026‑06‑16 | **«← Volver»** regresa a la vista de origen | Si entré desde Pendientes, volver a Pendientes, no a Equipos |
| 2026‑06‑16 | **Oficializar y cerrar** la reprogramación: la app indica **qué código y en qué columna del Excel** y, al recargar la carta, sugiere cerrar | Cerrar el ciclo: firmado → escribo el código en la carta → recargo (oficial) → cierro |
| 2026‑06‑16 | El respaldo no guarda columnas derivadas (se recalculan) | Respaldos más livianos para traspasar/guardar |
| 2026‑06‑16 | **Bitácora del equipo** en la ficha: una fila por evento con su fecha y estado (MP, reprogramaciones, OT, envíos, retornos, cierres, pendientes) en orden cronológico | Ver de un vistazo *qué ocurrió y cuándo* con cada equipo, sin reconstruirlo a mano |
| 2026‑06‑16 | Un **pendiente nuevo** parte **limpio** (tipo «Otro», sin checklist); el checklist aparece solo al **elegir** un tipo de protocolo/reprogramación | No quiero que se arme una lista por defecto en cualquier pendiente que creo |
| 2026‑06‑16 | **Archivo de grabaciones** en el repo (`grabaciones/`) + `GRABACIONES.md` con qué reveló cada una | Que el repositorio guarde las grabaciones y para qué sirvieron (entendimiento acumulativo) |
| 2026‑06‑16 | **Tablero de Inicio «¿qué hago hoy?»**: la app abre con el resumen accionable del día (equipos detenidos, OT por avanzar, reprogramaciones por etapa, MP del mes, pendientes vencidos) y los equipos más críticos; cada tarjeta lleva a su vista | Empezar el día sabiendo de inmediato qué tengo que hacer, sin armarlo a mano |
| 2026‑06‑16 | **Bitácora clickeable**: cada fila de la bitácora del equipo abre su evento de origen (la reprogramación/pendiente, la MP o el expediente) | Cuando veo un evento en la bitácora quiero ir directo a trabajarlo |
| 2026‑06‑16 | **Repaso de clickeabilidad**: filas del Historial → editar la mantención; filas del detalle de Correctivo → editar el evento (antes solo el botón ✎) | Que todo lo que parece clickeable lo sea, y poder ir directo a editar desde la fila |
| 2026‑06‑16 | Se **elimina la línea de tiempo** de los expedientes en la ficha | No me servía de mucho; la bitácora ya cuenta la historia |
| 2026‑06‑16 | **Bitácora filtrable**: chips por categoría (Preventivo/Reprogramación/Correctivo/Pendiente) y búsqueda | Encontrar rápido lo que busco dentro de la historia del equipo |
| 2026‑06‑16 | **Registro rápido de avances correctivos** (➕ Avance) desde la vista Correctivos, sin entrar a la ficha | Reviso carpetas y necesito registrar envíos/recepciones rápido; la vía actual era lenta |
| 2026‑06‑16 | **Grabación más inteligente**: captura la entidad de cada clic y detecta **clics muertos** | Que la grabación me sirva para que infieras lo que busco con cada clic |
| 2026‑06‑16 | **Panel de Verificación de inconsistencias**: la app revisa la calidad de los datos (detenidos sin OT, expedientes estancados, reportes vencidos/firmados sin oficializar, MP vencidas, FS/NU sin resolver, envíos sin retorno, pendientes muy atrasados); cada hallazgo abre la ficha | Detectar de una lo que no calza, sin descartar ni inventar nada, para corregirlo antes de oficializar |
| 2026‑06‑16 | **Imprimir ficha del equipo** («🖨 Imprimir ficha»): hoja limpia con identificación, estado, siguiente acción y bitácora completa + línea de firma, lista para la carpeta física | Necesito una versión en papel ordenada para archivar en la carpeta física de cada equipo |
| 2026‑06‑16 | **Resguardo ante almacenamiento lleno**: si el navegador no puede guardar, la app prioriza mi trabajo (mantenciones/pendientes/correctivos) liberando la planilla (que se recupera del Excel) y, si aun así no cabe, muestra un aviso fijo para descargar respaldo de inmediato | Que nunca pierda mi trabajo en silencio aunque el navegador se quede sin espacio |
| 2026‑06‑16 | **Tolerancia a respaldos antiguos/editados**: al cargar, la app completa estructuras faltantes (tareas, gestiones, avances) para no caerse con datos parciales | Poder restaurar respaldos viejos o corregidos a mano sin que la aplicación falle |
| 2026‑06‑16 | **«Visita diagnóstica» como tipo de evento correctivo**: aparece en el desplegable del modal de Correctivo, **sin pedir tipo de compra**, con folio opcional que se autocompleta con el del expediente abierto del equipo | Quería anotar una visita diagnóstica y solo tenía OT/Reporte; el formulario me empujaba a una compra que no corresponde |
| 2026‑06‑16 | **Aclaración del concepto borrador/oficial** (secciones 2 y 5): el rojo de la carta dice «no es oficial»; el borrador de la app dice además **«y esto es lo que falta»** | Dejar registrado el porqué del borrador con detalle, que es el corazón del sistema |
| 2026‑06‑16 | **Datos de servicios externos en correctivo y MP**: envío con **responsable**; **Reporte de Servicio** = reporte del ingeniero externo (fecha, ingeniero, empresa, N° de reporte, reparación/diagnóstico); retorno con **N° de guía de despacho** y «¿viene el reporte?» (si no, pendiente automático); **MP externa** con ingeniero externo + empresa; **lista reutilizable de ingenieros** | Registrar tal como ocurre: envíos, reparaciones/diagnósticos externos y retornos con sus datos reales, sin que el formulario me empuje a una compra |
| 2026‑06‑16 | **Almacenamiento en IndexedDB** (principal) + localStorage (respaldo): el guardado deja de fallar cuando el navegador llena el localStorage de `file://`; migra solo lo que ya había. El aviso crítico solo aparece si fallan **ambos** | En uso real el navegador dejó de guardar mis cambios (almacenamiento lleno); ahora el trabajo se guarda con cuota amplia y no se pierde |
| 2026‑06‑16 | **Ingeniero externo como texto libre con autocompletado** (en correctivo y MP) | Tenía que elegir de una lista vacía; ahora escribo el nombre y queda memorizado para la próxima |
| 2026‑06‑16 | **Retorno sin reporte abre el pendiente** para completarlo de inmediato | Evita que arme a mano un pendiente duplicado para gestionar el reporte que faltó |

---

## 11. Pendiente de aclarar / próximos pasos

> Espacio para dudas abiertas y lo que falta entender antes de la versión final.

- *(sin pendientes abiertos por ahora — agregar a medida que surjan)*

---

### Cómo se mantiene este documento

- Es la **fuente de la verdad del proceso**. Ante cada ajuste, primero se actualiza aquí (qué y
  por qué) y luego se construye en la app.
- Cuando confirmemos que **todo está entendido y no hay más ajustes**, esta es la base para
  **congelar la aplicación oficial final**.
