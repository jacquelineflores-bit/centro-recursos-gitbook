# IA: Mecanismos de Seguridad en GlobalSuite

# CUESTIONES REFERENTES A MECANISMOS DE SEGURIDAD IMPLEMENTADOS EN LA IA DE GlobalSuite®

1. **¿Cuáles son los mecanismos de seguridad que GlobalSuite® ha implementado en su Inteligencia Artificial para proteger la información y garantizar la integridad de los datos?**

En la actualidad, los datos utilizados por el sistema son los que se introducen manualmente en el sistema en el momento de la consulta, o previamente seleccionados desde GlobalSuite. El uso de los datos se limita exclusivamente a aquellos que son proporcionados por los propios clientes en el uso de los asistentes.

Con el fin de proporcionar mayor claridad, es importante señalar que utilizamos **Azure OpenAI** como servicio, donde dichas implementaciones se encuentran desplegadas dentro de la región europea. A continuación, se reitera la siguiente información proporcionada por dicho servicio:

{% hint style="info" %}
\*\*Importante\*\*
Las indicaciones (entradas) y finalizaciones (salidas), las inserciones y los datos de entrenamiento:
\* NO están disponibles para otros clientes.
\* NO están disponibles para OpenAI.
\* NO se usan para mejorar los modelos de OpenAI.
\* NO se usan para entrenar, volver a entrenar o mejorar los modelos base de Azure OpenAI Service.
\* NO se usan para mejorar cualquier producto o servicio de Microsoft o de terceros sin su permiso ni instrucción.
\* Los modelos de Azure OpenAI ajustados están disponibles exclusivamente para su uso.
El servicio Azure OpenAI está operado por Microsoft como servicio de Azure; Microsoft hospeda los modelos de OpenAI en el entorno de Azure de Microsoft y el servicio no interactúa con ningún servicio operado por OpenAI (por ejemplo, ChatGPT o la API de OpenAI).
{% endhint %}

En el caso del Asistente conversacional, se emplean técnicas de Recuperación y Generación Automática de Respuestas (RAG), basadas en documentación interna desarrollada por el área de producto, sin incluir en ningún momento información o datos personales relacionados con los clientes.

2. **¿Cómo funciona exactamente la IA dentro de la plataforma y en qué procesos se aplica?**

En la actualidad, se encuentra disponible el Recomendador de Riesgos y Controles, el cual se aplica al análisis de riesgos. Esta funcionalidad se completa con los datos introducidos por el cliente de forma anonimizada para obtener los riesgos y controles que le aplican.

Adicionalmente, se cuenta con un asistente conversacional transversal de GlobalSuite para responder dudas sobre el uso de la solución y dudas sobre cuestiones normativas. Esta funcionalidad se alimenta de únicamente documentación interna del producto.

Otro asistente específico centrado en la funcionalidad de Gestor Documental permite seleccionar un archivo del Sistema de Gestión para poder realizar consultas sobre el mismo, como solicitar un resumen del contenido, sugerencias de mejora, comparativa frente a una normativa, entre otros.

El último asistente actual es el de Compliance, centrado en realizar consultas y mejoras sobre una normativa previamente cargada en GlobalSuite®, permitiendo automatizar la identificación de aplicabilidad de ciertos requisitos, detectar brechas de cumplimiento o proponer acciones de mejora para aumentar el nivel de adecuación.

3. **¿De dónde obtiene la IA de GlobalSuite® la información o datos que utiliza para su funcionamiento y análisis?**

Hay que diferenciar el caso de uso de cada una de las funcionalidades disponibles:

Para el Asistente conversacional se emplean técnicas de Recuperación y Generación Automática de Respuestas (RAG) basadas en documentación interna elaborada por el equipo de producto.

Respecto al Recomendador de Riesgos y Controles, la información o datos de contexto son introducidos manualmente y enviados por el usuario de forma controlada. El sistema sugiere una lista de riesgos o controles que pueden ser añadidos al análisis bajo decisión del usuario. Sin embargo, es importante destacar que estos riesgos se incorporan al Análisis de Riesgos y no a los catálogos preexistentes. De esta manera, se garantiza una separación entre ambos modos de proponer riesgos y su respectiva gestión.

Asimismo, el motor para dicho Recomendador de Riesgos no almacena ni aprende de las interacciones con los usuarios. Cada solicitud que se realiza se procesa de forma independiente. De este modo, no existe retroalimentación o aprendizaje de los datos ingresados por los usuarios, y las respuestas proporcionadas no se ven influenciadas por consultas previas.

Para el asistente del Gestor Documental, la información de entrada es el documento seleccionado por el usuario, además de las consultas realizadas de forma textual. Esta información se utiliza para la consulta que se realiza en ese momento, no almacenándose en el sistema ni pudiéndose explotar en el futuro.

En el caso del asistente de Compliance, la información utilizada es la evaluación normativa sobre la que realizar consultas. De forma concreta, se obtienen los requisitos, su aplicabilidad, nivel de cumplimiento, justificación, controles asociados y no conformidades. La información se procesa y envía al acceder al asistente, y no se utiliza para el aprendizaje del mismo.

4. **En cuanto a la funcionalidad de la IA para la propuesta de controles y riesgos, ¿existe algún tipo de limitación en la cantidad de consultas que se pueden realizar o en los escenarios que pueden ser evaluados?**

En este momento, se ha implementado una limitación para esta funcionalidad, estableciendo un máximo de 60 generaciones de consultas por empresa al mes.

5. **En cuanto a la funcionalidad de la IA para los asistentes IA conversacionales, ¿existe algún tipo de limitación en la cantidad de consultas que se pueden realizar o en los escenarios que pueden ser evaluados?**

El servicio está limitado a 1.5M de tokens (cantidad de información que mide el motor de IA en cada procesamiento). Estos tokens se van consumiendo en base a preguntas y respuestas donde aproximadamente se pueden contar con 450 preguntas y respuestas. Este método de tokens por pregunta no es un procedimiento exacto por lo que dependerá del tamaño de las preguntas y el tamaño de las respuestas.

Para el asistente del Gestor Documental, existe la misma limitación del servicio de consumo de 1.5M de tokens mensual, que de manera aproximada permite el análisis y consulta de entre 100 y 150 documentos de 20 páginas.

Y en el caso del asistente de Compliance, la limitación mensual de 1.5M de tokens, aplicados tanto en las entradas (preguntas e información de contexto) y en las salidas (respuesta del asistente) computan de la misma forma.

6. **¿Se informa al usuario de manera clara sobre el uso de la Inteligencia Artificial en GlobalSuite®?**

En virtud del principio de transparencia, se comunica al usuario que toda funcionalidad de GlobalSuite® que haga uso de la Inteligencia Artificial, será informada mediante un aviso específico de uso de IA.  
Asimismo, dicho uso ya se encuentra regulado en las condiciones de contratación, donde se establece de manera clara y detallada el alcance y la naturaleza de la utilización de la misma.
