# HU-007 — Emitir y validar acreditaciones

**Estado:** Borrador derivado de RF; pendiente de validación.  
**Actor:** Coach y administrador de entradas.  
**Requisitos:** RF-032–RF-039, RF-088–RF-089.

## Historia

Como Coach quiero consultar y descargar las credenciales de mis equipos acreditados; como administrador de entradas quiero validar QR y registrar cada acceso.

## Criterios de aceptación derivados

1. Se emiten credenciales solo tras confirmación válida de pago y cumplimiento de los requisitos de acreditación aplicables.
2. La credencial tiene token aleatorio y se valida en el servidor.
3. La credencial indica estado válido, utilizado, revocado, pendiente o inválido.
4. El escáner web usa la cámara de un dispositivo autorizado para validar QR.
5. Cada acceso registra fecha, hora, lugar y administrador que validó.
6. El Coach puede consultar y descargar QR de sus equipos acreditados.
7. Inscripciones pendientes, pagos rechazados o acreditaciones revocadas no producen QR válidos.
8. Reembolsos y anulaciones gestionan revocación de acreditaciones conforme a la política definida.

## Pendiente

> PENDIENTE: Credencial por participante/equipo, reingreso, modo sin conexión, rotación de tokens y política de cancelación.
