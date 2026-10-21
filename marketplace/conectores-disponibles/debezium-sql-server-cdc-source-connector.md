# Debezium SQL Server CDC Source Connector

|  |  |
| --- | --- |
|  | **Debezium's SQL Server Connector can monitor and record the row-level changes in the schemas of a SQL Server 2017 database. This connector was added in Debezium 0.9.0. The first time it connects to a …**  **Etiquetas:** Bases de datos | Integración | Source | CDC |

|  |  |
| --- | --- |
| Herramienta o sistema | Debezium SQL Server CDC |
| Fabricante de la herramienta | Microsoft |
| Proveedor del conector | Confluent |
| Nombre del conector | Debezium SQL Server CDC Source Connector |
| Tipo de conector | Source |
| Etiquetas | Bases de datos | Integración | Source | CDC |
| Información que maneja | registros, tablas, colecciones y cambios de datos |

## Detalles

El conector Debezium SQL Server CDC Source Connector permite incorporar a GlobalSuite información procedente de Debezium SQL Server CDC relacionada con registros, tablas, colecciones y cambios de datos.

Está orientado a mantener actualizados procesos de gestión, evidencias e indicadores sin depender de cargas manuales, especialmente en escenarios de sincronización de catálogos, auditoría de cambios, reporting regulatorio y eliminación de cargas manuales.

## Características

* Incorporación configurable de registros, tablas, colecciones y cambios de datos desde Debezium SQL Server CDC hacia los procesos de GlobalSuite.
* Selección de tablas, colecciones, vistas o campos para sincronizar sólo información con valor funcional.
* Soporte a altas, modificaciones y bajas cuando el sistema origen o destino lo permite.
* Mapeo de claves, campos y entidades para mantener coherencia con catálogos e inventarios corporativos.
* Trazabilidad de cambios y resultados para auditoría, conciliación y control de calidad de datos.

## Beneficios clave

* Mantiene catálogos, inventarios y registros críticos sincronizados con menor intervención manual.
* Reduce errores por duplicidad o desalineación entre bases de datos y procesos de GlobalSuite.
* Facilita auditoría de cambios, conciliación de información y reporting regulatorio.
* Permite incorporar información operativa al flujo GRC sin esperar exportaciones puntuales.
* Mejora la calidad del dato al trabajar con orígenes estructurados y reglas de mapeo definidas.

## Instalación

|  |
| --- |
| **Nota de configuración:** Antes de activar la integración, valida credenciales, permisos, alcance funcional y una prueba de datos con el área responsable. |

1. Accede al Marketplace de GlobalSuite® y selecciona Debezium SQL Server CDC Source Connector.
2. Configura la conexión con Debezium SQL Server CDC: URL o endpoint, credenciales, permisos y entorno.
3. Define el alcance funcional de la sincronización: registros, tablas, colecciones y cambios de datos, filtros y frecuencia.
4. Mapea los campos recibidos con las entidades, evidencias o procesos correspondientes de GlobalSuite.
5. Ejecuta una prueba, revisa los registros sincronizados y activa la integración.

## Más información

<https://debezium.io/documentation/>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando necesites incorporar información de Debezium SQL Server CDC en procesos de GlobalSuite, por ejemplo para sincronización de catálogos, auditoría de cambios, reporting regulatorio y eliminación de cargas manuales. Antes de publicarlo, acuerda con el área propietaria qué datos son necesarios, con qué frecuencia deben actualizarse y quién revisará los resultados.
