# Cómo configurar encuestas de elementos-riesgos en GlobalSuite®

{% hint style="info" %}
Este tutorial explica, paso a paso, cómo crear y configurar las \*\*encuestas de elementos-riesgos\*\* en GlobalSuite®.
En esta guía se desarrollan las fases correspondientes al \*\*modelo de encuestas\*\* y a la \*\*configuración de encuestas de elementos y riesgos\*\*, detallando el proceso de selección de metodologías, la \*\*definición de dimensiones visibles, editables y obligatorias\*\*, la asociación de elementos y riesgos del inventario y la inclusión de \*\*adjuntos\*\* con documentación de referencia. También se describe cómo habilitar estados y consolidar la información para su análisis dentro del sistema de gestión
{% endhint %}

## Fases para la realización de Encuestas de Elementos-Riesgos

En esta guía se explicarán fases 1 y 2 del transcurso de creación de una encuesta.

![image-20251211-134006.png](../../../.gitbook/assets/1400111495-image-20251211-134006.png)

## Modelos de Encuestas

GlobalSuite® permite identificar y clasificar el inventario de elementos, realizar el análisis de riesgos y evaluar los controles de la organización a través de encuestas enviadas a los distintos responsables de la organización. Para ello, en primer lugar, se debe crear el modelo de encuesta que se desea mandar. Se permite crear varios modelos y, además, se pueden configurar para poder adaptarlos a las necesidades de la organización.

Para ello, cada modelo de encuesta puede ser configurado indicando el tipo de la misma. Existen tres tipos de encuestas que se pueden considerar al crear un modelo:

* **Encuesta de Elementos:** Permite la identificación de los elementos, categorización de los mismos y su clasificación.
* **Encuesta de Riesgos:** Permite la identificación de los riesgos de cada elemento (incluidos servicios y procesos) así como la evaluación de los mismos según la metodología de la organización.
* **Encuesta de Controles:** Permite la identificación de los controles implantados en la organización así como su evaluación de madurez según la metodología correspondiente.

En esta guía se va a explicar el funcionamiento del tipo “Encuesta de Elementos-Riesgos”.

