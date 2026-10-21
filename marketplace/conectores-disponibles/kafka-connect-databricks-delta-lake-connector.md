# Kafka Connect Databricks Delta Lake Connector

|  |  |
| --- | --- |
|  | **Conector para enviar desde GlobalSuite ficheros, evidencias, documentos y objetos de almacenamiento hacia Databricks Delta Lake o hacia el sistema destino definido.**  **Etiquetas:** Data Warehouse | Cloud | Sink | Almacenamiento |

|  |  |
| --- | --- |
| Herramienta o sistema | Databricks Delta Lake |
| Fabricante de la herramienta | Databricks |
| Proveedor del conector | Confluent, Inc |
| Nombre del conector | Kafka Connect Databricks Delta Lake Connector |
| Tipo de conector | Sink |
| Etiquetas | Data Warehouse | Cloud | Sink | Almacenamiento |
| Información que maneja | ficheros, evidencias, documentos y objetos de almacenamiento |

## Detalles

El conector Kafka Connect Databricks Delta Lake Connector permite enviar desde GlobalSuite hacia Databricks Delta Lake información relacionada con ficheros, evidencias, documentos y objetos de almacenamiento.

Es útil cuando Databricks Delta Lake debe actuar como sistema de destino, explotación, archivo o monitorización para casos de retención de evidencias, intercambio de ficheros con terceros, archivo documental y explotación analítica posterior.

## Características

* Envío controlado de ficheros, evidencias, documentos y objetos de almacenamiento desde GlobalSuite hacia Databricks Delta Lake o hacia el repositorio destino definido.
* Gestión de rutas, carpetas, contenedores o prefijos para ordenar la información por proceso o periodo.
* Compatibilidad con usos de archivo, intercambio de evidencias, respaldo documental o explotación posterior.
* Definición de formatos, filtros y criterios de selección para limitar el volumen importado o exportado.
* Trazabilidad sobre qué ficheros se han procesado, cuándo y con qué resultado.

## Beneficios clave

* Facilita conservar evidencias y documentación en repositorios corporativos ya gobernados.
* Reduce cargas manuales de ficheros y mejora la organización por proceso, tercero, control o periodo.
* Apoya políticas de retención, auditoría y respaldo documental con menor esfuerzo operativo.
* Permite compartir información con áreas internas o terceros usando ubicaciones controladas.
* Mejora la preparación de datos para reporting, data lake o análisis posteriores.

## Instalación

|  |
| --- |
| **Nota de configuración:** Antes de activar la integración, valida credenciales, permisos, alcance funcional y una prueba de datos con el área responsable. |

1. Accede al Marketplace de GlobalSuite® y selecciona Kafka Connect Databricks Delta Lake Connector.
2. Configura el destino en Databricks Delta Lake: URL o endpoint, credenciales, permisos y entorno.
3. Define qué información se enviará: ficheros, evidencias, documentos y objetos de almacenamiento, filtros, formato y periodicidad.
4. Mapea los campos de GlobalSuite con la estructura esperada por el sistema destino.
5. Ejecuta una prueba, revisa la recepción en destino y activa la integración.

## Más información

<https://www.databricks.com/product/delta-lake-on-databricks>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando necesites enviar información de GlobalSuite a Databricks Delta Lake, por ejemplo para retención de evidencias, intercambio de ficheros con terceros, archivo documental y explotación analítica posterior. Antes de publicarlo, valida con el equipo propietario del sistema destino el formato esperado, permisos, frecuencia y criterios de calidad.
