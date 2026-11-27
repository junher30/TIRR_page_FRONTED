# HU-006 — Pagar y conciliar inscripciones

**Estado:** Borrador derivado de RF; pendiente de validación.  
**Actor:** Coach y personal autorizado de cobros.  
**Requisitos:** RF-021–RF-031, RF-083–RF-087, RF-090.

## Historia

Como Coach, quiero pagar las inscripciones mediante el método permitido para el equipo; como personal autorizado, quiero registrar y verificar pagos para mantener el estado financiero correcto.

## Criterios de aceptación derivados

1. La tarifa se configura por campeonato/categoría y el importe se calcula en el servidor.
2. Equipos colombianos elegibles pueden iniciar pago PSE en checkout autorizado; equipos extranjeros quedan pendientes de pago presencial.
3. Una orden puede cubrir varios equipos colombianos.
4. El sistema gestiona los estados pendiente, en proceso, aprobado, rechazado, reembolsado y en revisión.
5. La confirmación digital verifica webhook y contrasta referencia, importe, moneda y estado con el proveedor.
6. Personal autorizado puede registrar pagos presenciales, importe y soporte; el registro guarda quién confirmó el pago.
7. El sistema previene procesamiento duplicado, conserva historial de transacciones y genera comprobantes requeridos.
8. El administrador de entradas no puede aprobar pagos por defecto.

## Pendiente

> PENDIENTE: Proveedor, monedas y excepciones de elegibilidad; reglas de conciliación, tiempos de expiración, reembolsos, documentos fiscales y manejo de discrepancias.
