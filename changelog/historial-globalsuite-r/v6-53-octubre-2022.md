# v6.53 (Octubre 2022)

### Nuevas funcionalidades y mejoras generales de GlobalSuite® GRC

 - Mejoras de gestión de **Planes de Tratamiento**: Dentro de la opción de Gestión de Riesgos, en el apartado de [Seguimiento del Plan de Tratamiento](https://help.globalsuite.es/display/GlobalSUITEes/Seguimiento+del+Plan+de+Tratamiento) se ha incluido la posibilidad de mantener las acciones asociadas a los Planes de Tratamiento al implantarlos.

* A partir de ahora, al Implantar los Planes de Tratamiento completados, se podrá decidir si se quieren eliminar las acciones que incluye cada Plan o conservarlas.
* Estos planes de tratamiento pasarán a gestionares como controles implantados desde Gestión de Controles, conservando las acciones realizadas.

- Mejoras internas y resolución de errores.

### Nuevas funcionalidades y mejoras generales de GlobalSuite® Continuity

- Ampliación en el informe de **BIAs Consolidados**: Se ha reestructurado la información del informe que se descarga en la vista principal de BIAs Consolidados de los Procesos, para incorporar la posibilidad de exportar información adicional de los BIA realizados.

* El informe con la información de los BIAs realizados, pasa a generarse en formato csv en vez de en formato .xlsx. Este formato CSV es un estándar que permite la explotación y volcado de la información de riesgos en otros sistemas, facilitando la interconexión y explotación de las mismas.
* El informe con la información de los BIAs, agrupado en un archivo .zip, un informe CSV para cada una de las preguntas personalizables de tipo Tabla, o Tabla Elementos (que estén configuradas en Administración > Continuidad de Negocio > [Configuración BIA](https://help.globalsuite.es/pages/viewpage.action?pageId=36178118))
* Se incorpora la información de la valoración de Impactos (cualitativos y cuantitativos) para todos los BIAs

 - Mejoras en la **consolidación de BIAs**: Desde esta versión se incluyen varias mejoras y automatizaciones para facilitar el volcado de información de BIAs Individuales al  [BIA Consolidado](https://help.globalsuite.es/display/GlobalSUITEes/BIAs+Consolidados) del Proceso de Negocio, y al Inventario.

* Cuando se consolide el BIA final de un Proceso a partir de un BIA Individual se realizará una copia de toda la información del BIA seleccionado, incluyendo la valoración de Impacto en el Negocio, MTPD, RTO y preguntas personalizadas.
* Las dimensiones valoradas para el Proceso de Negocio se aplicarán al mismo en el Inventario de forma definitiva.
* Además, los elementos incluidos en las preguntas de tipo Tabla Elementos, se consolidarán en el Inventario y se incluirán bajo el Proceso de Negocio en el [Árbol de Elementos](https://help.globalsuite.es/pages/viewpage.action?pageId=36177997).  
  NOTA: Si algún elemento coincidente ya existe en el Inventario no se volcará, y se podrá consultar los resultados de la consolidación en un informe generado.

**Resumen de nuevas funcionalidades versiones v6.51 a v6.53**

En el siguiente vídeo podrá ver una explicación de las novedades incorporadas en las últimas versiones de GlobalSuite®.

![](../.gitbook/assets/260473655-changelog-v6-50-v6-53-continuidad-de-negocio.mp4)

## Vídeos

{% file src="../.gitbook/assets/260473655-changelog-v6-50-v6-53-continuidad-de-negocio.mp4" %}
Changelog v6.50 - v6.53 Continuidad de Negocio.mp4
{% endfile %}
