# ClickHouse Kafka Connect Sink Connector

|  |  |
| --- | --- |
|  | **Conector para enviar desde GlobalSuite registros, tablas, colecciones y cambios de datos hacia ClickHouse o hacia el sistema destino definido.**  **Etiquetas:** Bases de datos | Sink |

|  |  |
| --- | --- |
| Herramienta o sistema | ClickHouse |
| Fabricante de la herramienta | ClickHouse |
| Proveedor del conector | ClickHouse Inc |
| Nombre del conector | ClickHouse Kafka Connect Sink Connector |
| Tipo de conector | Sink |
| Etiquetas | Bases de datos | Sink |
| Información que maneja | registros, tablas, colecciones y cambios de datos |

## Detalles

El conector ClickHouse Kafka Connect Sink Connector permite enviar desde GlobalSuite hacia ClickHouse información relacionada con registros, tablas, colecciones y cambios de datos.

Es útil cuando ClickHouse debe actuar como sistema de destino, explotación, archivo o monitorización para casos de sincronización de catálogos, auditoría de cambios, reporting regulatorio y eliminación de cargas manuales.

## Características

* Envío controlado de registros, tablas, colecciones y cambios de datos desde GlobalSuite hacia ClickHouse o hacia el repositorio destino definido.
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

1. Accede al Marketplace de GlobalSuite® y selecciona ClickHouse Kafka Connect Sink Connector.
2. Configura el destino en ClickHouse: URL o endpoint, credenciales, permisos y entorno.
3. Define qué información se enviará: registros, tablas, colecciones y cambios de datos, filtros, formato y periodicidad.
4. Mapea los campos de GlobalSuite con la estructura esperada por el sistema destino.
5. Ejecuta una prueba, revisa la recepción en destino y activa la integración.

## Más información

<https://clickhouse.com/>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando necesites enviar información de GlobalSuite a ClickHouse, por ejemplo para sincronización de catálogos, auditoría de cambios, reporting regulatorio y eliminación de cargas manuales. Antes de publicarlo, valida con el equipo propietario del sistema destino el formato esperado, permisos, frecuencia y criterios de calidad.
