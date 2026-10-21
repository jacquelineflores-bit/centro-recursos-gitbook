# Requerimientos

En cuanto a los tickets de requerimientos, GlobalSUITE® dispone de una apartado específico con la que poder registrar, gestionar y almacenar todo tipo de requerimientos que se hagan llegar desde cualquier ámbito, incluidos los trabajos de auditoría ejecutados.

Una vez dentro de la opción Requerimientos, se encontrará por defecto el listado de todas aquellas que permanecen registradas, implementándose, rechazadas o cerradas:

* ![image-20260709-152458.png](../../.gitbook/assets/266863647-image-20260709-152458.png)

  **Nuevo:** Permite generar manualmente nuevos requerimientos.
* **Eliminar:** Permite eliminar los requerimientos generados.
* **Copiar:** Esta opción permite duplicar un requerimiento seleccionado que ha sido definido con anterioridad, con toda la información que contiene.
* **Edición Múltiple:** Esta opción aparecerá en la barra de herramientas si hay configurado para este tipo de ticket un campo de estado.   
  El proceso se realiza desde un modal: se selecciona el estado actual (origen) —acompañado de su flujo de trabajo cuando corresponda y del número de tickets que se encuentran en él— y, a continuación, el nuevo estado (destino), que el sistema propone según el flujo de trabajo configurado. También puede decidirse si se envían las notificaciones de cambio de estado, activadas por defecto.

  ![image-20260709-111848.png](../../.gitbook/assets/266863647-image-20260709-111848.png)

  Antes de ejecutar, el sistema muestra un mensaje de confirmación con el número de tickets afectados y la transición que se va a aplicar. Al confirmar, la operación se ejecuta en segundo plano —su avance puede seguirse en Procesos de trabajo—, de modo que es posible continuar trabajando mientras se completa.
* **Mostrar:** Al utilizar GlobalSUITE como base de datos de conocimientos, mediante esta opción podrá seleccionar que se muestren tan sólo aquellas no conformidades que estén abiertas, o por el contrario todas, a través del desplegable del que dispone esta opción.

  ![image-20260709-113505.png](../../.gitbook/assets/266863647-image-20260709-113505.png)

  Adicionalmente, cuando el campo **Empleado** se encuentre configurado para el tipo de ticket, estarán disponibles las opciones **Abiertos por empleados** y **Todos por empleados**, que permiten mostrar los tickets agrupados por el empleado asociado.

* **Descarga:** Permite descargar el listado de No Conformidades representados en formato Excel o CSV.  Este Informe estará disponible en [Descargas Pendientes.](https://help.globalsuite.es/display/GlobalSUITEes/.Descargas+Pendientes+vv6.53)  
  Para las descargas en formato **Excel**, el sistema podrá limitar la generación del fichero cuando la información a exportar supere las **100.000 celdas**. Este límite se calcula en función de la cantidad de registros y columnas incluidas en la descarga.

  En caso de que no sea posible generar el fichero en formato Excel, se recomienda realizar la descarga en formato **CSV**.

* [Formulario de Requerimientos](formulario-de-requerimientos.md)
* [Workflow Requerimientos](workflow-requerimientos.md)
