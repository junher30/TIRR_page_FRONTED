# Requerimientos no funcionales

El checklist fuente no contiene identificadores ni objetivos RNF explícitos. Para no inventar requisitos, esta lista registra temas que aparecen en RF y preguntas que deben convertirse en RNF verificables. No asignar identificadores definitivos hasta aprobación.

| Tema | Evidencia fuente | Definición necesaria |
|---|---|---|
| Seguridad | RF-036, RF-069, RF-072, RF-084, RF-085 | > PENDIENTE: amenazas, algoritmos/protocolos, gestión de secretos y criterios de verificación. |
| Autorización | RF-008, RF-087 | > PENDIENTE: matriz rol-recurso-acción y reglas de alcance por evento/equipo. |
| Integridad/atomicidad | RF-029, RF-073, RF-085 | > PENDIENTE: garantías transaccionales, idempotencia y recuperación ante concurrencia. |
| Disponibilidad/monitoreo | RF-070 | > PENDIENTE: SLO, ventanas de mantenimiento, alertas y objetivos de recuperación. |
| Respaldo/recuperación | RF-068 | > PENDIENTE: RPO, RTO, frecuencia, retención y evidencia de restauración. |
| Rendimiento | RF-050, RF-058 | > PENDIENTE: latencia objetivo, usuarios concurrentes, volumen y frescura de datos. |
| Accesibilidad | RF-081 | > PENDIENTE: estándar objetivo y pruebas de conformidad. |
| Compatibilidad/adaptabilidad | RF-034, RF-074 | > PENDIENTE: navegadores, dispositivos, resoluciones y condiciones de cámara. |
| Mantenibilidad | RF-071 | > PENDIENTE: políticas de migración, revisión, rollback y compatibilidad. |
| Privacidad | RF-069, RF-063 | > PENDIENTE: datos personales tratados, base legal, consentimiento, retención y derechos. |
| Escalabilidad | RF-011, RF-050 | > PENDIENTE: crecimiento esperado de eventos, equipos, conexiones y almacenamiento. |
| Usabilidad | RF-075, RF-082 | > PENDIENTE: tareas críticas, perfiles, métricas y pruebas con usuarios. |

Cada RNF aprobado deberá tener identificador `RNF-NNN`, condición, métrica/umbral, método de verificación, prioridad y trazabilidad.
