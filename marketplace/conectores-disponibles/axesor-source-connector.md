# Axesor Source Connector

|  |  |
| --- | --- |
|  | **Conector para obtener noticias, incidencias y datos de solvencia de los proveedores de su empresa.**  **Etiquetas:** Source | Due Diligence |

|  |  |
| --- | --- |
| Herramienta o sistema | Axesor |
| Fabricante de la herramienta | Axesor (Experian) |
| Proveedor del conector | GlobalSuite Solutions |
| Nombre del conector | Axesor Source Connector |
| Tipo de conector | Source |
| Etiquetas | Source | Due Diligence |
| Información que maneja | noticias de prensa, incidencias judiciales y administrativas, y datos financieros y de rating |

## Detalles

El conector Axesor Source Connector permite incorporar a GlobalSuite la información del Informe 360 de Axesor para los proveedores registrados en la organización, tanto sus noticias de prensa e incidencias publicadas en boletines oficiales como sus datos identificativos, financieros y de rating.

Está orientado a mantener actualizada la ficha del proveedor y su vigilancia continua sin consultas manuales, especialmente en carteras de proveedores españoles, donde aporta además solvencia, estado registral y grupo de riesgo.

## Características

* Lectura de los proveedores registrados en GlobalSuite y consulta a la fuente a partir del CIF de cada proveedor.
* Incorporación de noticias de prensa con titular, fecha y medio de publicación.
* Incorporación de incidencias judiciales y administrativas publicadas en boletines oficiales.
* Actualización de datos identificativos, domicilio, estado registral, rating, probabilidad de impago y grupo de riesgo.
* Volcado en el apartado Noticias y Cumplimiento del proveedor a través del GlobalSuite Sink Connector.

## Beneficios clave

* Reúne en un único origen la solvencia y las novedades públicas del proveedor.
* Evita la consulta informe a informe para carteras amplias de proveedores.
* Anticipa señales de riesgo financiero o litigios antes de que impacten en el servicio.
* Ayuda a justificar decisiones de homologación y renovación con datos trazables.
* Mejora la coordinación entre compras, finanzas y cumplimiento.

## Instalación

|  |
| --- |
| **Nota de configuración:** Antes de activar la integración, valida credenciales, permisos, alcance funcional y una prueba de datos con el área responsable. |

1. Accede al Marketplace de GlobalSuite® y selecciona Axesor Source Connector. Configura la conexión con Axesor: URL o endpoint, credenciales, permisos y entorno. Indica la URL y la API Key de GlobalSuite® para que el conector pueda leer los proveedores registrados. Define el alcance funcional de la sincronización: los proveedores a consultar, la información del informe que se quiere trasladar y la frecuencia. Activa la sincronización de noticias para que el conector publique en el destino que consume el GlobalSuite Sink Connector. Ejecuta una prueba, revisa los registros sincronizados y activa la integración.

## Más información

<https://www.axesor.es/>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando la organización tenga contratado el servicio de informes de Axesor y quiera enriquecer sus proveedores y su apartado de noticias en GlobalSuite. Ten en cuenta que el servicio se factura por consulta, así que acuerda con el área propietaria el alcance y la frecuencia antes de activarlo.

Para conocer dónde se muestran las noticias en el producto, consulta [Noticias y Cumplimiento](https://globalsuitesolutions.atlassian.net/wiki/pages/createpage.action?spaceKey=GlobalSUITEes&title=Noticias%20y%20Cumplimiento).
