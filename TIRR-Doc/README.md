# TIRR — Documentación del sitio

Documentación funcional y técnica del sitio web TIRR y de las capacidades descritas en su checklist. Esta carpeta organiza la visión, los requisitos, las historias, la arquitectura y los diagramas del proyecto.

## Índice

- [Visión](00-vision/)
- [Requerimientos funcionales y no funcionales](01-requerimientos/)
- [Historias de usuario](02-historias/)
- [Arquitectura y modelo de datos](03-arquitectura/)
- [Diagramas](04-diagramas/)
- [Registro de cambios](CHANGELOG.md)

## Estado de la documentación

La fuente inicial es un checklist de 90 requisitos funcionales, RF-001 a RF-090. Los elementos técnicos que el checklist menciona —PostgreSQL, Docker Compose, Prisma, almacenamiento local y despliegue en VPS— son requisitos o tecnologías contempladas; no hay evidencia aportada de que estén aprobadas o implementadas.

Las decisiones aún no especificadas se marcan con `> PENDIENTE:`. Las propuestas se etiquetan como tales y no deben interpretarse como decisiones aprobadas. La existencia de un requisito no demuestra que la función esté construida o probada.

Las historias HU-001 a HU-015 son borradores derivados del checklist y esperan validación de los actores del proyecto.

## Convenciones

- Conservar los identificadores existentes `RF-NNN`.
- Usar `RNF-NNN`, `HU-NNN` y `ADR-NNN` para nuevos elementos, sin reutilizar identificadores.
- Registrar fuente, prioridad/estado y trazabilidad al actualizar requisitos.
- Mantener diagramas fuente editables junto con sus exportaciones; anotar herramienta y fecha de exportación.

## Pendientes generales

> PENDIENTE: Aprobar alcance, arquitectura, pasarela de pago, políticas operativas y rúbrica documental.
> PENDIENTE: Definir RNF medibles, historias de usuario, criterios de aceptación y casos de prueba.
