# Grabaciones de sesión — bitácora de hallazgos

> **Qué son.** El botón «🔴 Grabar» de la app registra **localmente** la interacción
> (clics, escritura, navegación, formularios, tiempos, errores). **Nada sale del computador**;
> al detener se descarga un `.json`. Aquí se archivan las grabaciones entregadas y, sobre todo,
> **para qué sirvieron**: qué fricción revelaron y qué ajuste produjeron. Es parte del
> entendimiento acumulativo (junto a `ENTENDIMIENTO.md`).

**Resumen:** 19 grabaciones archivadas · 8 rage-clicks y 0 errores en total
(señal de que la app se mantuvo estable). Las filas con «Qué reveló» detallado son las analizadas a fondo;
el resto fue uso general de exploración.

| Fecha | Archivo | Build | Dur (s) | Eventos | Vista | Rage | Err | Val. fallidas | Qué reveló / ajuste |
|------|---------|-------|--------:|--------:|-------|-----:|----:|---:|---------------------|
| 2026-06-12 18:34 | Grabacion_GMP2026_20260612_1457.json |  | 1347 | 188 |  | 0 | 0 | 0 | Uso general (exploración de vistas, pendientes, plan). |
| 2026-06-12 19:40 | Grabacion_GMP2026_20260612_1543.json |  | 170 | 62 |  | 0 | 0 | 0 | Uso general (exploración de vistas, pendientes, plan). |
| 2026-06-12 19:44 | Grabacion_GMP2026_20260612_1546.json |  | 140 | 59 |  | 0 | 0 | 0 | Uso general (exploración de vistas, pendientes, plan). |
| 2026-06-12 19:48 | Grabacion_GMP2026_20260612_1554.json |  | 368 | 104 |  | 0 | 0 | 0 | Uso general (exploración de vistas, pendientes, plan). |
| 2026-06-12 20:52 | Grabacion_GMP2026_20260612_1706.json | 2026-06-12.11 | 809 | 26 |  | 0 | 0 | 0 | Uso general (exploración de vistas, pendientes, plan). |
| 2026-06-12 21:59 | Grabacion_GMP2026_20260612_1811.json | 2026-06-12.13 | 675 | 103 |  | 0 | 0 | 0 | Uso general (exploración de vistas, pendientes, plan). |
| 2026-06-12 22:25 | Grabacion_GMP2026_20260612_1842.json | 2026-06-12.14 | 1005 | 160 |  | 0 | 0 | 0 | Uso general (exploración de vistas, pendientes, plan). |
| 2026-06-12 23:11 | Grabacion_GMP2026_20260612_1920.json | 2026-06-12.17 | 506 | 118 |  | 0 | 0 | 0 | Uso general (exploración de vistas, pendientes, plan). |
| 2026-06-15 12:30 | Grabacion_GMP2026_20260615_0835.json | 2026-06-13.19 | 309 | 90 |  | 0 | 0 | 0 | Uso general (exploración de vistas, pendientes, plan). |
| 2026-06-15 12:41 | Grabacion_GMP2026_20260615_0915.json | 2026-06-15.20 | 2054 | 531 |  | 0 | 0 | 0 | Uso general (exploración de vistas, pendientes, plan). |
| 2026-06-15 13:49 | Grabacion_GMP2026_20260615_1034.json | 2026-06-15.20 | 2724 | 263 |  | 0 | 0 | 0 | Uso general (exploración de vistas, pendientes, plan). |
| 2026-06-15 14:40 | Grabacion_GMP2026_20260615_1147.json | 2026-06-15.21 | 4061 | 319 |  | 0 | 0 | 0 | Uso general (exploración de vistas, pendientes, plan). |
| 2026-06-15 15:25 | Grabacion_GMP2026_20260615_1148.json | 2026-06-15.21 | 1324 | 129 |  | 0 | 0 | 0 | Uso general (exploración de vistas, pendientes, plan). |
| 2026-06-15 16:00 | Grabacion_GMP2026_20260615_1300.json | 2026-06-15.22 | 3623 | 707 |  | 0 | 0 | 0 | Uso general (exploración de vistas, pendientes, plan). |
| 2026-06-16 13:21 | Grabacion_GMP2026_20260616_0924.json | 2026-06-16.28 | 149 | 81 | detalle | 0 | 0 | 0 | Tipo de mantenimiento Externo + gestión pendiente. Confirmó el flujo MP interno/externo. |
| 2026-06-16 13:59 | Grabacion_GMP2026_20260616_1011.json | 2026-06-16.30 | 777 | 271 | detalle | 0 | 0 | 0 | Reprogramaciones con notas manuales («imprimir…») y fricción. → Disparó el ciclo de reporte de reprogramación y armarlo desde el tipo. |
| 2026-06-16 15:05 | Grabacion_GMP2026_20260616_1109.json | 2026-06-16.34 | 227 | 119 | pendientes | 5 | 0 | 0 | Carta Gantt: filtró abril por causales (reprogramadas) y por servicio. Reveló la necesidad de buscar envíos y de agrupar por servicio. |
| 2026-06-16 15:21 | Grabacion_GMP2026_20260616_1123.json | 2026-06-16.35 | 112 | 68 | plan | 0 | 0 | 0 | Gantt: filtró abril reprogramadas y exportó (10 equipos). Confirmó que el Gantt mezcla bien planilla (X) + app (C6). |
| 2026-06-16 17:05 | Grabacion_GMP2026_20260616_1308.json | 2026-06-16.38 | 197 | 53 | pendientes | 3 | 0 | 0 | Revisó la bitácora del equipo y trabajó un protocolo (Gestión + subtarea). Reportó el checklist por defecto al crear pendiente → se quitó. |

---

### Cómo se usa esta bitácora
- Cada vez que entregues una grabación nueva, se archiva aquí y se anota **qué mostró** y **qué se cambió**.
- Las columnas *Rage* (clics repetidos <0,8 s en lo mismo) y *Val. fallidas* (choques con validaciones)
  son las señales rápidas de fricción; *Err* debe ser 0.
- Sirve para no repetir análisis y para justificar cada ajuste con evidencia de uso real.
