# Correctivas y Preventivas

En cuanto a la gestión de Acciones Correctivas y Preventivas, GlobalSUITE dispone de una opción con la que poder registrar, tratar y almacenar todo este tipo de acciones que se hagan llegar desde cualquier ámbito.

Una vez dentro de la opción de acciones correctivas y preventivas, se encontrará por defecto el listado de todas aquellas que permanecen abiertas o cerradas:

![image-20260709-133104.png](../../.gitbook/assets/266864027-image-20260709-133104.png)

* **Nuevo:** Permite generar manualmente las acciones correctivas o preventivas.

* **Eliminar:** Permite eliminar las acciones generadas.

* **Copiar:** Esta opción permite copiar una acción correctiva o preventiva que ha sido definida con anterioridad.

* **Edición Múltiple:** Esta opción aparecerá en la barra de herramientas si hay configurado para este tipo de ticket un campo de estado.   
  El proceso se realiza desde un modal: se selecciona el estado actual (origen) —acompañado de su flujo de trabajo cuando corresponda y del número de tickets que se encuentran en él— y, a continuación, el nuevo estado (destino), que el sistema propone según el flujo de trabajo configurado. También puede decidirse si se envían las notificaciones de cambio de estado, activadas por defecto.

  ![image-20260709-111848.png](../../.gitbook/assets/266864027-image-20260709-111848.png)

  Antes de ejecutar, el sistema muestra un mensaje de confirmación con el número de tickets afectados y la transición que se va a aplicar. Al confirmar, la operación se ejecuta en segundo plano —su avance puede seguirse en Procesos de trabajo—, de modo que es posible continuar trabajando mientras se completa.
* **Mostrar:** Al utilizar GlobalSUITE como base de datos de conocimientos, mediante esta opción podrá seleccionar que se muestren tan sólo aquellas no conformidades que estén abiertas, o por el contrario todas, a través del desplegable del que dispone esta opción.

  ![image-20260709-113505.png](../../.gitbook/assets/266864027-image-20260709-113505.png)

  Adicionalmente, cuando el campo **Empleado** se encuentre configurado para el tipo de ticket, estarán disponibles las opciones **Abiertos por empleados** y **Todos por empleados**, que permiten mostrar los tickets agrupados por el empleado asociado.

* **Mostrar gráficas:** Permite representar todas aquellas acciones que se han definido.

* **Descarga:** Permite descargar el listado de acciones Correctivas y Preventivas en formato Excel o CSV.  Este Informe estará disponible en [Descargas Pendientes.](https://help.globalsuite.es/display/GlobalSUITEes/.Descargas+Pendientes+vv6.53)  
  Para las descargas en formato **Excel**, el sistema podrá limitar la generación del fichero cuando la información a exportar supere las **100.000 celdas**. Este límite se calcula en función de la cantidad de registros y columnas incluidas en la descarga.

  En caso de que no sea posible generar el fichero en formato Excel, se recomienda realizar la descarga en formato **CSV**.
* **Importar:** Esta opción permite realizar una carga masiva de Acciones que se encuentran en un archivo Excel. Al pulsar el botón, la herramienta solicita un archivo en formato Excel que debe contener un conjunto de columnas con la información de las Acciones que se desean importar, no importa el orden de las columnas ya que permite seleccionar aquellas que se quieren importar.![](../../.gitbook/assets/266864027-importar-datos-5.jpg)

* [Formulario de Correctivas y Preventivas](formulario-de-correctivas-y-preventivas.md)
* [Workflow Correctivas y Preventivas](workflow-correctivas-y-preventivas.md)
