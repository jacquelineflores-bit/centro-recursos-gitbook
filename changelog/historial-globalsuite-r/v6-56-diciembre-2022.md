# v6.56 (Diciembre 2022)

### Nuevas funcionalidades y mejoras generales de GlobalSuite® GRC

 - Mejoras de **usabilidad** en el nuevo módulo de **Encuestas de Elementos, Riesgos y Controles**: Se ha incorporado una mejora de usabilidad para poder consultar, editar y revisar los campos textuales de las encuestas ERC, en caso de que incluyan textos extensos.

* En las tablas de Elementos, Riesgos y Controles, se podrá consultar el detalle de las dimensiones textuales en una ventana externa para facilitar su lectura (aparece un campo (info.) en cada celda para ver el detalle)
* En los formularios o fichas, los cuadros de texto se expandirán para visualizar todo el contenido de cada campo sin necesidad de una barra de desplazamiento dentro del campo.

 - Ampliación de **Importación de Riesgos**: Se ha incorporado la posibilidad de importar la Agrupación o Tipo de Riesgo que se puede asociar a las amenazas o riesgos definidos en el análisis, para poder categorizarlas y obtener resultados agregados.

* Cuando se disponga del módulo de **Data Import** en la opción de Análisis de Riesgos, se podrá realizar una importación de los Tipos de Riesgo de cada uno, en una segunda hoja del archivo para importar, pudiendo asociar varios tipos o agrupaciones de riesgo a cada uno.
* El Modelo de Importación en Excel con la estructura adicional se puede descargar desde la [Tabla de Elementos](https://help.globalsuite.es/display/GlobalSUITEes/Tabla+de+Elementos)

 - Campo **Id Externo del Control** editable: Hasta ahora el campo Id Externo, disponible en la ficha de controles del análisis de riesgos, únicamente era posible cargarlo mediante importación de controles en Excel

* El control será editable tanto en la tabla principal como en el formulario de los controles, permitiendo utilizar este campo sin necesidad de importarlo, si este está visible (la configuración se realiza en [Metodología de Elementos](https://help.globalsuite.es/pages/viewpage.action?pageId=36178138) > Ficha de Control).
* El campo se incluirá en los informes que se tengan para estos campos.

 - Mejora de optimización de **Históricos**: En el apartado de [Históricos](https://help.globalsuite.es/pages/viewpage.action?pageId=36178018) de análisis, se ha optimizado la vista para consultar los elementos del Inventario de un histórico para una fecha concreta

* Reestructuración de la vista de Inventario de Elementos para un histórico, pudiendo consultar la información de manera más eficiente.
* Optimización de la descarga del Informe:

  * La descarga ha pasado a generarse en segundo plano para evitar esperas del usuario. Una vez generado, podrá obtenerlo en el apartado[Descargas Pendientes](https://help.globalsuite.es/display/GlobalSUITEes/Descargas+Pendientes)
  * El archivo generado ha pasado de formato Excel a formato CSV para facilitar su explotación posterior.

- Mejoras internas y resolución de errores.

### Nuevas funcionalidades y mejoras generales de GlobalSuite® Continuity

- Mejora en las **encuestas de BIA**: A partir de ahora, será posible configurar los Modelos de Encuesta de BIA (tanto [BIA por Tiempo](https://help.globalsuite.es/display/GlobalSUITEes/Modelo+Encuesta+BIA+por+Tiempo), como [BIA por Impacto](https://help.globalsuite.es/display/GlobalSUITEes/Modelo+Encuesta+BIA+por+Impacto)) para no incluir los campos de MTPD y valoración de Impacto, pudiendo crear encuestas para recabar otra información de los procesos fuera de estos campos.

* Al igual que el resto de campos del BIA, se podrá ocultar de la plantilla o modelo de encuesta tanto el MTPD como las tablas de Impacto (cualitativo, cuantitativo, en período crítico) para no enviarlo en las encuestas.
* Esta información no se consolidará en el BIA en caso de no estar incluida en la encuesta.
