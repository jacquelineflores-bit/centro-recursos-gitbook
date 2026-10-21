# Funcionamiento de encuestas BIA ante cambios en la configuración

|  |
| --- |
| **Idea clave**  Las encuestas BIA guardan una foto de la configuración propia del modelo de encuesta en el momento de su lanzamiento. Sin embargo, determinados parámetros de la configuración general de BIA siguen siendo compartidos al módulo de BIA y al módulo de encuestas BIA, por lo que sus cambios pueden impactar en encuestas activas o ya existentes. |

## 1. Objetivo

Este artículo explica cómo se comportan las encuestas BIA de GlobalSuite® cuando se modifican configuraciones relacionadas con el Análisis de Impacto en el Negocio. El objetivo es aclarar qué cambios quedan congelados en las encuestas ya lanzadas, qué cambios pueden seguir aplicando sobre encuestas existentes y qué buenas prácticas deben seguirse para evitar impactos no deseados durante una campaña activa.

La explicación aplica al módulo de BIAs, a los modelos de encuesta BIA y a las encuestas BIA generadas para procesos de negocio, especialmente cuando se utilizan para recopilar información de áreas usuarias no expertas en continuidad.

## 2. Contexto funcional

GlobalSuite dispone de un módulo de BIA para realizar la Evaluación de Impacto en el Negocio de los procesos. La estructura del formulario BIA es configurable a nivel de la solución y puede incluir, entre otros elementos, tipos de impacto, escalas temporales, niveles, campos, etiquetas, bloques, preguntas personalizables y recursos críticos.

Además, el módulo de encuestas BIA permite definir modelos o plantillas de encuesta. Estos modelos sirven para adaptar la experiencia de cumplimentación al destinatario, por ejemplo, sustituyendo campos metodológicos como MTPD, RTO o RPO por preguntas más comprensibles para usuarios de negocio, configurando la visibilidad de campos o seleccionando qué preguntas personalizables se incluyen en cada bloque.

Cuando se lanza una nueva encuesta BIA, la herramienta conserva una foto de la configuración propia del modelo de encuesta utilizado. Por este motivo, si posteriormente se modifica el modelo de encuesta, las encuestas ya lanzadas no se actualizan con esos cambios.

La particularidad que debe tenerse en cuenta es que esta foto no convierte todos los parámetros del BIA en una copia independiente. Existen parámetros estructurales de la configuración general de BIA que son compartidos por los BIAs y por las encuestas BIA, y que pueden afectar a encuestas existentes si se modifican.

## 3. Dos niveles de configuración

Para entender el comportamiento es importante diferenciar dos tipos de configuración: la configuración general de BIA y la configuración propia del modelo de encuesta.

|  |  |  |  |
| --- | --- | --- | --- |
| **Nivel de configuración** | **Dónde se configura** | **Ejemplos** | **Comportamiento esperado** |
| Configuración general de BIA | Ajustes > Continuidad > BIAs | Tipos de impacto, escalas de impacto, niveles, criticidad, criterios de cálculo, bloques o secciones del formulario, campos base del BIA, preguntas personalizables definidas a nivel BIA. | Es una configuración estructural compartida por BIAs y encuestas BIA. Puede aplicar sobre encuestas activas o existentes porque afecta a la estructura, cálculo, consolidación e integridad del dato. |
| Modelo de encuesta BIA | Ajustes o Gestión de modelos de encuesta BIA, según la configuración de la instalación | Visibilidad y obligatoriedad de campos en la encuesta, textos de preguntas, sustitución de campos metodológicos por preguntas, preguntas incluidas en el modelo, bloque y orden en el que se muestran, mensajes introductorios y adjuntos del modelo. | Se toma como foto al lanzar la encuesta. Si se modifica el modelo después del lanzamiento, no afecta a las encuestas ya generadas. Aplica a nuevas encuestas creadas a partir del modelo actualizado. |

