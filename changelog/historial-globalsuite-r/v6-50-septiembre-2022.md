# v6.50 (Septiembre 2022)

### Nuevas funcionalidades y mejoras generales de GlobalSuite® GRC

 - Mejoras de seguridad y parametrización en los **Workflows de Ticketing**: Se ha incluido la posibilidad de marcar como **Sólo Lectura** los bloques de campos de un ticket, para cada estado del [Workflow](https://help.globalsuite.es/display/GlobalSUITEes/Workflow+Incidencias).

* Si en la configuración del workflow, para un estado se marca como Sólo Lectura un apartado del formulario del ticket, los responsables del ticket podrán ver los campos de ese apartado pero no podrán modificarlos.
* Estos campos se podrán descargar en el informe .docx del ticket.
* Se podrá seguir configurando el ocultar un apartado para un estado del flujo, en cuyo caso los campos no serán visibles ni editables.

- Mejoras internas y resolución de errores.

### Nuevas funcionalidades y mejoras generales de GlobalSuite® Continuity

- Automatización y ampliación de la **consolidación** de **BIAs**: Se ha ampliado la funcionalidad para consolidar un [BIA Consolidado](https://help.globalsuite.es/display/GlobalSUITEes/BIAs+Consolidados) de un proceso de negocio a partir de un BIA Individual.

* En caso de que se consolide el BIA Consolidado de un proceso a partir de un único BIA, además de la valoración de impactos por tiempo, se copiarán el resto de campos, incluyendo MTPD, RTO, RPO, valoración de dimensiones y las preguntas personalizadas que estén configuradas en Administración > Continuidad > [Configuración BIA](https://help.globalsuite.es/pages/viewpage.action?pageId=36178118).
* Además, en el caso de las preguntas de tipo Tabla Elementos, los elementos identificados en estas preguntas se incluirán en el Inventario y en el árbol de elementos bajo el proceso de negocio evaluado.

- Mejoras y ampliación en el **informe**de **BIAs Individuales**: Se ha reestructurado la información del informe que se descarga en el listado principal de BIAs, para incorporar la funcionalidad

* El informe con la información de los BIAs realizados, pasa a generarse en formato csv en vez de en formato .xlsx. Este formato CSV es un estándar que permite la explotación y volcado de la información de riesgos en otros sistemas, facilitando la interconexión y explotación de las mismas.
* En próximas versiones se ampliará el informe con el resto de apartados y campos de los BIAs Individuales, y se aplicará el mismo formato para los BIAs Consolidados.

 - Posibilidad de ocultar la **criticidad** en los **BIAs**: En caso de que no se quiera utilizar la funcionalidad para obtener y calcular un valor de criticidad de los procesos (en función de la valoración de impacto), es posible desactivarla en el apartado de Configuración BIA, de Administración.

* En caso de estar deshabilitado, ya no aparecerá el campo en la tabla de impacto, ni en las distintas vistas donde se muestra actualmente. Tampoco aparecerá en los Informes del Listado de BIAs (Informe CSV) ni en los Informes de formulario de los BIAs (Informe Docx).
* Si la criticidad está habilitada, se podrá seguir obteniendo en función de los criterios de cálculo establecidos, y se visualizará en todas las partes de la herramienta

**Resumen de nuevas funcionalidades versiones v6.45 a v6.50**

En el siguiente vídeo podrá ver una explicación de las novedades incorporadas en las últimas versiones de GlobalSuite®.

![](../.gitbook/assets/260472918-changelog-v6-45-v6-50-general.mp4)

## Vídeos

{% file src="../.gitbook/assets/260472918-changelog-v6-45-v6-50-general.mp4" %}
Changelog v6.45 - v6.50 General.mp4
{% endfile %}
