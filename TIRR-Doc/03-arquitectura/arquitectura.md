# Arquitectura de software

## Estado de la arquitectura

No se proporcionó una arquitectura aprobada ni código fuente para inspección. Este documento registra restricciones y tecnologías mencionadas por el checklist, sin convertirlas en decisiones adoptadas.

## Tecnologías mencionadas por la fuente

- PostgreSQL como base de datos (RF-064).
- Docker Compose para desarrollo local (RF-065).
- Despliegue de aplicación y PostgreSQL en servidor/VPS propio (RF-066).
- Volumen persistente local para archivos (RF-067).
- Prisma para migraciones (RF-071).

## Capacidades/integraciones requeridas

- Pasarela colombiana con PSE y notificaciones webhook verificables (RF-022, RF-024, RF-084–RF-085).
- Cámara web para lectura de QR (RF-034).
- Correo para verificación de cuenta y notificaciones (RF-001, RF-078).
- Plataforma externa de transmisión (RF-055).
- Modelo/servicio de IA (RF-056–RF-063).

## Contexto funcional derivado

Los requisitos sugieren actores de administración, Coaches, jueces y público. Los flujos principales atraviesan identidad y autorización; eventos/equipos; inscripción/pago; acreditación; competencia/resultados; publicación. La forma de despliegue, los límites de componentes y el protocolo de comunicación no están especificados.

## Principios/restricciones explícitos

- El servidor calcula importes (RF-027).
- La confirmación de pagos digitales se basa en notificaciones verificadas y contraste con datos del proveedor (RF-024, RF-085).
- El personal de entradas no aprueba pagos por defecto (RF-003, RF-087).
- El procesamiento debe evitar duplicados y estados parciales (RF-029, RF-073).

> PENDIENTE: Definir diagrama de contexto/contenedores, límites de confianza, tecnologías de aplicación, API, autenticación, despliegue, disponibilidad, observabilidad y decisión de almacenamiento.
