# Google BigQuery Sink Connector (Legacy)

|  |  |
| --- | --- |
|  | **A sink connector for writing to Google BigQuery, with support for automatic table creation and schema evolution.**  **Etiquetas:** Data Warehouse | Cloud | Sink |

|  |  |
| --- | --- |
| Herramienta o sistema | Google BigQuery ( ) |
| Fabricante de la herramienta | Google Cloud |
| Proveedor del conector | WePay |
| Nombre del conector | Google BigQuery Sink Connector (Legacy) |
| Tipo de conector | Sink |
| Etiquetas | Data Warehouse | Cloud | Sink |
| Información que maneja | datasets, tablas y datos analíticos |

## Detalles

El conector Google BigQuery Sink Connector (Legacy) permite enviar desde GlobalSuite hacia Google BigQuery ( ) información relacionada con datasets, tablas y datos analíticos.

Es útil cuando Google BigQuery ( ) debe actuar como sistema de destino, explotación, archivo o monitorización para casos de reporting ejecutivo, cuadros de mando de riesgo, consolidación de datos y analítica histórica.

## Características

* Envío controlado de datasets, tablas y datos analíticos desde GlobalSuite hacia Google BigQuery ( ) o hacia el repositorio destino definido.
* Preparación de datasets para reporting, cuadros de mando, análisis histórico o inteligencia de negocio.
* Mapeo de tablas, esquemas, campos o particiones según el modelo analítico acordado.
* Soporte a cargas incrementales o periódicas para mantener datos de explotación actualizados.
* Separación entre información operativa y capa analítica para facilitar gobierno y rendimiento.

## Beneficios clave

* Permite explotar datos de GlobalSuite y sistemas relacionados en herramientas de BI y analítica.
* Acelera la creación de cuadros de mando ejecutivos sobre riesgos, cumplimiento, auditoría o operación.
* Reduce la dependencia de extracciones manuales para reporting recurrente.
* Facilita análisis histórico, comparativas y seguimiento de tendencias.
* Ayuda a separar la gestión operativa diaria de la capa analítica usada por dirección y reporting.

## Instalación

|  |
| --- |
| **Nota de configuración:** Antes de activar la integración, valida credenciales, permisos, alcance funcional y una prueba de datos con el área responsable. |

1. Accede al Marketplace de GlobalSuite® y selecciona Google BigQuery Sink Connector (Legacy).
2. Configura el destino en Google BigQuery ( ): URL o endpoint, credenciales, permisos y entorno.
3. Define qué información se enviará: datasets, tablas y datos analíticos, filtros, formato y periodicidad.
4. Mapea los campos de GlobalSuite con la estructura esperada por el sistema destino.
5. Ejecuta una prueba, revisa la recepción en destino y activa la integración.

## Más información

<https://docs.confluent.io/cloud/current/connectors/cc-gcp-bigquery-sink.html>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando necesites enviar información de GlobalSuite a Google BigQuery ( ), por ejemplo para reporting ejecutivo, cuadros de mando de riesgo, consolidación de datos y analítica histórica. Antes de publicarlo, valida con el equipo propietario del sistema destino el formato esperado, permisos, frecuencia y criterios de calidad.
