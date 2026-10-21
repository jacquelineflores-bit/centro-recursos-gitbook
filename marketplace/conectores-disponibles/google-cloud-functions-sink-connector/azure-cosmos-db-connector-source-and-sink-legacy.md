# Azure Cosmos DB Connector (Source and Sink) (Legacy)

|  |  |
| --- | --- |
|  | **Conector para intercambiar registros, tablas, colecciones y cambios de datos entre GlobalSuite y Azure Cosmos DB ( ) en los escenarios habilitados.**  **Etiquetas:** Bases de datos | Source y Sink | Cloud |

|  |  |
| --- | --- |
| Herramienta o sistema | Azure Cosmos DB ( ) |
| Fabricante de la herramienta | Microsoft |
| Proveedor del conector | Microsoft Corporation |
| Nombre del conector | Azure Cosmos DB Connector (Source and Sink) (Legacy) |
| Tipo de conector | Source y Sink |
| Etiquetas | Bases de datos | Source y Sink | Cloud |
| Información que maneja | registros, tablas, colecciones y cambios de datos |

## Detalles

El conector Azure Cosmos DB Connector (Source and Sink) (Legacy) permite intercambiar información entre GlobalSuite y Azure Cosmos DB ( ), combinando flujos de entrada y salida según el caso de uso.

Facilita mantener alineados registros, tablas, colecciones y cambios de datos en ambos entornos, con especial aplicación en escenarios de sincronización de catálogos, auditoría de cambios, reporting regulatorio y eliminación de cargas manuales.

## Características

* Intercambio bidireccional de registros, tablas, colecciones y cambios de datos entre GlobalSuite y Azure Cosmos DB ( ), según el flujo habilitado.
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

1. Accede al Marketplace de GlobalSuite® y selecciona Azure Cosmos DB Connector (Source and Sink) (Legacy).
2. Configura la conexión con Azure Cosmos DB ( ): URL o endpoint, credenciales, permisos y entorno.
3. Define la dirección de cada flujo y el alcance funcional: registros, tablas, colecciones y cambios de datos, filtros y frecuencia.
4. Configura el mapeo de campos para la entrada, la salida o ambos escenarios.
5. Ejecuta pruebas separadas por dirección, valida resultados y activa la integración.

## Más información

<https://learn.microsoft.com/azure/cosmos-db/>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando Azure Cosmos DB ( ) y GlobalSuite deban intercambiar información en ambos sentidos, por ejemplo para sincronización de catálogos, auditoría de cambios, reporting regulatorio y eliminación de cargas manuales. Conviene separar claramente qué datos entran, qué datos salen y quién es responsable de resolver discrepancias.
