# Requerimientos funcionales

Fuente: checklist proporcionado por el usuario. Los requisitos se transcriben conservando texto e identificadores; su presencia no implica aprobación o implementación.

## 1. Usuarios, roles y permisos

- [ ] **RF-001 — Autenticación:** Registro, inicio de sesión, recuperación de contraseña y verificación de correo electrónico.
- [ ] **RF-002 — Superadministrador:** Administrar usuarios, roles, eventos, pagos, reglamentos, resultados y configuración global.
- [ ] **RF-003 — Administrador de entradas:** Escanear códigos QR, validar acreditaciones y registrar entradas sin poder aprobar pagos.
- [ ] **RF-004 — Administrador de eventos:** Crear y modificar campeonatos, categorías, cupos, equipos, fechas, horarios y sedes.
- [ ] **RF-005 — Jueces:** Consultar encuentros asignados, registrar puntuaciones, penalizaciones y resultados autorizados.
- [ ] **RF-006 — Capitán / Coach:** Único rol que puede registrar equipos, gestionar integrantes, inscribirlos y consultar pagos, horarios y clasificaciones.
- [ ] **RF-007 — Visitantes públicos:** Consultar eventos, reglamentos, resultados, clasificaciones y transmisiones sin iniciar sesión.
- [ ] **RF-008 — Control de permisos:** Restringir cada operación por rol, evento, categoría y equipos asignados.
- [ ] **RF-009 — Varios equipos por Coach:** Permitir que una cuenta gestione e inscriba múltiples equipos y categorías.
- [ ] **RF-010 — Competidores sin cuenta obligatoria:** Los participantes son registrados por su Capitán / Coach y pueden consultar información pública sin autenticarse.

## 2. Eventos y campeonatos

- [ ] **RF-011 — Múltiples campeonatos:** Administrar competencias, ediciones y eventos simultáneos desde una sola plataforma.
- [ ] **RF-012 — Categorías:** Crear sumo, minisumo, seguidor de línea, soccer, brush race y otras modalidades.
- [ ] **RF-013 — Configuración de categorías:** Definir edad, integrantes permitidos, cupos, precios y requisitos de participación.
- [ ] **RF-014 — Sedes y horarios:** Administrar ubicaciones, pistas, mesas, jornadas y rondas.
- [ ] **RF-015 — Estados de inscripción:** Abrir, cerrar, suspender o ampliar las inscripciones y modificar fechas límite.
- [ ] **RF-016 — Administración de equipos:** Aprobar, rechazar, retirar o descalificar equipos, registrando cada cambio.
- [ ] **RF-017 — Agenda:** Publicar los horarios de enfrentamientos y comunicar modificaciones.
- [ ] **RF-018 — Responsables por equipo:** Relacionar cada equipo con un Capitán / Coach responsable.

## 3. Inscripciones y pagos

- [ ] **RF-019 — Inscripción por Capitán / Coach:** Solo una cuenta autenticada con este rol puede inscribir equipos en las competencias.
- [ ] **RF-020 — Formulario de inscripción:** Registrar nombre del equipo, integrantes, institución, país, categoría y contacto.
- [ ] **RF-021 — Tarifas configurables:** Establecer precios por campeonato y categoría, expresados en pesos colombianos para PSE.
- [ ] **RF-022 — Pagos colombianos por PSE:** Permitir pagos digitales de equipos elegibles de Colombia mediante una pasarela integrada.
- [ ] **RF-023 — Pagos extranjeros presenciales:** Registrar las inscripciones extranjeras como pendientes de pago físico hasta su confirmación.
- [ ] **RF-024 — Confirmación mediante webhook:** Verificar criptográficamente las notificaciones del proveedor y confirmar transacciones válidas.
- [ ] **RF-025 — Estados de pago:** Gestionar pendiente, en proceso, aprobado, rechazado, reembolsado y en revisión.
- [ ] **RF-026 — Órdenes con varios equipos:** Permitir pagar varios equipos colombianos mediante una misma orden.
- [ ] **RF-027 — Cálculo automático:** Calcular precios en el servidor con base en las categorías y equipos seleccionados.
- [ ] **RF-028 — Comprobantes:** Generar comprobantes de inscripción, confirmaciones y documentos fiscales cuando corresponda.
- [ ] **RF-029 — Prevención de duplicados:** Evitar pagos duplicados, repetición de inscripciones y procesamiento múltiple de webhooks.
- [ ] **RF-030 — Registro administrativo presencial:** Permitir que personal autorizado registre pagos extranjeros, importes y soportes.
- [ ] **RF-031 — Historial de transacciones:** Almacenar referencias, identificadores de pago, fechas, métodos y responsables.

