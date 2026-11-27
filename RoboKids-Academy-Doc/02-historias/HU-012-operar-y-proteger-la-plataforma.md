# HU-012 — Operar y proteger la plataforma

**Estado:** Borrador derivado de RF; pendiente de validación técnica.  
**Actor:** Administrador técnico/operador.  
**Requisitos:** RF-064–RF-073.

## Historia

Como operador técnico quiero desplegar, respaldar, actualizar y monitorear la plataforma para conservar los datos y detectar fallos operativos.

## Criterios de aceptación derivados

1. PostgreSQL almacena usuarios, equipos, campeonatos, inscripciones, pagos, QR y resultados.
2. Los servicios principales pueden ejecutarse localmente con Docker Compose.
3. La aplicación y PostgreSQL pueden instalarse en servidor o VPS compatible.
4. Los archivos se guardan en volumen persistente.
5. Se programan respaldos y se prueba su recuperación.
6. Se aplican HTTPS, contraseñas seguras, autorización y protección de datos.
7. Se registran errores, disponibilidad, eventos críticos y funcionamiento del servidor.
8. Los cambios de esquema se gestionan con Prisma sin perder información.
9. Las credenciales API, secretos de webhook y datos de transacción se protegen.
10. El procesamiento concurrente evita acreditaciones parciales o duplicadas.

## Pendiente

> PENDIENTE: Stack de aplicación, controles concretos, estrategia de secretos, RPO/RTO, retención de logs y procedimiento de despliegue/rollback.
