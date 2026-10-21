# Dow Jones Risk & Compliance Source Connector

|  |  |
| --- | --- |
|  | **Conector para obtener noticias y alertas de cumplimiento de los proveedores de su empresa.**  **Etiquetas:** Source | Due Diligence |

|  |  |
| --- | --- |
| Herramienta o sistema | Dow Jones Risk & Compliance |
| Fabricante de la herramienta | Dow Jones |
| Proveedor del conector | GlobalSuite Solutions |
| Nombre del conector | Dow Jones Risk & Compliance Source Connector |
| Tipo de conector | Source |
| Etiquetas | Source | Due Diligence |
| Información que maneja | noticias, medios adversos, sanciones y personas de relevancia pública (PEP) |

## Detalles

El conector Dow Jones Risk & Compliance Source Connector permite incorporar a GlobalSuite las noticias y alertas de cumplimiento que Dow Jones publica sobre los proveedores registrados en la organización, resolviendo previamente la identidad de cada proveedor en la fuente.

Está orientado a sostener la monitorización continua de terceros sin depender de consultas manuales en el portal de la fuente, especialmente en escenarios de due diligence, revisión de medios adversos, cribado de sanciones y seguimiento de personas de relevancia pública.

## Características

* Lectura de los proveedores registrados en GlobalSuite y correspondencia con la compañía equivalente en la fuente.
* Sincronización incremental de novedades, para traer solo las noticias publicadas desde la última ejecución.
* Normalización de cada noticia con titular, fecha de publicación, fuente, categoría y criticidad.
* Volcado en el apartado Noticias y Cumplimiento del proveedor a través del GlobalSuite Sink Connector.
* Registro de la sincronización para revisar qué se ha traído y cuándo.

## Beneficios clave

* Concentra en la ficha del proveedor las alertas que hoy se revisan en el portal de la fuente.
* Reduce el tiempo dedicado a la vigilancia continua de la cartera de terceros.
* Permite priorizar la revisión por criticidad y categoría de la noticia.
* Facilita evidenciar ante auditoría que la monitorización de proveedores se realiza de forma periódica.
* Mejora la coordinación entre compras, cumplimiento y las áreas propietarias del servicio.

## Instalación

|  |
| --- |
| **Nota de configuración:** Antes de activar la integración, valida credenciales, permisos, alcance funcional y una prueba de datos con el área responsable. |

1. Accede al Marketplace de GlobalSuite® y selecciona Dow Jones Risk & Compliance Source Connector. Configura la conexión con Dow Jones Risk & Compliance: URL o endpoint, credenciales, permisos y entorno. Indica la URL y la API Key de GlobalSuite® para que el conector pueda leer los proveedores registrados. Define el alcance funcional de la sincronización: las noticias y alertas de cumplimiento que se quieren traer, los filtros por categoría y la frecuencia. Activa la sincronización de noticias para que el conector publique en el destino que consume el GlobalSuite Sink Connector. Ejecuta una prueba, revisa los registros sincronizados y activa la integración.

## Más información

<https://developer.dowjones.com/>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando la organización tenga contratado Dow Jones Risk & Compliance y necesite que sus alertas lleguen al apartado de noticias de los proveedores de GlobalSuite. Antes de activarlo, acuerda con el área propietaria qué categorías son relevantes, con qué frecuencia deben actualizarse y quién revisará las noticias recibidas.

Para conocer dónde se muestran las noticias en el producto, consulta [Noticias y Cumplimiento](https://globalsuitesolutions.atlassian.net/wiki/pages/createpage.action?spaceKey=GlobalSUITEes&title=Noticias%20y%20Cumplimiento).