## 4. Códigos QR y control de entradas

- [ ] **RF-032 — Emisión condicionada de QR:** Generar QR únicamente después de confirmar el pago y aprobar la inscripción, cuando aplique.
- [ ] **RF-033 — Credenciales únicas:** Crear una credencial por participante o equipo según la política del evento.
- [ ] **RF-034 — Escáner web:** Validar códigos QR utilizando la cámara de un dispositivo autorizado.
- [ ] **RF-035 — Estados de acreditación:** Distinguir acreditación válida, utilizada, revocada, pendiente o inválida.
- [ ] **RF-036 — Protección antifraude:** Emplear tokens aleatorios, hashes seguros y validación del lado del servidor.
- [ ] **RF-037 — Registro de accesos:** Guardar fecha, hora, lugar y administrador que validó cada credencial.
- [ ] **RF-038 — Entrega al Coach:** Permitir que el Capitán / Coach consulte y descargue los QR de sus equipos acreditados.
- [ ] **RF-039 — Restricción de accesos:** No habilitar QR válidos para inscripciones pendientes, pagos rechazados o acreditaciones revocadas.

## 5. Reglamentos, llaves y sistema competitivo

- [ ] **RF-040 — Reglamentos oficiales:** Subir documentos PDF, versionarlos y asociarlos a categorías y campeonatos.
- [ ] **RF-041 — Modalidades competitivas:** Soportar eliminación directa, doble eliminación, grupos y todos contra todos.
- [ ] **RF-042 — Generación de llaves:** Crear llaves automáticas o manuales con equipos, posiciones y cruces.
- [ ] **RF-043 — Siembras y sorteos:** Configurar cabezas de serie y asignación de posiciones.
- [ ] **RF-044 — Puntuación configurable:** Definir criterios, penalizaciones, desempates, tiempos y número de rondas.
- [ ] **RF-045 — Clasificación automática:** Actualizar tablas, posiciones y avances de los ganadores.
- [ ] **RF-046 — Auditoría de resultados:** Registrar modificaciones, autores, fechas y motivos de corrección.
- [ ] **RF-047 — Apelaciones:** Gestionar reclamaciones, disputas y aprobación final de resultados.
- [ ] **RF-048 — Reglas por categoría:** Permitir distintos sistemas de evaluación para minisumo, seguidores de línea y otras disciplinas.

## 6. Resultados públicos en vivo

- [ ] **RF-049 — Portal público:** Publicar eventos, equipos, categorías, reglamentos y clasificaciones.
- [ ] **RF-050 — Marcadores en tiempo real:** Actualizar resultados sin necesidad de recargar la página.
- [ ] **RF-051 — Llaves interactivas:** Mostrar rondas, cruces, equipos clasificados y próximos encuentros.
- [ ] **RF-052 — Programación competitiva:** Publicar pista, hora, orden de participación y rivales.
- [ ] **RF-053 — Pantallas de exhibición:** Ofrecer vistas especiales para proyectores y pantallas grandes.
- [ ] **RF-054 — Historial:** Mostrar resultados anteriores, podios, ganadores y estadísticas.
- [ ] **RF-055 — Transmisiones:** Integrar videos o emisiones en vivo desde plataformas externas.

## 7. Asistente de inteligencia artificial

- [ ] **RF-056 — Asistente público:** Responder consultas sobre campeonatos, inscripciones, categorías y horarios.
- [ ] **RF-057 — Consultas de reglamentos:** Responder con base en documentación oficial, citando reglas y secciones.
- [ ] **RF-058 — Datos actualizados:** Consultar información publicada de los eventos en la base de datos.
- [ ] **RF-059 — Soporte multilingüe:** Atender inicialmente en español e inglés.
- [ ] **RF-060 — Control de respuestas:** Evitar presentar información no verificada como una norma oficial.
- [ ] **RF-061 — Escalamiento:** Derivar reclamaciones y consultas administrativas a personal autorizado.
- [ ] **RF-062 — Control de consumo:** Limitar solicitudes abusivas y gestionar los costos de los modelos de IA.
- [ ] **RF-063 — Preguntas sobre pagos:** Explicar que los equipos colombianos pagan por PSE y los extranjeros presencialmente, sin acceder a información privada.

