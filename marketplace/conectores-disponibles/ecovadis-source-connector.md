# EcoVadis Source Connector

|  |  |
| --- | --- |
|  | **Conector para obtener novedades de desempeño ESG de los proveedores de su empresa.**  **Etiquetas:** Source | Due Diligence |

|  |  |
| --- | --- |
| Herramienta o sistema | EcoVadis |
| Fabricante de la herramienta | EcoVadis |
| Proveedor del conector | GlobalSuite Solutions |
| Nombre del conector | EcoVadis Source Connector |
| Tipo de conector | Source |
| Etiquetas | Source | Due Diligence |
| Información que maneja | evaluaciones y novedades de desempeño ambiental, social y de gobernanza (ESG) |

## Detalles

El conector EcoVadis Source Connector permite incorporar a GlobalSuite las evaluaciones y las novedades de desempeño ambiental, social y de gobernanza que EcoVadis publica sobre los proveedores registrados en la organización.

Está orientado a integrar la sostenibilidad en la evaluación de terceros sin cargas manuales, especialmente en escenarios de reporting de sostenibilidad, homologación de proveedores y seguimiento de planes de mejora ESG.

## Características

* Lectura de los proveedores registrados en GlobalSuite y correspondencia con el proveedor evaluado en la fuente.
* Incorporación de las novedades de evaluación y de los cambios relevantes de puntuación.
* Clasificación de las novedades por ámbito de sostenibilidad informado por la fuente.
* Sincronización incremental, para traer solo las novedades posteriores a la última ejecución.
* Volcado en el apartado Noticias y Cumplimiento del proveedor a través del GlobalSuite Sink Connector.

## Beneficios clave

* Integra el desempeño ESG del proveedor en el mismo lugar donde se gestiona su riesgo.
* Evita mantener en paralelo hojas de cálculo con las evaluaciones de sostenibilidad.
* Permite detectar deterioros de desempeño antes de una renovación o una nueva adjudicación.
* Aporta trazabilidad para el reporting de sostenibilidad de la cadena de suministro.
* Mejora la coordinación entre sostenibilidad, compras y cumplimiento.

## Instalación

|  |
| --- |
| **Nota de configuración:** Antes de activar la integración, valida credenciales, permisos, alcance funcional y una prueba de datos con el área responsable. |

1. Accede al Marketplace de GlobalSuite® y selecciona EcoVadis Source Connector. Configura la conexión con EcoVadis: URL o endpoint, credenciales, permisos y entorno. Indica la URL y la API Key de GlobalSuite® para que el conector pueda leer los proveedores registrados. Define el alcance funcional de la sincronización: los ámbitos de sostenibilidad relevantes, los proveedores incluidos y la frecuencia. Activa la sincronización de noticias para que el conector publique en el destino que consume el GlobalSuite Sink Connector. Ejecuta una prueba, revisa los registros sincronizados y activa la integración.

## Más información

<https://www.ecovadis.com/>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando la organización tenga contratado EcoVadis y quiera que el desempeño ESG de sus proveedores llegue al apartado de noticias de GlobalSuite. Antes de activarlo, acuerda con el área de sostenibilidad qué novedades deben generar seguimiento y quién las revisará.

Para conocer dónde se muestran las noticias en el producto, consulta [Noticias y Cumplimiento](https://globalsuitesolutions.atlassian.net/wiki/pages/createpage.action?spaceKey=GlobalSUITEes&title=Noticias%20y%20Cumplimiento).