|  |
| --- |
| **Importante**  El hecho de que una encuesta BIA conserve la configuración del modelo no significa que quede aislada de todos los cambios realizados en la configuración general de BIA. Los cambios metodológicos o estructurales deben planificarse fuera de campañas activas. |

## 4. Funcionamiento ante cambios

### 4.1 Cambios realizados en el modelo de encuesta BIA

Los cambios realizados en un modelo de encuesta BIA afectan a las nuevas encuestas que se generen a partir de ese modelo, pero no modifican las encuestas ya lanzadas. Esto permite mantener distintas plantillas para distintos ámbitos, como encuestas estratégicas, encuestas para procesos operativos o encuestas adaptadas a perfiles concretos de negocio.

* Modificar el texto de una pregunta del modelo no cambia el texto ya mostrado en encuestas existentes.
* Cambiar la visibilidad de un campo en el modelo no modifica el alcance de encuestas ya lanzadas.
* Añadir o retirar una pregunta del modelo no altera las encuestas ya generadas con una versión anterior del modelo.
* Reordenar campos o preguntas dentro del modelo aplica a nuevas encuestas creadas desde ese modelo actualizado.

Este comportamiento permite que cada campaña mantenga coherencia interna respecto al modelo con el que fue creada.

### 4.2 Cambios realizados en la configuración general de BIA

Los cambios realizados en la configuración general de BIA tienen un alcance diferente. Esta configuración es la base estructural del propio formulario BIA y también de las encuestas BIA. Por tanto, determinados cambios pueden verse reflejados en encuestas activas o ya existentes.

* Cambios en tipos de impacto, niveles, escalas temporales o criterios de criticidad pueden afectar a la forma en que se muestra, calcula o consolida la información.
* Cambios en bloques o secciones del formulario pueden afectar a la navegación, orden o agrupación de campos en encuestas ya existentes.
* Ocultar o deshabilitar campos en la configuración general puede limitar su disponibilidad en los modelos de encuesta.
* Cambios en preguntas personalizables definidas a nivel BIA pueden tener efecto cuando esas preguntas forman parte de la estructura común que consume el modelo.

Este comportamiento no es una incidencia puntual, sino el funcionamiento definido desde el diseño original del módulo de encuestas BIA. La razón principal es preservar la relación entre encuesta, BIA, cálculos y consolidación de datos.

### 4.3 Resumen de comportamiento

|  |  |  |
| --- | --- | --- |
| **Cambio realizado** | **Afecta a encuestas ya lanzadas** | **Motivo** |
| Modificar el texto de una pregunta configurada en el modelo de encuesta. | No, salvo que se cree una nueva encuesta. | El modelo de encuesta queda fotografiado al lanzar la encuesta. |
| Ocultar un campo en el modelo de encuesta. | No para encuestas ya lanzadas. | La visibilidad propia del modelo forma parte de la configuración congelada de la encuesta. |
| Cambiar tipos de impacto o escalas de impacto. | Sí, puede afectar. | Son parámetros metodológicos comunes al BIA y a las encuestas BIA. |
| Modificar niveles, criticidad o criterios de cálculo. | Sí, puede afectar. | Intervienen en el cálculo, representación y consolidación de resultados del BIA. |
| Cambiar bloques o secciones generales del formulario BIA. | Sí, puede afectar. | Los bloques forman parte de la estructura general usada por el formulario BIA y por la navegación de encuestas. |
| Añadir una pregunta al modelo de encuesta. | No para encuestas existentes. | La inclusión de preguntas en el modelo queda fijada al lanzar la encuesta. |
| Crear una nueva encuesta después de actualizar modelo y configuración general. | Sí, en la nueva encuesta. | La nueva encuesta toma la configuración vigente en el momento de su creación. |

## 5. Por qué la configuración general puede impactar en encuestas activas

La configuración general de BIA define la metodología y la estructura común que permite que la información completada en una encuesta se pueda trasladar correctamente al BIA del proceso. Por este motivo, no todos los elementos pueden tratarse como simples textos o campos visuales de una plantilla.

