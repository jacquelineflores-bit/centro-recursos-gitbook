# Oracle XStream CDC Source Connector

|  |  |
| --- | --- |
|  | **Conector para incorporar en GlobalSuite registros, tablas, colecciones y cambios de datos procedentes de Oracle XStream CDC.**  **Etiquetas:** Bases de datos | Integración | Source | CDC |

|  |  |
| --- | --- |
| Herramienta o sistema | Oracle XStream CDC |
| Fabricante de la herramienta | Oracle |
| Proveedor del conector | Confluent, Inc |
| Nombre del conector | Oracle XStream CDC Source Connector |
| Tipo de conector | Source |
| Etiquetas | Bases de datos | Integración | Source | CDC |
| Información que maneja | registros, tablas, colecciones y cambios de datos |

## Detalles

El conector Oracle XStream CDC Source Connector permite incorporar a GlobalSuite información procedente de Oracle XStream CDC relacionada con registros, tablas, colecciones y cambios de datos.

Está orientado a mantener actualizados procesos de gestión, evidencias e indicadores sin depender de cargas manuales, especialmente en escenarios de sincronización de catálogos, auditoría de cambios, reporting regulatorio y eliminación de cargas manuales.

## Características

* Incorporación configurable de registros, tablas, colecciones y cambios de datos desde Oracle XStream CDC hacia los procesos de GlobalSuite.
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

1. Accede al Marketplace de GlobalSuite® y selecciona Oracle XStream CDC Source Connector.
2. Configura la conexión con Oracle XStream CDC: URL o endpoint, credenciales, permisos y entorno.
3. Define el alcance funcional de la sincronización: registros, tablas, colecciones y cambios de datos, filtros y frecuencia.
4. Mapea los campos recibidos con las entidades, evidencias o procesos correspondientes de GlobalSuite.
5. Ejecuta una prueba, revisa los registros sincronizados y activa la integración.

## Más información

<https://www.oracle.com/database/technologies/high-availability/goldengate.html>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando necesites incorporar información de Oracle XStream CDC en procesos de GlobalSuite, por ejemplo para sincronización de catálogos, auditoría de cambios, reporting regulatorio y eliminación de cargas manuales. Antes de publicarlo, acuerda con el área propietaria qué datos son necesarios, con qué frecuencia deben actualizarse y quién revisará los resultados.