## 8. Base de datos e infraestructura

- [ ] **RF-064 — PostgreSQL:** Almacenar usuarios, equipos, campeonatos, inscripciones, pagos, QR y resultados.
- [ ] **RF-065 — Desarrollo local:** Ejecutar todos los servicios principales en un computador utilizando Docker Compose.
- [ ] **RF-066 — Despliegue propio:** Instalar la aplicación y PostgreSQL en un servidor o VPS compatible.
- [ ] **RF-067 — Archivos locales:** Almacenar documentos, imágenes y reglamentos en un volumen persistente del servidor.
- [ ] **RF-068 — Respaldos:** Programar copias de seguridad y probar su recuperación.
- [ ] **RF-069 — Seguridad:** Implementar HTTPS, contraseñas seguras, controles de autorización y protección de datos.
- [ ] **RF-070 — Monitoreo:** Registrar errores, disponibilidad, eventos críticos y funcionamiento del servidor.
- [ ] **RF-071 — Migraciones:** Gestionar cambios de esquema mediante Prisma sin perder información.
- [ ] **RF-072 — Integración de pagos:** Proteger credenciales API, secretos de webhooks y datos de transacciones.
- [ ] **RF-073 — Atomicidad:** Evitar acreditaciones parciales y duplicadas cuando se procesen pagos concurrentes.

## 9. Diseño, administración y experiencia de uso

- [ ] **RF-074 — Diseño adaptable:** Crear vistas para celulares, tabletas, computadores y pantallas públicas.
- [ ] **RF-075 — Paneles por rol:** Personalizar menús y herramientas según los permisos del usuario.
- [ ] **RF-076 — Identidad visual:** Gestionar logotipos, patrocinadores, colores e imagen de eventos.
- [ ] **RF-077 — Búsqueda:** Filtrar equipos, categorías, competidores, eventos y resultados.
- [ ] **RF-078 — Notificaciones:** Enviar confirmaciones de inscripción, pagos, acreditaciones y cambios de horarios.
- [ ] **RF-079 — Exportaciones:** Generar informes en Excel, CSV y PDF.
- [ ] **RF-080 — Estadísticas:** Consultar participantes, países, ingresos, cupos y estado de competencias.
- [ ] **RF-081 — Accesibilidad:** Permitir navegación por teclado, contraste adecuado y lectura en móviles.
- [ ] **RF-082 — Panel del Coach:** Mostrar equipos administrados, pagos pendientes, acreditaciones, programación y resultados.

## 10. Gestión operativa de pagos y acreditaciones

- [ ] **RF-083 — Selección del método:** Asignar el flujo PSE o presencial según la elegibilidad y el país del equipo.
- [ ] **RF-084 — Checkout seguro:** Dirigir al Coach colombiano a un checkout autorizado sin almacenar sus datos de tarjeta o banca.
- [ ] **RF-085 — Verificación del proveedor:** Contrastar referencia, importe, moneda y estado antes de confirmar una orden.
- [ ] **RF-086 — Confirmación presencial:** Permitir que personal con permiso de cobros confirme pagos de equipos extranjeros.
- [ ] **RF-087 — Separación de responsabilidades:** Impedir que el rol de administrador de entradas apruebe pagos por defecto.
- [ ] **RF-088 — Acreditación automática:** Emitir credenciales después de una confirmación válida de pago y de cumplir los requisitos del evento.
- [ ] **RF-089 — Reembolsos y anulaciones:** Gestionar la revocación de acreditaciones según la política de cancelaciones.
- [ ] **RF-090 — Auditoría financiera:** Registrar quién confirmó un pago presencial y los eventos relevantes de pagos digitales.

## Observaciones de consistencia

- RF-022–RF-031 y RF-083–RF-090 se solapan en pagos; aclarar si la sección 10 define reglas operativas complementarias o reemplaza parte de la sección 3.
- RF-032 y RF-088 condicionan la acreditación a pago y requisitos; RF-032 también menciona aprobación de inscripción “cuando aplique”. Definir una única regla de emisión y sus excepciones.
- RF-033 deja pendiente la granularidad de credencial (por participante o equipo), delegándola a la política del evento.
- RF-028 deja sin especificar la jurisdicción y condiciones fiscales.
