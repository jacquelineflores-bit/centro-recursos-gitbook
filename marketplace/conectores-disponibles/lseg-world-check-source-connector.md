# LSEG World-Check Source Connector

|  |  |
| --- | --- |
|  | **Conector para obtener coincidencias de screening y medios adversos de los proveedores de su empresa.**  **Etiquetas:** Source | Due Diligence |

|  |  |
| --- | --- |
| Herramienta o sistema | LSEG World-Check |
| Fabricante de la herramienta | LSEG (London Stock Exchange Group) |
| Proveedor del conector | GlobalSuite Solutions |
| Nombre del conector | LSEG World-Check Source Connector |
| Tipo de conector | Source |
| Etiquetas | Source | Due Diligence |
| Información que maneja | coincidencias en listas de sanciones, personas de relevancia pública (PEP) y medios adversos |

## Detalles

El conector LSEG World-Check Source Connector permite incorporar a GlobalSuite las coincidencias de screening que World-Check publica sobre los proveedores registrados en la organización: listas de sanciones, personas de relevancia pública y medios adversos.

Está orientado a cubrir el cribado regulatorio de terceros de forma continua y trazable, especialmente en procesos de know your supplier, prevención de blanqueo de capitales y cumplimiento de programas de sanciones.

## Características

* Lectura de los proveedores registrados en GlobalSuite y cribado de cada uno contra la fuente.
* Incorporación de las coincidencias detectadas con su categoría y su nivel de criticidad.
* Distinción entre coincidencias nuevas y ya conocidas, para centrarse en las novedades.
* Enlace a la ficha de origen de la coincidencia cuando la fuente lo facilita.
* Volcado en el apartado Noticias y Cumplimiento del proveedor a través del GlobalSuite Sink Connector.

## Beneficios clave

* Cubre el cribado de sanciones y PEP de la cartera de proveedores de forma sistemática.
* Concentra las coincidencias en la ficha del proveedor, con constancia de su revisión.
* Reduce el riesgo de operar con un tercero sancionado sin haberlo detectado.
* Facilita evidenciar el cumplimiento del programa de cribado ante auditoría o supervisor.
* Mejora la coordinación entre cumplimiento, compras y asesoría jurídica.

## Instalación

|  |
| --- |
| **Nota de configuración:** Antes de activar la integración, valida credenciales, permisos, alcance funcional y una prueba de datos con el área responsable. |

1. Accede al Marketplace de GlobalSuite® y selecciona LSEG World-Check Source Connector. Configura la conexión con LSEG World-Check: URL o endpoint, credenciales, permisos y entorno. Indica la URL y la API Key de GlobalSuite® para que el conector pueda leer los proveedores registrados. Define el alcance funcional de la sincronización: las listas y categorías de cribado aplicables, el umbral de coincidencia y la frecuencia. Activa la sincronización de noticias para que el conector publique en el destino que consume el GlobalSuite Sink Connector. Ejecuta una prueba, revisa los registros sincronizados y activa la integración.

## Más información

<https://www.lseg.com/en/risk-intelligence>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando la organización tenga contratado World-Check y necesite un cribado continuo de sus proveedores dentro de GlobalSuite. Antes de activarlo, define el umbral de coincidencia, quién resuelve los posibles falsos positivos y cómo se documenta la decisión.

Para conocer dónde se muestran las noticias en el producto, consulta [Noticias y Cumplimiento](https://globalsuitesolutions.atlassian.net/wiki/pages/createpage.action?spaceKey=GlobalSUITEes&title=Noticias%20y%20Cumplimiento).
