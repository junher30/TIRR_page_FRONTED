# Modelo de datos

## Entidades conceptuales sugeridas por los requisitos

Los nombres siguientes son conceptos de dominio inferidos para organizar requisitos; no constituyen un esquema aprobado.

| Concepto | Requisitos relacionados | Preguntas de modelado |
|---|---|---|
| Usuario, rol y permiso | RF-001–RF-008 | > PENDIENTE: cardinalidad de roles, alcance y gestión de cuentas. |
| Coach, equipo e integrante | RF-006, RF-009, RF-010, RF-018–RF-020 | > PENDIENTE: identidad de competidor, duplicados y pertenencia histórica. |
| Campeonato, edición, categoría | RF-011–RF-013 | > PENDIENTE: ciclo de vida y relación entre evento y edición. |
| Sede, pista/mesa, jornada | RF-014, RF-052 | > PENDIENTE: disponibilidad, zonas horarias y conflictos. |
| Inscripción y requisitos | RF-015–RF-020 | > PENDIENTE: estados/transiciones y aprobación. |
| Tarifa, orden, pago, transacción | RF-021–RF-031, RF-083–RF-087, RF-090 | > PENDIENTE: moneda, proveedor, idempotencia, reembolso y conciliación. |
| Acreditación, credencial y acceso | RF-032–RF-039, RF-088–RF-089 | > PENDIENTE: credencial por participante/equipo y política de reingreso. |
| Reglamento y versión | RF-040, RF-057 | > PENDIENTE: publicación, vigencia y asociación. |
| Encuentro, llave, puntuación y resultado | RF-041–RF-048, RF-051–RF-054 | > PENDIENTE: estructuras por modalidad y revisiones. |
| Apelación y auditoría | RF-046–RF-047, RF-090 | > PENDIENTE: estados, permisos, retención e inmutabilidad. |
| Notificación y archivo | RF-067, RF-078 | > PENDIENTE: canales, retención y límites de almacenamiento. |

No hay diagrama ER, diccionario de datos, claves, restricciones, índices ni estrategia de migración detallada disponible.
