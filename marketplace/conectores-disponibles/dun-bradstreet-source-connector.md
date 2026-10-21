# Dun & Bradstreet Source Connector

|  |  |
| --- | --- |
|  | **Conector para obtener noticias corporativas y alertas de riesgo de los proveedores de su empresa.**  **Etiquetas:** Source | Due Diligence |

|  |  |
| --- | --- |
| Herramienta o sistema | Dun & Bradstreet |
| Fabricante de la herramienta | Dun & Bradstreet |
| Proveedor del conector | GlobalSuite Solutions |
| Nombre del conector | Dun & Bradstreet Source Connector |
| Tipo de conector | Source |
| Etiquetas | Source | Due Diligence |
| Información que maneja | identificación D-U-N-S, noticias corporativas y alertas de riesgo |

## Detalles

El conector Dun & Bradstreet Source Connector permite incorporar a GlobalSuite las noticias corporativas y las alertas de riesgo que Dun & Bradstreet publica sobre los proveedores registrados en la organización, resolviendo previamente su identificador D-U-N-S.

Está orientado a sostener la monitorización continua de terceros con una identidad estable y contrastada, especialmente en carteras internacionales y en grupos empresariales con filiales, donde la desambiguación del proveedor es crítica.

## Características

* Resolución del identificador D-U-N-S del proveedor a partir de su razón social, país y datos de domicilio.
* Registro del nivel de confianza de la correspondencia, para revisar los casos ambiguos.
* Sincronización incremental de noticias por rango de fechas desde la última ejecución.
* Clasificación de las noticias por categoría, según la tipificación de la fuente.
* Volcado en el apartado Noticias y Cumplimiento del proveedor a través del GlobalSuite Sink Connector.

## Beneficios clave

* Aporta una identidad de proveedor estable y reconocida internacionalmente.
* Reduce los falsos positivos en carteras con grupos empresariales y filiales.
* Concentra las alertas de riesgo corporativo en la propia ficha del proveedor.
* Facilita evidenciar la vigilancia continua ante auditorías y comités de riesgo.
* Mejora la coordinación entre compras, cumplimiento y las áreas propietarias del servicio.

## Instalación

|  |
| --- |
| **Nota de configuración:** Antes de activar la integración, valida credenciales, permisos, alcance funcional y una prueba de datos con el área responsable. |

1. Accede al Marketplace de GlobalSuite® y selecciona Dun & Bradstreet Source Connector. Configura la conexión con Dun & Bradstreet: URL o endpoint, credenciales, permisos y entorno. Indica la URL y la API Key de GlobalSuite® para que el conector pueda leer los proveedores registrados. Define el alcance funcional de la sincronización: las categorías de noticia relevantes, el rango de fechas y la frecuencia de sincronización. Activa la sincronización de noticias para que el conector publique en el destino que consume el GlobalSuite Sink Connector. Ejecuta una prueba, revisa los registros sincronizados y activa la integración.

## Más información

<https://directplus.documentation.dnb.com/>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando la organización tenga contratado un servicio de Dun & Bradstreet y necesite una identificación fiable de sus proveedores junto con sus noticias y alertas de riesgo. Antes de activarlo, define el umbral de confianza a partir del cual la correspondencia se acepta automáticamente y quién revisará los casos ambiguos.

Para conocer dónde se muestran las noticias en el producto, consulta [Noticias y Cumplimiento](https://globalsuitesolutions.atlassian.net/wiki/pages/createpage.action?spaceKey=GlobalSUITEes&title=Noticias%20y%20Cumplimiento).
