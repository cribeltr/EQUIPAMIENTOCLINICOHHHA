# Sistema de Gestión MP 2026 · Equipamiento Clínico HHHA

Aplicación web (HTML + JavaScript, sin servidor) que implementa el **Flujo de Trabajo del Sistema de Gestión MP 2026** — Programa de Mantenciones Preventivas de Equipos.

## Cómo usar

**Opción A (un solo archivo):** abre `SistemaGestionMP2026.html` en cualquier navegador moderno (Chrome, Edge, Firefox). Es totalmente autónomo: incluye la librería de lectura de Excel incrustada y **funciona sin conexión a internet**.

**Opción B (carpeta del repositorio):** abre `index.html`, que carga la librería desde `js/xlsx.full.min.js`.

No requiere instalación ni servidor. Los datos quedan guardados localmente en el navegador (localStorage).

## Flujo implementado (especificación "Flujo_Sistema_Gestion_MP_2026")

| Paso | Función |
|------|---------|
| 1 | Carga del archivo **ProgramaciónMP2026** (hoja `PMP_2026`, encabezados fila 7, datos desde fila 8, columnas B–P). Se incluyen **todos** los registros (incluso con valor 0). `Serie` y `N° Inventario` se leen **como texto**, conservando ceros a la izquierda («00039» no se convierte en «39»), también en la vista y en la exportación. El ID es solo orden de fila: el identificador único es la Serie o el N° Inventario. |
| 2 | Vista de equipos con las mismas columnas y **filtros tipo Excel** por columna (selección múltiple, búsqueda y orden), búsqueda global, paginación y exportación a Excel. Cada fila abre el detalle del equipo. |
| 3 | Lectura de la programación (columnas T–AE, Ene–Dic) con códigos `X`, `R`, `RA`, `PM`, vinculada por Serie o N° Inventario. |
| 4 | Lectura de la hoja `Registro_MP-2026` (datos desde fila 8; cada mes con columna **P** y columna **R**: Enero T/U … Diciembre AP/AQ; columna AR = Observación). Se ignoran valores no válidos (ceros de relleno, números sueltos como «22» o «27»). **Regla Oficial/Borrador:** lo leído de planilla es Oficial; un Borrador de la app pasa a Oficial si la mantención aparece al recargar la planilla, y conserva Borrador si no aparece. |
| 5 | Interpretación de resultados: `Si`, `C1–C8`, `Si-RA`, `FS`, `No`, `NU`, `Baja` (con su significado visible en toda la app). |
| 6 | Reglas de reprogramación: causales C1–C8 documentadas; al registrar `C2/C3/C4` la app indica que no se fija nueva fecha; con `C1/C5/C6/C7/C8` indica el plazo de 30 días (con fecha límite calculada) y sugiere crear la gestión pendiente. |
| 7 | Vista de detalle del equipo con todos sus datos, programación/resultados por mes, historial y los tres botones **«Mantenimiento Preventivo»**, **«Pendientes»** y **«Mantenimiento Correctivo»**. |
| 8 | Formulario de Mantenimiento Preventivo: fecha, programación (X/R/RA/PM), ejecutor (lista oficial de 11), resultado, observaciones, estado del equipo (Operativo / No Operativo), gestión pendiente (Sí/No) y tipo de registro (Oficial / Borrador). |
| 9 | Formulario de Pendientes: fecha de compromiso con atajos (Hoy / 3 días / 1 semana), tipo de pendiente, descripción, lista de tareas, Responsable Administrativo (por defecto Cristián Beltrán Oviedo), Responsable Ejecutivo y bitácora de **gestión asociada**. Vista global de pendientes (abiertos / vencidos / completados). |
| 10 | Formulario de Mantenimiento Correctivo: el botón despliega la lista de **tipo de documento** — **Orden de Trabajo, Reporte de Servicio o Envío a Servicio Técnico** — y el formulario registra Requerimiento (opcional), Fecha del documento, **Folio de Solicitud de SIGEM**, Técnico asignado (misma lista de ejecutores), Estado del equipo (Operativo / No Operativo / **Servicio Técnico**), Gestión pendiente (Sí/No) y Tipo de registro (Oficial / Borrador). El estado más reciente (preventivo o correctivo) se refleja en la ficha del equipo. |
| 11 | Descarga de registros y respaldo (ver sección siguiente). |

Además incluye una pestaña **«Códigos y Reglas»** con las tablas de referencia de los pasos 3, 4, 5 y 6, y un botón **«Cargar datos de ejemplo»** para probar la aplicación sin la planilla real.

## Descargas y respaldo

En la pestaña **Carga de Datos** (sección «Descargas y respaldo», también accesible desde la vista de equipos con «⬇ Excel completo»):

- **Descargar todos los registros (Excel):** genera `Registros_GMP2026_<fecha>.xlsx` con 5 hojas — *Equipos* (columnas del Paso 1), *Programación* (códigos X/R/RA/PM de los 12 meses), *Mantenciones* (registros de la planilla y de la aplicación, con ejecutor, observaciones, tipo Oficial/Borrador y origen), *Pendientes* (con tareas y bitácora de gestión asociada) y *Correctivos* (documentos OT / Reporte de Servicio / Envío a Servicio Técnico, con folio SIGEM, técnico, estado, gestión pendiente y tipo de registro). Todas las celdas son de texto para conservar los ceros a la izquierda.
- **Descargar respaldo (.json):** genera `Respaldo_GMP2026_<fecha>.json` con absolutamente todo el estado de la aplicación (planilla cargada, mantenciones, pendientes y metadatos).
- **Restaurar respaldo:** carga un archivo de respaldo y reemplaza los datos actuales (pide confirmación y valida que el archivo sea un respaldo legítimo del sistema). Permite traspasar la información a otro computador o recuperarla si se limpió el navegador.

## Estructura del repositorio

```
index.html                 Aplicación (usa js/xlsx.full.min.js)
SistemaGestionMP2026.html  Versión autónoma en un solo archivo (recomendada para distribuir)
js/xlsx.full.min.js        Librería SheetJS 0.18.5 (lectura/escritura de .xlsx)
```

## Notas

- Los registros creados en la aplicación (mantenciones y pendientes) se conservan entre sesiones en el navegador y **sobreviven a las recargas de la planilla** (es ahí donde se aplica la regla Borrador→Oficial).
- «Borrar todos los datos» (pestaña Carga de Datos) elimina lo almacenado en ese navegador.
- La exportación genera celdas de texto para no perder los ceros a la izquierda al abrir en Excel.
