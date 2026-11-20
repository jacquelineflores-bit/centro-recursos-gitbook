# Tipos de campos en los tickets de GlobalSuite®

{% hint style="info" %}
En este artículo trataremos los distintos tipos de campos que se pueden configurar en los tickets de GlobalSuite®, y cómo cada uno permite adaptar los formularios a las necesidades de registro y gestión de incidencias, peticiones o eventos.
{% endhint %}

En GlobalSuite®, los tickets pueden personalizarse mediante diferentes tipos de campos que definen la información a registrar en cada formulario. Estos campos permiten capturar textos, fechas, selecciones, relaciones con otros elementos del sistema o datos calculados automáticamente.  
A continuación, se detallan todos los tipos de campo disponibles y su comportamiento tanto en el área de **Ajustes** como en la vista de uso de **GlobalSuite®**, facilitando la configuración y el diseño de formularios adaptados a cada proceso de gestión.

A continuación se presenta el listado completo de tipos de campo disponibles, que podrás consultar en detalle más abajo en esta misma guía.

|  |  |  |
| --- | --- | --- |
| [INPUT](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#INPUT) | [STATUS](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#STATUS) | [CMDB](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#CMDB) |
| [TXT](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#TXT) | [REFERENCES](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#REFERENCES) | [SERVICES](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#SERVICES) |
| [DATE](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#DATE) | [EMPLOYEES](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#EMPLOYEES) | [ORGANIZATIONAL STRUCTURE](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#ORGANIZATIONAL-STRUCTURE) |
| [CHECK](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#CHECK) | [INVOLVED AREAS](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#INVOLVED-AREAS) | [ID](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#ID) |
| [SELECT](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#SELECT) | [CLIENT](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#CLIENT) | [WORKFLOW](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#WORKFLOW) |
| [SELECTED-NESTED](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#SELECTED-NESTED) | [MANAGERS](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#MANAGERS) | [SIMULATION RISK](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#SIMULATION-RISK) |
| [TICKETS-INPUTS](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#TICKETS-INPUTS) | [RISK](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#RISKS) | [TYPE](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#TYPE) |
| [TICKETS-OUTPUTS](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#TICKETS-OUTPUTS) | [TYPES FOLLOW-UP](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#TYPES-FOLLOW-UP) | [OWNER](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#OWNER) |
| [NUM](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#NUM) | [EVIDENCES](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#EVIDENCES) | [PROCESSES](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#PROCESSES) |
| [SUPERVISOR](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#SUPERVISOR) | [DELIVERABLES](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#DELIVERABLES) | [THREATS](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#THREATS) |
| [URGENCY](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#URGENCY) | [SUPPLIERS](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#SUPPLIER) | [AUDIT-WORKS](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#AUDIT-WORKS) |
| [IMPACT](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#IMPACT) | [INCIDENT MANAGEMENT PLANS](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#INCIDENT-MANAGEMENT-PLANS) |  |
| [PRIORITY](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#PRIORITY) | [FOLLOWS UP](tipos-de-campos-en-los-tickets-de-globalsuite-r.md#FOLLOWS-UP) |  |

### INPUT

{% hint style="info" %}
Permite añadir al ticket un campo de texto, este texto debe tener una longitud corta - media.
{% endhint %}

* **Nombre:** Etiqueta del campo que se mostrará en el formulario.
* **Alias informes:** Identificador único del campo (alfanumérico, máx. 5) para usar en plantillas de informes de Tickets.
* **Obligatorio:** Marca este campo como imprescindible. Sin completarlo no podrás crear ni actualizar el ticket.
* **E-mail:** Activado indica que el campo introducido debe ser formato de correo. Ej: [name@mail.com](mailto:name@mail.com)
* **Ayuda:** El texto ingresado aquí se mostrará como guía para completar el campo.
* **Orden:** Define la posición en la que el campo aparecerá dentro de la sección.
* **Cambiar sección:** Indica la sección actual del campo y permite moverlo a otra. Al hacerlo, el campo se ubicará al final de la nueva sección.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-101817.png | image-20251215-101833.png |

### TXT

{% hint style="info" %}
Permite añadir al ticket un campo de texto, el campo se irá adaptando al tamaño del texto insertado.
{% endhint %}

* **Nombre:** Etiqueta del campo que se mostrará en el formulario.
* **Alias informes:** Identificador único del campo (alfanumérico, máx. 5) para usar en plantillas de informes de Tickets.
* **Obligatorio:** Marca este campo como imprescindible. Sin completarlo no podrás crear ni actualizar el ticket.
* **Ayuda:** El texto ingresado aquí se mostrará como guía para completar el campo.
* **Orden:** Define la posición en la que el campo aparecerá dentro de la sección.
* **Cambiar sección:** Indica la sección actual del campo y permite moverlo a otra. Al hacerlo, el campo se ubicará al final de la nueva sección.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-101758.png | image-20251215-101744.png |

### DATE

{% hint style="info" %}
Permite añadir al ticket un campo de fecha para registros de tiempo.
{% endhint %}

* **Nombre:** Etiqueta del campo que se mostrará en el formulario.
* **Alias informes:** Identificador único del campo (alfanumérico, máx. 5) para usar en plantillas de informes de Tickets.
* **Obligatorio:** Marca este campo como imprescindible. Sin completarlo no podrás crear ni actualizar el ticket.
* **Tipo de Fecha**: Permite configurar diferentes referencias de fecha como: inicial (se puede utilizar en gráficas y para envío de alertas), final, inicio previsto y fin previsto (estos últimos 3 tipos se puede utilizar en gráficas).
* **Automático:** Permite indicar si se completa automaticamente, al marcarlo permite seleccionar con cuál fecha, las opciones disponibles son: Creación, Ultima modificación, Cierre, Reapertura y Fecha calculada

  * **Fecha calculada:** Permite calcular la fecha a partir de otra fecha del propio ticket. Al seleccionarla se configura la fórmula: una fecha base (otro campo de fecha del mismo tipo de ticket), una cantidad (número entero) y una unidad (días o meses). El campo resultante no es editable y se recalcula automáticamente al informar o modificar la fecha base.

    El botón Calcular Fecha aplica la fórmula a los tickets ya existentes, recalculando sus fechas en segundo plano, con opción de incluir los tickets cerrados.
* **Editable**: Activando este check, permitirá al usuario editar la fecha de este campo.
* **Alertar plazo cumplido:** Activando este check, muestra la fecha en rojo en el listado de tickets, alertando con esto que la fecha del día de hoy es posterior a la fecha registrada en este campo.
* **Configuración de Reglas de Fechas:** Permite definir validaciones sobre este campo. Por ejemplo, que la Fecha de fin no pueda ser anterior a la Fecha de inicio.
* **Ayuda:** El texto ingresado aquí se mostrará como guía para completar el campo.
* **Orden:** Define la posición en la que el campo aparecerá dentro de la sección.
* **Cambiar sección:** Indica la sección actual del campo y permite moverlo a otra. Al hacerlo, el campo se ubicará al final de la nueva sección.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-102548.png | image-20251215-102350.png |

### CHECK

{% hint style="info" %}
Permite añadir al ticket un campo de Check, que dará la posibilidad de completar el formulario de tickets con preguntas de respuesta rápida Sí/No (check activado).
{% endhint %}

* **Nombre:** El nombre del campo, con el cual se mostrará en el formulario.
* **Alias informes:** Identificador único del campo (alfanumérico, máx. 5) para usar en plantillas de informes de Tickets.
* **Ayuda:** El texto ingresado aquí se mostrará como guía para completar el campo.
* **Orden:** Define la posición en la que el campo aparecerá dentro de la sección.
* **Cambiar sección:** Indica la sección actual del campo y permite moverlo a otra. Al hacerlo, el campo se ubicará al final de la nueva sección.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-102748.png | image-20251215-103116.png |

### SELECT

{% hint style="info" %}
Permite añadir al ticket un campo de tipo selección, en el que se dispondrá de diferentes opciones a elegir.
{% endhint %}

* **Nombre:** El nombre del campo, con el cual se mostrará en el formulario.
* **Alias informes:** Identificador único del campo (alfanumérico, máx. 5) para usar en plantillas de informes de Tickets.
* **Obligatorio:** Marca este campo como imprescindible. Sin completarlo no podrás crear ni actualizar el ticket.
* **Ayuda:** El texto ingresado aquí se mostrará como guía para completar el campo.
* **Orden:** Define la posición en la que el campo aparecerá dentro de la sección.
* **Cambiar sección:** Indica la sección actual del campo y permite moverlo a otra. Al hacerlo, el campo se ubicará al final de la nueva sección.
* **Opciones:** Tabla donde se pueden añadir las diferentes opciones que van a estar disponibles en el select. También se puede añadir una descripción concreta para cada una de las opciones añadidas y un valor numérico para cada una.

| **Vista en Ajustes** |
| --- |
| image-20251215-103930.png |
| **Vista en GlobalSuite®** |
| image-20251215-103549.png |

### SELECTED-NESTED

{% hint style="info" %}
Permite añadir un campo Select Anidado, que da la posibilidad de añadir un select dependiente de otro select.
{% endhint %}

* **Nombre:** El nombre del campo, con el cual se mostrará en el formulario.
* **Alias informes:** Identificador único del campo (alfanumérico, máx. 5) para usar en plantillas de informes de Tickets.
* **Obligatorio:** Marca este campo como imprescindible. Sin completarlo no podrás crear ni actualizar el ticket.
* **Ayuda:** El texto ingresado aquí se mostrará como guía para completar el campo.
* **Orden:** Define la posición en la que el campo aparecerá dentro de la sección.
* **Cambiar sección:** Indica la sección actual del campo y permite moverlo a otra. Al hacerlo, el campo se ubicará al final de la nueva sección.
* **Mostrar descripción:** Check que muestra la descripción del campo si se activa y se ha rellenado.
* **Opciones**: Diferentes opciones a elegir que se pueden modificar.
* **Subopciones**: Seleccionando alguna opción se añaden en la segunda tabla por cada opción.

| **Vista en Ajustes** |
| --- |
| image-20251215-121629.png |
| **Vista en GlobalSuite®** |
| image-20251215-123912.png |

### TICKETS-INPUTS

{% hint style="info" %}
Permite asociar Tickets existentes o nuevos a cada ticket.
{% endhint %}

* **Nombre:** El nombre del campo, con el cual se mostrará en el formulario.
* **Alias informes:** Identificador único del campo (alfanumérico, máx. 5) para usar en plantillas de informes de Tickets.
* **Ayuda:** El texto ingresado aquí se mostrará como guía para completar el campo.
* **Orden:** Define la posición en la que el campo aparecerá dentro de la sección.
* **Cambiar sección:** Indica la sección actual del campo y permite moverlo a otra. Al hacerlo, el campo se ubicará al final de la nueva sección.
* **En GlobalSuite®**

  * **Añadir**: Permite incluir nuevos tickets en el ticket creado desde esta opción.
  * **Desasociar**: Permite desasociar tickets en el ticket
  * **Asociar Existentes:** Permite asociar tickets ya creados

{% hint style="info" %}
La parametrización de los campos mostrados en los tickets con este campo se realiza en la opción "Pantalla Común“.
{% endhint %}

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-132117.png | image-20251215-131853.png |

### TICKETS-OUTPUTS

* **Añadir:** Permite incluir nuevos tickets en el ticket creado desde esta opción.
* **Desasociar**: Permite desasociar tickets en el ticket
* **Asociar Existentes**: Permite asociar tickets ya creados

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-132408.png | image-20251215-133340.png |

{% hint style="info" %}
\*\*NOTA\*\*: La parametrización de los campos mostrados en los tickets con este campo se realiza en la opción "Pantalla Común“.
{% endhint %}

### NUM

Campo de tipo **numérico** que restringe la entrada a solo números.

* **Mínimo/Máximo**: Permite limitar el rango de inserción.
* **Máximo de decimales**: Delimita la cantidad de decimales que se permite introducir.
* **Automático**: Si se activa, permite introducir fórmulas utilizando los campos numéricos.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-133655.png | image-20251215-134135.png |

#### CONFIGURAR FÓRMULA

Campo de tipo numérico con fórmula automática. Se debe pulsar el botón configurar.

* **Campos numéricos:** Permite operaciones matemáticas con los campos de tipo NUM.
* **Validar fórmula**: Tras configurar la fórmula se debe validar sin fallos para luego poder guardarla.
* **Fórmula Condicional**: Permite utilizar condicionales (IF) para comparar campos de forma avanzada.

| **Vista en Ajustes** |
| --- |
| image-20251215-134851.png |
| **Vista en GlobalSuite®** |
| image-20251215-135306.png |

### SUPERVISOR

Permite añadir un campo de tipo supervisor, que permite relacionar un empleado con el ticket, además, dará la posibilidad de mandar alertas a este empleado relacionado.

* **Obligatorio**: Este check marcado obliga a que se deba rellenar el campo.

| **Vista en Ajustes** |
| --- |
| image-20251215-135513.png |
| **Vista en GlobalSuite®** |
| image-20251215-140224.png |

### URGENCY

Permite añadir un campo de tipo Select, con opciones configurables para valorar la urgencia.

* **Urgencia**: Tabla de configuración de las diferentes opciones del campo, sus valores y descripciones.

{% hint style="info" %}
\*\*NOTA\*\*: Relacionada con campos Impact y Priority.
{% endhint %}

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-140945.png | image-20251215-141142.png |

### IMPACT

Permite añadir un campo de tipo Select, con opciones configurables para valorar el impacto.

* **Impacto**: Tabla de configuración de las diferentes opciones del campo, sus valores y descripciones.

{% hint style="info" %}
\*\*NOTA\*\*: Relacionado con los campos Urgency y Priority.
{% endhint %}

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-141615.png | image-20251215-141343.png |

### PRIORITY

Añade una valoración multiplicando los campos Impact y Urgency. Permitirá configurar una serie de valores dependientes de unos rangos de valoración, para definir que resultado de prioridad deseado.

* **Prioridad**: Se configuran los niveles, con su rango máximo y mínimo de valoración y las descripciones en cada caso. Además un color paca cado nivel.

{% hint style="info" %}
\*\*NOTA\*\*: Relacionada con campos Impact y Urgency, será una media (sumatorio dividido entre 2) de los valores de los 2 campos.
{% endhint %}

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-141807.png | image-20251215-141944.png |

### STATUS

Permite añadir un campo de selección con los diferentes posibles estados de un ticket. Los estados pueden ser configurados tanto en nombre, descripción como tipo.

* **Estados**: Tabla de configuración de los diferentes estados del ticket.
* **Tipos Estado**: Pueden ser de 3 tipos,

  * Inicial (es único)
  * Intermedio (múltiples)
  * Final (múltiples, bloquea estado a solo lectura y permite reabrirse mandando notificación).

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-151924.png | image-20251215-151902.png |

### REFERENCES

Permite añadir una tabla de registros, que serán referencias con una link o URL a una página web.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-152937.png | image-20251215-153753.png |

### EMPLOYEES

Permite añadir una tabla de registros de empleados de la herramienta, que se asociarán al ticket.

* **¿Mostrar horas dedicadas?**: Permite introducir horas que cada empleado haya dedicado.
* **Notificar vía e-mail**: Permite enviar notificaciones al empleado vía email cuando ha sido añadido al ticket. Además se podrá alertar a este empleado de acciones de Creación, Modificación y Cierre de Tickets

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-154401.png | image-20251215-154212.png |

### INVOLVED AREAS

Permite añadir una tabla de registros, estos registros serán Áreas de la empresa que estarán relacionadas con el ticket. Se pueden configurar en la parte de Ajustes > Configuración > General en el apartado [**Propiedades Configuración de Gestión**](https://help.globalsuitesolutions.com/es/globalsuite/v1/propiedades-configuracion-de-gestion) > Áreas afectadas.

* **Asociar**: Permite asociar áreas afectadas al ticket.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-155143.png | image-20251215-155347.png |

### CLIENT

Permite añadir un conjunto de campos de contacto con diferentes variantes. Se podrá asociar directamente algún nombre, e-mail de contacto o utilizar alguno existente en la opción de “[**Relaciones con el Negocio**](https://help.globalsuitesolutions.com/es/globalsuite/v1/relaciones-con-el-negocio).”

* Conjunto de campos Cliente: Aquellos que estén rellenados aparecerán en el ticket.

{% hint style="info" %}
\*\*NOTA\*\*: además de los que se ven en la imagen, existe E-mail, Alertar email y Contacto/Grupo.
{% endhint %}

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-165356.png | image-20251215-164715.png |

### MANAGERS

Permite añadir una tabla de responsables superiores, estos registros serán roles con empleado/usuario de entidades superiores. Por tanto, la tabla aparecerá en el formulario, solo si está en una entidad hija.

Para usar este campo se deben usar entidades.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-165813.png | image-20251215-171043.png |

### RISKS

Permite añadir una tabla de registros, que serán riesgos creados en la parte de configuración en la tabla de Categoría Riesgos (Ajustes> [Metodologías Elementos](https://help.globalsuitesolutions.com/es/globalsuite/v1/metodologia-elementos)).

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-171426.png | image-20251215-171549.png |

### TYPES FOLLOW-UP

Permite añadir una tabla de registros, estos registros serán seguimientos del ticket, donde se podrán añadir una fecha del mismo, un tipo y unas observaciones del seguimiento.

* **Nuevo**: Crea un nuevo seguimiento.

| **Vista en Ajustes** |
| --- |
| image-20251215-171944.png |
| **Vista en GlobalSuite®** |
| image-20251215-172330.png |

### EVIDENCES

Permite añadir una tabla de registros, estos registros serán de documentación asociada al ticket, permitirá adjuntar documentos, añadirles una fecha y una serie de descripciones para tener un control total de las evidencias registradas.

* **Evidencias**: Permite adjuntar archivos de evidencia al ticket.

{% hint style="info" %}
\*\*NOTA:\*\* Solo podrá ser añadido una vez
{% endhint %}

| **Vista en Ajustes** |
| --- |
| image-20251215-172746.png |
| **Vista en GlobalSuite®** |
| image-20251215-172958.png |

### DELIVERABLES

Permite añadir una tabla de registros, estos registros serán de documentación asociada al ticket, permitirá adjuntar documentos, añadirles una fecha y una serie de descripciones para tener un control total de los entregables.

* **Adjuntar**: Permite adjuntar archivos de evidencia al ticket.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251215-173558.png | image-20251215-173358.png |

## SUPPLIER

Permite asociar al ticket un proveedor del listado que se tenga cargado en la opción de Proveedores. Se podrá añadir más de un campo de este tipo, para poder registrar los proveedores que estén relacionados con el ticket.

| **Vista en Ajustes** |
| --- |
| image-20251220-122659.png |
| **Vista en GlobalSuite®** |
| image-20251220-123641.png |

## INCIDENT MANAGEMENT PLANS

Permite añadir una tabla de registros, estos registros serán un plan de gestión de incidentes. Permitirá asociar al ticket adicionalmente una serie de impactos y niveles.

* **Impactos/Niveles**: Se pueden añadir valoraciones para formar el Plan para luego poder activarlo.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251220-130813.png | image-20251220-131141.png |

## FOLLOWS UP

Permite añadir una tabla de registros, estos registros serán seguimientos del ticket, donde quedará constancia de que usuario realizó el seguimiento, con una fecha y su descripción. También dará la posibilidad de enviar el seguimiento a un listado de correos que este definido por ";".

* **Enviar Email:** Para enviar emails de seguimiento tras haber puesto el correo en el espacio en blanco.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251220-131432.png | image-20251220-131828.png |

## CMDB

Este campo permite asociar elementos, que estarán relacionados con el CMDB a través de el ticket. Permitirá asociar al ticket una serie de elementos y almacenar el historial de los mismos.

* **Crear L.R.**: Se pueden crear historiales (líneas de referencia) de los elementos asociados.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251220-132602.png | image-20251220-132542.png |

## SERVICES

Permite añadir una tabla de registros, estos registros serán servicios definidos en el Catálogo de Servicios de la pestaña Inicio. Se podrá asociar con esta tabla, un ticket con los servicios a los que afecta o está relacionado.

* **Añadir/Eliminar:** Se añaden o eliminan servicios de la lista predefinida al ticket relacionados con él.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251220-132737.png | image-20251220-133817.png |

## ORGANIZATIONAL STRUCTURE

Permite añadir una tabla de registros, que son parte del árbol de la Estructura Organizativa definida en la opción de **Inicio>**[**Estructura Organizativa**](https://help.globalsuitesolutions.com/es/globalsuite/v1/estructura-organizativa)**.**

Se puede asociar con esta tabla, un ticket con el área de la empresa a la que afecta o está relacionado.

* **Añadir E.O.**: Permite añadir Estructura predefinidas.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251220-134124.png | image-20251220-134451.png |

## ID

Permite añadir un campo de texto que generará una numeración única para cada uno de los tickets.

* **Inicio Secuencia:** Permite definir si la secuencia es Automática donde se generará un número de forma automática, o Secuencia donde se definirá el patrón de numeración por el que va a comenzar.
* **Editable**: Permite definir si una vez creado el ticket con una numeración única, ésta podrá modificarse.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251220-134945.png | image-20251220-134959.png |

## WORKFLOW

Permite añadir un campo de selección donde aparecerán los flujos de trabajo que se tengan definidos para cada uno de los tickets. Una vez se seleccione un Workflow para el ticket, en el campo estado se modificarán los diferentes estados por defecto, por los estados del Workflow seleccionado.

{% hint style="info" %}
\*\*NOTA\*\*: Para que aparezca la configuración del WF, es necesario añadir antes el campo "STATUS“ y el campo “WORKFLOW”.
{% endhint %}

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251220-140252.png | image-20251220-140959.png |

## SIMULATION RISK

Permite añadir una tabla de registros, donde se podrá definir para una incidencia o ticket concreto, como afecta a los elementos de un análisis de riesgo concreto. Se podrá realizar la simulación y posterior incorporación al análisis para que afecte a los valores generales.

* **Asociar/Desasociar**: Permite asociar/desasociar riesgos.
* **Restaurar riesgo**: Permite restaurar los valores del riesgo a los del Análisis de Riesgos.

| **Vista en Ajustes** |
| --- |
| image-20251220-141135.png |
| **Vista en GlobalSuite®** |
| image-20251220-142012.png |

## TYPE

Permite añadir un campo de selección donde nos aparecerán todos los tipos de tickets del SG, con este campo, se podrán categorizar los tickets según hayan se registrado, para “transformar” posteriormente este ticket a “No conformidad”, “Acción Correctiva”, “Incidencia”, etc.

{% hint style="info" %}
\*\*NOTA\*\*: Solo podrá ser añadido una vez y en un solo tipo de ticket, desde donde se podrá realizar la categorización.
{% endhint %}

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251220-142934.png | image-20251220-143057.png |

## OWNER

Permite añadir una tabla de registros, donde se puede definir que Empleados (con usuario relacionado) son propietarios del ticket, y por tanto, se quiere que tengan acceso al mismo.

* **Notificar vía Email:** Para enviar emails de seguimiento tras haber puesto el correo en el espacio en blanco.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251220-143325.png | image-20251220-143443.png |

## PROCESSES

Permite añadir una tabla de registros, estos registros serán procesos definidos en la opción **Inicio>** [**Procesos**](https://help.globalsuitesolutions.com/es/globalsuite/v1/procesos) de GlobalSuite®. Se puede asociar con esta tabla, un ticket con los procesos a los que afecta o está relacionado.

* **Asociar/Eliminar**: Se añaden o eliminan procesos de la lista predefinida al ticket relacionados con él.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251220-143757.png | image-20251220-145529.png |

## THREATS

Permite añadir una tabla de registros, estos registros serán elementos definidos en el [**Análisis de Riesgos**](https://help.globalsuitesolutions.com/es/globalsuite/v1/analisis-riesgos) de GlobalSuite. Se pueden asociar estas amenazas con el ticket al que afecta o está relacionado.

* **Asociar/Desasociar**: Permite asociar/borrar elementos.

| **Vista en Ajustes** |
| --- |
| image-20251220-144848.png |
| **Vista en GlobalSuite®** |
| image-20251220-151220.png |

## AUDIT-WORKS

Permite añadir una tabla de registros, estos registros serán trabajos de auditoría definidos en [**Programa de Auditorías**](https://help.globalsuitesolutions.com/es/globalsuite/v1/programa-auditorias) de GlobalSuite. Permite acceder al trabajo a través del link.

| **Vista en Ajustes** | **Vista en GlobalSuite®** |
| --- | --- |
| image-20251220-152119.png | image-20251220-152054.png |