Para configurar un modelo de encuesta debe ser un usuario Administrador (Administrador Plataforma, Administrador Enterprise o Administrador Configuración), ya que se encuentra en el apartado de **Ajustes**>[**Modelos de Encuestas**](https://help.globalsuitesolutions.com/es/globalsuite/v1/modelo-encuesta-elementos-riesgos-y-controles)

![](../../../.gitbook/assets/1400111495-att-0-for-1400111495.jpeg)

En la opción se debe elegir qué tipo de modelo de encuesta se quiere crear en el botón “**Nueva Encuesta**” (en este caso, el tipo “**Elementos, Riesgos y Controles**”). Además, en esta opción se podrán eliminar modelos (botón “**Eliminar**”) y descargar un listado de los modelos configurados (botón “**Descarga**”).

En la última columna mostrará los modelos que están habilitados. Sólo se podrán crear encuestas de los modelos habilitados.

![image-20251205-130114.png](../../../.gitbook/assets/1400111495-image-20251205-130114.png)

Dentro del modelo de encuesta se permite configurar aspectos como el nombre, el departamento o la fecha de creación, así como indicar si se requiere que el modelo esté **habilitado** para su utilización y si se quiere “**Consolidar en último estado**”, es decir, que desde el último estado del flujo se pueda consolidar directamente los datos de la encuesta en el análisis definitivo.

También es posible utilizar estados en la encuesta, la utilización de estos estados permite que diferentes personas puedan rellenar o validar información introducida en estado anteriores. Se podrá pasar de un estado a otro de forma automática si se marca el indicador (check automático) y también se podría pasar a un estado anterior de la misma manera, marcando el indicador correspondiente (check vuelta atrás).

![](../../../.gitbook/assets/1400111495-att-1-for-1400111495.jpeg)

En la sección “**Tipo de Encuesta”** se debe elegir qué tipo de modelo se quiere crear. En este caso se va a seleccionar el tipo “**Encuesta de Elementos-Riesgos**”.

![](../../../.gitbook/assets/1400111495-att-2-for-1400111495.jpeg)

A continuación, se visualiza la sección “Taxonomía” (Tipos / Agrupación de Riesgos), donde se puede seleccionar su configuración. Se puede seleccionar si se quiere que sea visible y editable en la encuesta. También es posible indicar en qué orden se quiere visualizar.

![](../../../.gitbook/assets/1400111495-att-3-for-1400111495.jpeg)

En la siguiente sección “**Encuesta de Elementos**”, se muestran las dimensiones configuradas en el inventario de elementos indicando el tipo de dimensión y si ésta es manual o automática.

![](../../../.gitbook/assets/1400111495-att-4-for-1400111495.jpeg)

El usuario puede configurar las siguientes opciones de cada dimensión:

* **Visible**: permite definir si la dimensión se incluirá en la encuesta o no, pulsando sobre la celda.
* **Editable**: indica si la dimensión se podrá modificar en la encuesta, o sólo será visible en modo consulta.
* **Obligatoria**: indica la obligatoriedad de rellenar una dimensión al pasar de estado, en el caso de que se usen encuestas con estados.
* **Pregunta**: en el caso de encuestas de tipo "Formulario" (se verá más adelante), permite mostrar una pregunta explicativa, en lugar de únicamente el nombre de la dimensión.

Si se selecciona una dimensión, se permite cambiar el orden en el que va a aparecer, utilizando los botones “Subir” y “Bajar” se puede posicionar en el lugar deseado.

![image-20251205-130342.png](../../../.gitbook/assets/1400111495-image-20251205-130342.png)

Con el botón “**Actualizar Dimensiones**”, tal y como indica el mensaje en amarillo, se actualiza el listdo de las dimensiones de la metodología de elementos por si se hubieran añadido nuevas dimensiones después de la creación del modelo.

Los ajustes sobre las dimensiones anteriores que ya existían se conservan, únicamente aparecen las nuevas dimensiones que se hayan creado en la metodología de elementos para poder ser incluidas en la encuesta.

Al marcar una dimensión de tipo cualitativa, en la tabla inferior (“Niveles de Elementos”) se muestran a título informativo los niveles que tiene configurados en Ajustes>[Metodología Elementos](https://help.globalsuitesolutions.com/es/globalsuite/v1/metodologia-elementos).

![](../../../.gitbook/assets/1400111495-att-5-for-1400111495.jpeg)

En la última sección “**Encuesta de Riesgos”**, en primer lugar, se debe seleccionar qué metodología de riesgos se quiere utilizar en la encuesta. Al seleccionar la metodología se muestran las dimensiones configuradas en la misma, indicando el tipo de dimensión y si ésta es manual o automática. El usuario puede configurar las opciones al igual que con las dimensiones de los elementos.

![image-20251205-130920.png](../../../.gitbook/assets/1400111495-image-20251205-130920.png)

Al escoger al metodología se muestra un mensaje informativo indicando que se cambiaran las dimensiones por las de la metodología seleccionada.

> *«Al cambiar la metodologia se reemplazarán las dimensiones de Riesgos actuales por las de la nueva metodología seleccionada, ¿Desea Continuar?»*

En la sección “**Adjuntos**” se podrá adjuntar a la encuesta los archivos necesarios para que el receptor de la misma pueda consultar.

Las opciones disponibles son:

* **Seleccionar archivo**: permite buscar y seleccionar un fichero de nuestro explorador de archivos.
* **Adjuntar**: permite subir el archivo seleccionado.
* **Eliminar**: permite eliminar un archivo seleccionado en la tabla “Documentación Asociada”.
* **Descargar**: permite descargar el archivo seleccionado en la tabla “Documentación Asociada”.
* **Visualizar**: permite visualizar desde el navegador, el archivo seleccionado en la tabla “Documentación Asociada”. Únicamente es posible visualizar archivos con la extensión .pdf, .jpeg, .jpg, .bmp o .png.

![image-20251205-131028.png](../../../.gitbook/assets/1400111495-image-20251205-131028.png)

## Configuración de Encuestas

Una vez configurado el modelo de encuesta, éste se puede utilizar para configurar tantas encuestas como se requiera. Para ello, hay que dirigirse a la opción **Gestión>** [**Encuestas**](https://help.globalsuitesolutions.com/es/globalsuite/v1/configurar-encuestas)

![](../../../.gitbook/assets/1400111495-att-6-for-1400111495.jpeg)

Para crear la configuración de una encuesta se debe filtrar por el tipo de encuesta y posteriormente elegir el modelo deseado.

Al pulsar el botón “**Nuevo**” se creará una encuesta del tipo y modelo elegido. Si desea eliminar la configuración de una encuesta tiene que pulsar el botón “**Eliminar**”. Hay que tener en cuenta que si se elimina una Configuración, todas las encuestas creadas a partir de esta Configuración también se eliminarán.

También se permite descargar el listado de configuraciones de encuestas tanto en formato Excel como pdf.

![image-20251205-131154.png](../../../.gitbook/assets/1400111495-image-20251205-131154.png)

Al acceder a la configuración de la encuesta aparecen un conjunto de secciones que permiten su configuración.

En la primera sección, “Datos Generales Configuración”, se puede identificar el nombre de la configuración, visualizar el tipo y modelo de encuesta, cambiar la fecha y también permite activar o no el check “**Habilitado”** que permite indicar si la Configuración puede utilizarse para generar nuevas encuestas.

![](../../../.gitbook/assets/1400111495-att-7-for-1400111495.jpeg)

Si en el modelado se han incluido estados (workflow), entonces en la configuración aparece también la sección de  “Estados” para poder asignar un responsable a cada estado:

![image-20251205-132822.png](../../../.gitbook/assets/1400111495-image-20251205-132822.png)

En la sección “Configuración Riesgos”, aparece la información relacionada con los Elementos y los Riesgos. Se debe seleccionar el análisis de riesgos se quiere utilizar en la encuesta. Al seleccionar el análisis, se muestra el catálogo de riesgos asociado por si se quiere consultar.

![image-20251205-132858.png](../../../.gitbook/assets/1400111495-image-20251205-132858.png)

Una vez seleccionado el análisis, se deben escoger los elementos, pulsando el botón “Añadir Elementos”, de los cuales se quiera valorar los riesgos que tienen asociados.

Cuando se selecciona el elemento añadido, en la parte inferior , se muestran los riesgos asociados. Si se quieren incluir estos riesgos en la encuesta o no, se indica marcando o desmarcando el check de la izquierda.

![image-20251205-132939.png](../../../.gitbook/assets/1400111495-image-20251205-132939.png)

Una vez que se han completado todos los pasos del formulario, se pulsa el botón “Guardar” y ya está lista la configuración para poder ser utilizada.

Desde la sección “**Adjuntos**”, se podrá añadir documentos específicos a la propia configuración. A su vez, se podrá visualizar y/o gestionar los documentos heredados provenientes del modelo de encuesta.

![image-20251205-133012.png](../../../.gitbook/assets/1400111495-image-20251205-133012.png)
