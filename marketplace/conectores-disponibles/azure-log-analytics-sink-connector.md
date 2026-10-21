# Azure Log Analytics Sink Connector

|  |  |
| --- | --- |
|  | **Conector para enviar desde GlobalSuite logs, métricas, eventos y señales operativas hacia Azure Log Analytics o hacia el sistema destino definido.**  **Etiquetas:** Analítica y monitorización | Cloud | Sink | Logs |

|  |  |
| --- | --- |
| Herramienta o sistema | Azure Log Analytics |
| Fabricante de la herramienta | Microsoft |
| Proveedor del conector | Confluent, Inc |
| Nombre del conector | Azure Log Analytics Sink Connector |
| Tipo de conector | Sink |
| Etiquetas | Analítica y monitorización | Cloud | Sink | Logs |
| Información que maneja | logs, métricas, eventos y señales operativas |

## Detalles

El conector Azure Log Analytics Sink Connector permite enviar desde GlobalSuite hacia Azure Log Analytics información relacionada con logs, métricas, eventos y señales operativas.

Es útil cuando Azure Log Analytics debe actuar como sistema de destino, explotación, archivo o monitorización para casos de centralización de evidencias, análisis de incidentes, cuadros de mando operativos y alertas de cumplimiento.

## Características

* Envío controlado de logs, métricas, eventos y señales operativas desde GlobalSuite hacia Azure Log Analytics o hacia el repositorio destino definido.
* Clasificación de eventos por origen, criticidad, servicio o responsable para acelerar la interpretación.
* Soporte a monitorización continua de señales relevantes para seguridad, cumplimiento u operación.
* Conservación de evidencias operativas que pueden asociarse a incidencias, controles o auditorías.
* Capacidad de alimentar cuadros de mando o procesos de alerta con datos actualizados.

## Beneficios clave

* Aumenta la visibilidad sobre eventos relevantes para seguridad, continuidad, cumplimiento y operación.
* Acelera el análisis de incidencias al centralizar señales y evidencias en un flujo gobernado.
* Facilita alimentar cuadros de mando, alertas y procesos de escalado con información fiable.
* Reduce búsquedas manuales de logs o métricas durante auditorías y revisiones post-incidente.
* Permite relacionar eventos técnicos con riesgos, controles, servicios o responsables de negocio.

## Instalación

|  |
| --- |
| **Nota de configuración:** Antes de activar la integración, valida credenciales, permisos, alcance funcional y una prueba de datos con el área responsable. |

1. Accede al Marketplace de GlobalSuite® y selecciona Azure Log Analytics Sink Connector.
2. Configura el destino en Azure Log Analytics: URL o endpoint, credenciales, permisos y entorno.
3. Define qué información se enviará: logs, métricas, eventos y señales operativas, filtros, formato y periodicidad.
4. Mapea los campos de GlobalSuite con la estructura esperada por el sistema destino.
5. Ejecuta una prueba, revisa la recepción en destino y activa la integración.

## Más información

<https://learn.microsoft.com/azure/azure-monitor/logs/>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando necesites enviar información de GlobalSuite a Azure Log Analytics, por ejemplo para centralización de evidencias, análisis de incidentes, cuadros de mando operativos y alertas de cumplimiento. Antes de publicarlo, valida con el equipo propietario del sistema destino el formato esperado, permisos, frecuencia y criterios de calidad.
