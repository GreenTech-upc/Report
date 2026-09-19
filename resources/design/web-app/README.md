# SkyCrop Web App — entrega incremental

**Estado: bloque 1 parcial.** Se crearon fundamentos en Figma; la cuota MCP del plan Starter impidió generar la captura de revisión y continuar con los componentes. Este avance no constituye la entrega de pantallas ni un prototipo navegable.

- [Archivo del equipo](https://www.figma.com/design/1nlenowk3dSY0qdNiG6hYD/Diseno-UX-UI---SkyCrop)
- [Página nueva: Web App — Foundations](https://www.figma.com/design/1nlenowk3dSY0qdNiG6hYD/Diseno-UX-UI---SkyCrop?node-id=45-2)
- [Tablero de fundamentos](https://www.figma.com/design/1nlenowk3dSY0qdNiG6hYD/Diseno-UX-UI---SkyCrop?node-id=45-3)

## Qué se creó

| Elemento | Resultado |
|---|---|
| Colecciones | `SkyCrop Web / Primitives` y `SkyCrop Web / Semantic` |
| Variables | 35 primitivas y 52 semánticas; estas últimas referencian las primitivas |
| Tipografía | Roboto: Display, H1, H2, H3, Body, Body/Small, Label y Caption |
| Elevación | Estilos `Elevation/Card` y `Elevation/Dialog` |
| Tablero | Paleta, muestras tipográficas, espaciado, radios y reglas de accesibilidad |
| Páginas | Una página nueva, `Web App — Foundations` |

La llamada de creación del tablero informó dimensiones de 1440 × 1840 px. La revisión visual y la exportación de la captura están pendientes; no se afirma que el tablero haya pasado esa revisión.

## Decisiones visuales

| Color | Uso |
|---|---|
| `#A4D65E` | Acento lima; usar texto oscuro sobre este fondo |
| `#66BB6A` | Verde de apoyo; usar texto oscuro sobre este fondo |
| `#2E7D32` | Acción principal y éxito |
| `#F4F7F5` | Fondo de la aplicación |
| `#17221C` | Texto principal |
| `#607D8B` | Bordes de controles y acentos; no texto pequeño sobre fondo claro |
| `#1976A8` | Información, enlaces y foco |
| `#0B3954` | Superficies oscuras y navegación |

Se añadieron neutros para superficies, bordes y texto secundario; tintes para estados; verde oscuro para hover/pressed; rojo `#B3261E` y ámbar `#805600` exclusivamente para errores y advertencias. Los estados deberán tener texto e iconos, además del color.

La escala tipográfica usa tamaños de 48, 32, 24, 20, 16, 14 y 12 px. Se establecen controles táctiles de al menos 48 px y campos de 56 px, espaciado con base de 4 px y radios de 8 px para campos, 16 px para tarjetas y 24 px para diálogos. El inglés será el idioma predeterminado y se incluirá español latinoamericano.

La referencia existente del equipo usa Inter en wireframes. Se conserva sin cambios. Roboto se aplica únicamente a los fundamentos nuevos, conforme al plan aprobado y a las guías encontradas en `origin/feature/style-guidelines`.

## Protección y organización del archivo

Las páginas `0:1` (Landing Page) y `5:2` (Web Applications), incluidos sus avances de login, suscripciones y marcos de pantallas, se inspeccionaron en modo lectura. Ninguna escritura se dirigió a sus nodos ni a sus componentes. Las variables y estilos nuevos tienen el prefijo `SkyCrop Web`.

El plan Starter permite tres páginas. El intento de crear las tres páginas adicionales no persistió; después se creó únicamente Foundations en una llamada independiente. La alternativa propuesta es separar Foundations, Wireframes y Mockups & Prototype en secciones dentro de la nueva página. La preferencia del usuario sigue pendiente al registrar este avance.

`figma-state.json` registra los identificadores propios y las huellas previas del contenido existente. La comparación posterior quedó pendiente al agotarse la cuota. Para reanudar, inspeccionar primero el estado real del archivo; no borrar ni restaurar contenido del equipo si sus huellas cambiaron, pues puede haber edición simultánea.

## Validación realizada y pendiente

- La inspección en Figma confirmó 35 variables primitivas, 52 semánticas y ocho estilos tipográficos.
- No se detectaron alias rotos, variables sin sintaxis WEB ni variables con `ALL_SCOPES`.
- `contrast-check.json` registra verificaciones locales de combinaciones de color; no sustituye una auditoría del prototipo completo.
- Pendiente: captura, revisión visual, comparación final del contenido protegido y verificación de instancias de componentes.
- La consulta de metadatos devolvió una lista de páginas desactualizada respecto del editor; al retomar se debe contrastar con la lectura directa de `figma.root.children`.

## Próximos bloques

| Bloque | Pendiente | Commit sugerido |
|---|---|---|
| 1 — cierre | Revisar tablero; crear Button, Text field, Checkbox, Status badge, Navigation item, Alert y Dialog con variantes y propiedades editables | `design(web-app): add reusable SkyCrop components` |
| 2 | Login e inicio por rol, desktop/móvil, EN/ES | `design(web-app): add access and home screens` |
| 3 | Parcelas, formulario, invitación pendiente y colaborador incorporado | `design(web-app): add plots and collaboration flows` |
| 4 | Vinculación, configuración, confirmación y estados del vuelo | `design(web-app): add drone and flight screens` |
| 5 | Historial de reportes, dashboard y diagnósticos | `design(web-app): add reports and diagnoses` |
| 6 | Seis wireflows y user flows en FigJam; prototipos, capturas y documentación 4.4–4.5 | `docs(web-app): document flows and prototypes` |

Al cerrar cada bloque se debe informar al usuario y dejar los archivos listos para su commit antes de comenzar el siguiente. No se han hecho commits ni push. El video explicativo y su publicación en Microsoft Stream corresponden a una actividad posterior del equipo; no hay evidencia de video todavía.

## Archivos de este avance

- `design-tokens.json`: valores, alias, tipografía y elevaciones para el diseño; no implementa un frontend.
- `figma-state.json`: registro de IDs, páginas protegidas, validación y pendientes.
- `contrast-check.json`: cálculo local de contraste para las combinaciones previstas.

Commit sugerido para este avance parcial: `design(web-app): add SkyCrop visual foundations`.