Algunos parámetros son necesarios para mantener la integridad del dato: determinan qué se mide, cómo se calcula, cómo se agrupa y cómo se consolida. Si estos elementos se duplicaran de forma completamente independiente para cada encuesta, podrían producirse inconsistencias entre lo que el usuario responde, lo que se consolida en el BIA y lo que se explota posteriormente en informes o históricos.

Por ejemplo, un cambio en los niveles de impacto o en la escala temporal no es equivalente a cambiar el texto de una pregunta. Afecta a la interpretación metodológica de las respuestas y puede alterar la forma en la que se calcula la criticidad o se determina la recuperación del proceso.

## 6. Buenas prácticas recomendadas

### 6.1 No realizar cambios estructurales con campañas activas

No se recomienda realizar cambios estructurales o metodológicos en la configuración general de BIA mientras exista una campaña de encuestas activa. Esta recomendación aplica especialmente a cambios en tipos de impacto, escalas, niveles, bloques, criticidad, cálculos de MTPD/RTO/RPO, campos base del BIA o preguntas generales utilizadas por el formulario.

|  |
| --- |
| **Recomendación**  Antes de lanzar una campaña, revise y valide la metodología BIA completa. Durante la campaña, limite los cambios a ajustes operativos que no alteren la estructura ni la metodología. |

### 6.2 Crear un histórico de BIAs antes de modificar la metodología

Antes de modificar la configuración general de BIA, se recomienda crear un histórico de los BIAs afectados. El histórico permite conservar las evaluaciones y la configuración existente en ese momento, de forma que se pueda consultar posteriormente la información con la estructura y las preguntas vigentes cuando se generó el histórico.

Esta práctica es especialmente relevante cuando se va a cambiar la estructura del formulario, los criterios de impacto o las preguntas utilizadas para la evaluación.

### 6.3 Descargar el informe Word de la encuesta como evidencia

Desde cada encuesta BIA puede generarse un informe descargable con el contenido completado hasta ese momento. Se recomienda descargar el informe Word de la encuesta antes de realizar cambios estructurales, especialmente si la encuesta forma parte de una campaña ya iniciada o si se necesita conservar evidencia de auditoría.

Este informe permite almacenar una evidencia externa del contenido respondido, independientemente de que posteriormente se realicen cambios en la configuración general de BIA.

### 6.4 No reutilizar encuestas o publicaciones en ciclos sucesivos

No se recomienda reutilizar encuestas o publicaciones de campañas anteriores para ciclos o años sucesivos. La práctica recomendada es iniciar un flujo nuevo para cada campaña o ciclo de revisión.

Al comenzar un flujo nuevo, las encuestas se crean con la configuración actualizada tanto del BIA como del modelo de encuesta utilizado. Además, se mantiene correctamente el origen de la información completada para el BIA del proceso, evitando confusiones entre ciclos metodológicos diferentes.

### 6.5 Validar la consolidación antes de ejecutar Crear BIA o Modificar BIA

Las acciones Crear BIA y Modificar BIA trasladan la información de la encuesta al BIA correspondiente. Estas acciones deben ejecutarse cuando la encuesta y la configuración metodológica hayan sido revisadas, ya que la consolidación realizada desde la encuesta no debe considerarse un cambio provisional.

|  |
| --- |
| **Importante**  Antes de consolidar una encuesta BIA en el BIA del proceso, revise que la campaña ha finalizado, que las respuestas son correctas y que no existen cambios metodológicos pendientes. |

## 7. Procedimiento recomendado para cambios metodológicos

Cuando sea necesario modificar la configuración general de BIA, se recomienda seguir este procedimiento operativo:

