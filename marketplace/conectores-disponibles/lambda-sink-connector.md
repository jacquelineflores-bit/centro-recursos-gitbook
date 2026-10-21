# Lambda Sink Connector

|  |  |
| --- | --- |
|  | **Conector para enviar desde GlobalSuite tickets, tareas, objetos de negocio y estados de proceso hacia Lambda o hacia el sistema destino definido.**  **Etiquetas:** Integración | Sink | APIs | Cloud |

|  |  |
| --- | --- |
| Herramienta o sistema | Lambda |
| Fabricante de la herramienta | Amazon Web Services |
| Proveedor del conector | Confluent Cloud |
| Nombre del conector | Lambda Sink Connector |
| Tipo de conector | Sink |
| Etiquetas | Integración | Sink | APIs | Cloud |
| Información que maneja | tickets, tareas, objetos de negocio y estados de proceso |

## Detalles

El conector Lambda Sink Connector permite enviar desde GlobalSuite hacia Lambda información relacionada con tickets, tareas, objetos de negocio y estados de proceso.

Es útil cuando Lambda debe actuar como sistema de destino, explotación, archivo o monitorización para casos de seguimiento de tareas, gestión de incidencias, automatización de aprobaciones y trazabilidad entre equipos.

## Características

* Envío controlado de tickets, tareas, objetos de negocio y estados de proceso desde GlobalSuite hacia Lambda o hacia el repositorio destino definido.
* Mapeo de proyectos, estados, objetos de negocio, tickets o tareas con procesos gestionados en GlobalSuite.
* Uso de filtros por responsable, estado, tipo, prioridad o periodo para sincronizar sólo datos relevantes.
* Soporte a flujos de seguimiento, aprobación, remediación o comunicación entre equipos.
* Trazabilidad funcional entre la acción operativa y el riesgo, control, evidencia o plan asociado.

## Beneficios clave

* Conecta el trabajo operativo de los equipos con riesgos, controles, planes de acción o evidencias en GlobalSuite.
* Reduce seguimientos manuales por correo al sincronizar estados, responsables y prioridades.
* Facilita auditoría de acciones realizadas en herramientas de ticketing, CRM, ITSM o colaboración.
* Permite medir avances y cuellos de botella en remediaciones, aprobaciones o tareas recurrentes.
* Mejora la coordinación entre negocio, tecnología, cumplimiento y proveedores.

## Instalación

|  |
| --- |
| **Nota de configuración:** Antes de activar la integración, valida credenciales, permisos, alcance funcional y una prueba de datos con el área responsable. |

1. Accede al Marketplace de GlobalSuite® y selecciona Lambda Sink Connector.
2. Configura el destino en Lambda: URL o endpoint, credenciales, permisos y entorno.
3. Define qué información se enviará: tickets, tareas, objetos de negocio y estados de proceso, filtros, formato y periodicidad.
4. Mapea los campos de GlobalSuite con la estructura esperada por el sistema destino.
5. Ejecuta una prueba, revisa la recepción en destino y activa la integración.

## Más información

<https://aws.amazon.com/lambda/>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando necesites enviar información de GlobalSuite a Lambda, por ejemplo para seguimiento de tareas, gestión de incidencias, automatización de aprobaciones y trazabilidad entre equipos. Antes de publicarlo, valida con el equipo propietario del sistema destino el formato esperado, permisos, frecuencia y criterios de calidad.