1. Identificar si hay campañas de encuestas BIA activas o publicaciones pendientes de respuesta.
2. Cerrar o finalizar la campaña activa antes de modificar la configuración general, siempre que sea posible.
3. Descargar el informe Word de las encuestas relevantes para conservar evidencia del contenido completado.
4. Crear un histórico de los BIAs que deban conservarse con la metodología anterior.
5. Aplicar los cambios necesarios en Ajustes > Continuidad > BIAs.
6. Revisar y actualizar los modelos de encuesta BIA que deban adaptarse a la nueva metodología.
7. Lanzar una nueva campaña o flujo de encuestas, en lugar de reutilizar encuestas o publicaciones anteriores.
8. Validar una encuesta de prueba antes de enviar la campaña completa a los destinatarios.
9. Consolidar los resultados en el BIA solo cuando la campaña esté revisada y finalizada.

## 8. Ejemplos prácticos

|  |  |  |
| --- | --- | --- |
| **Situación** | **Interpretación** | **Práctica recomendada** |
| Se cambia la redacción de la pregunta que sustituye al campo MTPD en el modelo de encuesta. | Las encuestas ya lanzadas mantienen el texto anterior. Las nuevas encuestas usarán el nuevo texto. | Crear una nueva encuesta si se necesita que los destinatarios respondan con la nueva redacción. |
| Se añade un nuevo tipo de impacto en la configuración general de BIA durante una campaña. | Puede afectar a la estructura de evaluación y a la forma de consolidar impactos. | No realizar el cambio hasta cerrar la campaña o crear una nueva campaña con la metodología actualizada. |
| Se cambia el nombre o el orden de un bloque general del formulario BIA. | Puede afectar a la navegación y agrupación de campos en encuestas existentes. | Planificar el cambio fuera de campañas activas y documentar la modificación. |
| Se oculta un campo desde la configuración general de BIA. | El campo puede dejar de estar disponible para los modelos de encuesta y afectar a la consolidación. | Revisar los modelos dependientes antes de aplicar el cambio. |
| Se quiere repetir la campaña anual del año anterior. | Reutilizar la encuesta anterior puede mezclar una campaña antigua con una configuración actualizada parcialmente. | Crear una nueva configuración/publicación o un nuevo flujo para el ciclo actual. |

## 9. Conclusión

Las encuestas BIA combinan dos comportamientos: estabilidad de la configuración propia del modelo de encuesta y dependencia de la configuración estructural general del BIA. Esta combinación permite adaptar la experiencia de respuesta para distintos usuarios o ámbitos, manteniendo al mismo tiempo la coherencia de los datos que se consolidan en el BIA del proceso.

Para evitar incidencias operativas, la recomendación principal es no modificar la configuración general de BIA durante campañas activas, conservar evidencia mediante informes Word, generar históricos antes de cambios metodológicos y crear nuevos flujos de encuesta para cada ciclo o campaña.

## 10. Páginas relacionadas del manual

Para ampliar la información operativa, se recomienda revisar las siguientes páginas del manual de usuario:

* [Configuración BIA.](https://help.globalsuitesolutions.com/es/globalsuite/v1/configuracion-bia)
* [Modelo Encuesta BIA por Impacto](https://help.globalsuitesolutions.com/es/globalsuite/v1/modelo-encuesta-bia-por-impacto).
* [Encuestas BIA (Configuración).](https://help.globalsuitesolutions.com/es/globalsuite/v1/encuestas-bia-configuracion)
* [Encuesta BIA](https://help.globalsuitesolutions.com/es/globalsuite/v1/encuestas-bia-impactos).
* [Encuesta](https://help.globalsuitesolutions.com/es/globalsuite/v1/encuestas-bia-impactos)
* [Flujo de encuestas y creación o modificación del BIA.](https://help.globalsuitesolutions.com/es/globalsuite/v1/flujo-de-encuestas-y-consolidacion)
* [Seguimientos, comentarios y archivos adjuntos.](https://help.globalsuitesolutions.com/es/globalsuite/v1/seguimientos-comentarios-y-archivos-adjuntos)
* [Históricos BIAs.](https://help.globalsuitesolutions.com/es/globalsuite/v1/historicos-bias)
