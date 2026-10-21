# Plantillas Informes Auditoría

{% hint style="info" %}
Los \*\*informes dinámicos de Auditoría en Word\*\* permiten generar documentos totalmente personalizables en formato \*\*.docx\*\* a partir de la información registrada en los \*\*Planes de Auditoría\*\* y \*\*Trabajos de Auditoría\*\*.
Esta funcionalidad amplía el sistema actual de plantillas Word, añadiendo dos nuevos tipos de informe específicos para el módulo de Auditoría y habilitando la creación de documentos completamente configurables mediante plantillas cargadas por el usuario.
{% endhint %}

## Descargar plantilla

La solución incorpora dos plantillas de ejemplo que pueden descargarse, revisarse y utilizarse como base:

* Plantilla de **Plan de Auditoría**
* Plantilla de **Trabajo de Auditoría**

Ambas plantillas contienen la estructura básica de información, tablas y etiquetas que pueden emplearse como punto de partida para personalizar los informes de Auditoría.

![image-20260828-223253.png](../../.gitbook/assets/1387241425-image-20260828-223253.png)

## **Subir plantilla**

En la opción **Subir plantilla**, los usuarios podrán cargar plantillas Word para:

* **Plan de Auditoría**
* **Trabajo de Auditoría**

![image-20260828-223341.png](../../.gitbook/assets/1387241425-image-20260828-223341.png)

## Variables

Las plantillas de **Plan de Auditoría** y **Trabajo de Auditoría** permiten utilizar un conjunto de variables que se sustituyen automáticamente por la información registrada en el módulo de Auditoría.

Estas variables pueden insertarse en **cualquier parte del documento Word**, ya sea en texto, encabezados, pies, tablas o listas.

A continuación se detallan las variables disponibles organizadas por categorías, siguiendo la estructura utilizada en las plantillas estándar de Word.

### Plan de Auditoría

#### Datos generales del plan

| Variable | Descripción |
| --- | --- |
| {planning.name} | Nombre del Plan de Auditoría. |
| {planning.description} | Descripción del plan. |
| {planning.status} | Estado del plan. |
| {planning.date} | Fecha del plan (formato configurable en plantilla). |

#### Metodología y análisis de riesgos del plan

| Variable | Descripción |
| --- | --- |
| {planning.planningMethodology} | Metodología de planificación. |
| {#planning.riskAnalysis}   * {analysis.name}   {/} | Listado de análisis de riesgos asociados al plan. |

#### Responsables del Plan de Auditoría

Se estructura con un bucle de roles y, dentro de cada rol, un bucle de empleados.

| Variable | Descripción |
| --- | --- |
| {#planning.roles}{role.name} {/} | Listado de roles del Plan de Auditoría. |
| {#role.employees}   * {employee.name} {/} | Listado de empleados de ese rol. Si por ejemplo se quisiera un listado con bullets. |

### Elementos asociados al Plan

| Variable | Descripción |
| --- | --- |
| {#planning.items} | Inicio del listado de elementos asociados al plan. |
| {item.name} | Nombre del elemento asociado. |
| {item.category} | Categoría del elemento. |
| {item.riskAnalysis} | Análisis de riesgos asociado al elemento. |
| {item.associateWorks} | Trabajos de auditoría asociados al elemento. |
| {item.dim\_alias.dimension.value} | Valor de las dimensiones del elemento, usando el alias configurado en la metodología. |
| {/} | Fin del listado de elementos asociados al plan. |

### Trabajos de Auditoría

#### Datos generales del trabajo

| Variable | Descripción |
| --- | --- |
| {#planning.auditWorks} | Inicio del listado de trabajos asociados al plan. |
| {auditWork.name} | Nombre del trabajo de auditoría. |
| {auditWork.type} | Tipo de trabajo. |
| {auditWork.responsible} | Responsable del trabajo. |
| {auditWork.status} | Estado del trabajo. |
| {auditWork.description} | Descripción del trabajo. |
| {auditWork.date} | Fecha del trabajo. |
| {#auditWork.items}   * {item.name}{/} | Elementos asociados al trabajo con bullets. |
| {auditWork.expectedStartDate} | Fecha de inicio prevista. |
| {auditWork.expectedEndDate} | Fecha de fin prevista. |
| {auditWork.actualStartDate} | Fecha de inicio real. |
| {auditWork.actualEndDate} | Fecha de fin real. |
| {auditWork.progress} | Progreso del trabajo (porcentaje). |
| {auditWork.auditPlan} | Plan de Auditoría al que pertenece el trabajo. |
| {/} | Fin del listado de trabajos asociados al plan. |

#### Campos configurables del trabajo

| Variable | Descripción |
| --- | --- |
| {auditWork.alias} | Campo configurable del trabajo, usando el alias definido en Ajustes > Metodologías Auditoría > [General](https://help.globalsuitesolutions.com/es/globalsuite/v1/metodologias-auditorias#MetodologíasAuditorías-Configuracióndecampos) |

#### Planificación del trabajo

(Sección específica de planificación de un trabajo de auditoría)

| Variable | Descripción |
| --- | --- |
| {auditWork.name} | Nombre del trabajo. |
| {auditWork.type} | Tipo de trabajo. |
| {auditWork.responsible} | Responsable. |
| {auditWork.description} | Descripción. |
| {auditWork.objectives} | Objetivos. |
| {auditWork.requester} | Solicitante. |
| {auditWork.status} | Estado. |
| {auditWork.auditPlan} | Plan de auditoría asociado. |
| {auditWork.expectedStartDate} | Fecha fin prevista |
| {auditWork.expectedEndDate} | Fecha prevista fin. |

### Equipo de trabajo

| Variable | Descripción |
| --- | --- |
| {#auditWork.workTeams} | Inicio del listado del equipo de trabajo. |
| {workTeam.role} | Rol dentro del equipo de trabajo. |
| {workTeam.employee} | Empleado asociado al rol. |
| {workTeam.type} | Tipos de auditor. |
| {workTeam.plannedHours} | Horas planificadas para ese miembro. |
| {/} | Fin del listado del equipo de trabajo. |

### Documentación asociada

| Variable | Descripción |
| --- | --- |
| {#auditWork.documentations} | Inicio del listado de documentación |
| {documentation.name} | Nombre del archivo. |
| {documentation.extension} | Extensión del archivo. |
| {documentation.date} | Fecha. |
| {documentation.description} | Descripción de la documentación. |
| {/} | Fin del listado de documentación |

### Metodologías de ejecución

| Variable | Descripción |
| --- | --- |
| {auditWork.executionMethodologies.items} | Metodología de ejecución de Elementos. |
| {auditWork.executionMethodologies.risks} | Metodología de ejecución de Riesgos. |
| {auditWork.executionMethodologies.controls} | Metodología de ejecución de Controles. |

### Alcance del Plan

| Variable | Descripción |
| --- | --- |
| {#auditWork.scope} | Inicio del listado del Alcance. |
| {item} | Elemento incluido en el alcance. |
| {category} | Categoría del elemento. |
| {categoryPath} | Ruta / jerarquía de categoría. |
| {riskAnalysis} | Análisis de riesgos asociado al elemento. |
| {dim\_alias.dimension\_name} | Nombre de las dimensiones del elemento (alias de metodología). |
| {dim\_alias.dimension.value} | Dimensiones del elemento (alias de metodología). |
| {dim\_alias.dimension\_alias} | Alias de las dimensiones del elemento (alias de metodología). |
| {/} | Fin del listado del Alcance. |
| {#auditWork.scope}  {#dimensions}{dimension\_name}{/} | Ejemplo Listado de dimensiones por elemento. |

Ejemplo:

| Elemento | Categoría | Análisis de riesgos | Dimensión U1 |
| --- | --- | --- | --- |
| {#auditWork.scope}{item} | {category} | {riskAnalysis} | Alias: {dim\_U1.dimension\_alias}  Nombre: {dim\_U1.dimension\_name}  Valor: {dim\_U1.dimension\_value} |

Resultado:

| Elemento | Categoría | Análisis de riesgos | dim\_U1 |
| --- | --- | --- | --- |
| Servicio reparto de mercancías | Servicios | Análisis de riesgos operacional | Alias:U1  Nombre: Riesgo del elemento  Valor: Medio |
| Servicio de soporte técnico | Servicios | Análisis de riesgos operacional,  Análisis de riesgos de seguridad | Alias:U1  Nombre: Riesgo del elemento  Valor: Alto |

### Ejecución – Elementos

| Variable | Descripción |
| --- | --- |
| {#auditWork.executionItems} | Inicio del listado de elementos de ejecución del trabajo. |
| {executionItem.name} | Nombre del elemento. |
| {executionItem.category} | Categoría del elemento. |
| {executionItem.categoryPath} | Ruta / jerarquía de la categoría. |
| {executionItem.riskAnalysis} | Análisis de riesgos asociado al elemento. |
| {#executionItem.dimensions} | Inicio del listado de dimensiones de ejecución de elementos. |
| {dimension\_name} | Nombre de la dimensión. |
| {dimension.value} | Valor de la dimensión. |
| {dimension\_alias} | Alias de la dimensión. |
| {#executionItem.tickets} | Inicio del listado de tickets asociados al elemento. |
| {/}{/} | Fin del listado del elementos de ejecución del trabajo y del listado de dimensiones |

### Ejecución – Riesgos

| Variable | Descripción |
| --- | --- |
| {#executionItem.risks} | Inicio del listado de riesgos de ejecución del trabajo. |
| {risk.name} | Riesgo. |
| {risk.taxonomy} | Agrupación de riesgo (taxonomía). |
| {risk.riskAnalysis} | Análisis de riesgos asociado. |
| {#risk.dimensions} | Inicio del listado de dimensiones de ejecución de riesgos. |
| {dimension\_name} | Nombre de la dimensión de riesgo. |
| {dimension.value} | Valor de la dimensión de riesgo. |
| {dimension\_alias} | Alias de la dimensión. |
| {#risk.tickets} | Inicio del listado de tickets asociados al riesgo. |
| {/}{/} | Fin del listado del elementos de ejecución del trabajo y del listado de dimensiones |

### Ejecución – Controles

| Variable | Descripción |
| --- | --- |
| {#executionItem.controls} | Inicio del listado de controles de ejecución del trabajo. |
| {control.name} | Nombre del control. |
| {control.riskAnalysis} | Análisis de riesgos asociado al control. |
| {#control.risks}  - {risk.name}{/} | Inicio y fin del listado de riesgos asociados al control |
| {#control.dimensions} | Inicio del listado de dimensiones de ejecución de controles. |
| {dimension\_name} | Nombre de la dimensión de control. |
| {dimension\_value} | Valor de la dimensión de control. |
| {dimension\_alias} | Alias de la dimensión. |

### Planificación (proyecto y tareas)

#### Proyecto

| Variable | Descripción |
| --- | --- |
| {auditWork.project.level} | Nivel |
| {auditWork.project.name} | Nombre del proyecto. |
| {auditWork.project.remainingDays} | Días restantes. |
| {auditWork.project.expectedStartDate} | Fecha prevista inicio. |
| {auditWork.project.expectedEndDate} | Fecha prevista fin. |
| {auditWork.project.realStartDate} | Fecha real inicio. |
| {auditWork.project.realEndDate} | Fecha real fin. |
| {auditWork.project.estimatedTime} | Tiempo estimado. |
| {auditWork.project.dedicatedTime} | Tiempo dedicado. |
| {auditWork.project.estimatedCost} | Coste estimado. |
| {auditWork.project.realCost} | Coste real. |

#### Tareas

| Variable | Descripción |
| --- | --- |
| {#auditWork.project.tasks} | Inicio del listado de tareas del proyecto. |
| {task.level} | Nivel de la tarea en el árbol |
| {task.name} | Nombre de la tarea. |
| {task.description} | Descripción. |
| {task.type} | Tipo. |
| {task.responsibles} | Responsables. |
| {task.remainingDays} | Días restantes. |
| {task.requestDate} | Fecha de solicitud. |
| {task.expectedStartDate} | Fecha prevista inicio. |
| {task.expectedEndDate} | Fecha prevista fin. |
| {task.realStartDate} | Fecha real inicio. |
| {task.realEndDate} | Fecha real fin. |
| {task.estimatedTime} | Tiempo estimado. |
| {task.dedicatedTime} | Tiempo dedicado. |
| {task.estimatedCost} | Coste estimado. |
| {task.realCost} | Coste real. |
| {task.status} | Estado. |
| {task.priority} | Prioridad. |
| {task.progress} | Porcentaje de progreso. |
| {/} | Fin del listado de tareas del proyecto. |

### Papeles de trabajo

| Variable | Descripción |
| --- | --- |
| {#auditWork.workingPapers} | Inicio del listado de papeles de trabajo. |
| {workingPaper.code} | Código del papel de trabajo. |
| {workingPaper.name} | Nombre del papel de trabajo. |
| {workingPaper.type} | Tipo de papel de trabajo. |
| {workingPaper.description} | Descripción. |
| {workingPaper.attachment} | Anexo asociado. |
| {#workingPaper.relatedRecords}   * {name} {/} | Inicio del listado de registros relacionados. |
| {#executionItem.workingPapers} | Inicio del listado de papeles de trabajo asociados al elemento. |
| {#risk.workingPapers} | Inicio del listado de papeles de trabajo asociados al riesgo. |
| {/} | Fin del listado de papeles de trabajo. |

### Tickets

| Variable | Descripción |
| --- | --- |
| {#planning. tickets} | Inicio del listado de tickets asociados a una planificación. |
| {#auditWork.tickets} | Inicio del listado de tickets asociados al trabajo |
| {#auditWork.unrelatedTickets} | Inicio del listado de tickets asociados al trabajo, que no están relacionados a ningún elemento o riesgo. |
| {#executionItem.tickets} | Inicio del listado de tickets asociados al elemento. Debe utilizarse dentro del bloque `{#auditWork.tickets}` |
| {#risk.tickets} | Inicio del listado de tickets asociados al riesgo. |

#### Caso de uso: Tickets relacionados con los tickets del trabajo

Este caso de uso permite obtener, desde un Informe de Auditoría, los tickets relacionados —entradas o salidas— con los tickets asociados a un trabajo de auditoría.

Para descargar el listado de tickets relacionados, es necesario incluir dentro del bucle de tickets del trabajo un segundo **bucle correspondiente al campo de entrada o salida.**

Por ejemplo, para mostrar las salidas relacionadas con cada ticket:

{% hint style="info" %}
```
{#auditWork.tickets}
Nombre del ticket: {REASU}
◦ Salidas: {#REOUT}
{CPASU} {NCASU}
{/}
{/}
```
{% endhint %}

En este ejemplo:

* `{#auditWork.tickets}` inicia el listado de tickets asociados al trabajo de auditoría.
* `{REASU}` es el alias del campo Asunto del ticket asociado al trabajo.
* `{#REOUT}`inicia el bucle de las salidas relacionadas con ese ticket. Se debe indicar el alias del campo de **Entradas** o **Salidas**, según la información que se necesite mostrar.
* `{CPASU}` y `{NCASU}`son ejemplos de alias de los campos que se quieren mostrar para cada ticket de entrada o salida. Estos campos deberán repetirse según los tipos de tickets que se deseen incluir. En este caso, `{CPASU}` corresponde al campo Asunto de los tickets de tipo Acciones correctivas y preventivas, mientras que `{NCASU}` corresponde al campo Asunto de los tickets de tipo No conformidades.

Es importante incluir el bucle del campo entrada o salida; en este ejemplo, `{#REOUT}`. Si únicamente se introduce el campo de la salida sin su bucle, no se descargará correctamente el listado completo de tickets relacionados.

## Opciones de formateo

Las plantillas dinámicas de Auditoría permiten aplicar opciones de formateo directamente sobre las variables utilizadas en los informes. Estas opciones funcionan en cualquier plantilla Word o Excel configurada en GlobalSuite® y son compatibles con todas las variables disponibles del módulo de Auditoría.

---

### Formateo de listas mediante `|join`

Cuando una variable representa un conjunto de valores (arrays), es posible convertir la lista en una única línea concatenando los elementos con el separador que se desee.

Sintaxis:

`{variable | join:' - '}`

Ejemplos:

`{role.employees|join:' - ' }`

`{auditWork.items|join:' - '}`

`{control.risks|join:' - '}`

Resultado esperado:

Una lista como:

{% hint style="info" %}
```
Elemento A
Elemento B
Elemento C
```
{% endhint %}

Se mostrará como:

{% hint style="info" %}
```
Elemento A - Elemento B - Elemento C
```
{% endhint %}

Ejemplo tabla:

| Rol | Empleado |
| --- | --- |
| {#planning.roles}{role.name} | {role.employees|join:' - ' }{/} |

Resultado:

| Rol | Empleado |
| --- | --- |
| Equipo Auditoría | Cristina R.- Pedro S.- Elena P. |
| Rol Workflow | Daniel T - Ana M. - Diego R. |

Esta opción puede usarse **con cualquier variable múltiple**, incluyendo:

* Elementos
* Riesgos
* Controles
* Dimensiones
* Empleados de un rol
* Documentos
* Tickets
* Registros relacionados
* Cualquier alias configurado

### Formateo de fechas mediante `|formatDate`

Las variables que representan fechas pueden mostrarse usando el formato por defecto del sistema o un formato personalizado definido por el usuario.

#### 1. Formato por defecto

Si no se especifica ningún formato, GlobalSuite® utilizará automáticamente:

`dd/MM/yyyy HH:mm:ss`

Ejemplo:

`{auditWork.date}`

→ `13/06/2025 11:41:48`

#### 2. Formato personalizado

Si se desea controlar la representación de la fecha, puede definirse un formato directamente en la plantilla.

Sintaxis:

`{variable | formatDate:"yyyy-MM-dd"}`

Ejemplos:

**Fecha simple**   
planning.date | formatDate:"yyyy-MM-dd"  
→ 2025-09-18

**Día/mes/año sin hora**  
 | formatDate:"dd/MM/yyyy"  
→ 18/09/2025

**Fecha larga con nombre del mes**  
auditWork.date | formatDate:"dd MMMM yyyy"  
→ 18 septiembre 2025

**Día de la semana + fecha**  
task.requestDate | formatDate:"EEEE, dd/MM/yyyy"  
→ jueves, 18/09/2025

**Año abreviado + mes abreviado + día**  
auditWork.actualEndDate | formatDate:"yy MMM dd"  
→ 25 sep 18

**Fecha y hora con formato válido date-fns**  
task.requestDate | formatDate:"dd-MM-yyyy HH:mm"  
→ 18-09-2025 14:30

**Caracteres más utilizados**

* yyyy → año completo
* yy → año abreviado
* MM → mes numérico (01–12)
* MMM → mes abreviado (ene, feb, mar…)
* MMMM → mes completo
* dd → día del mes
* EEEE → día de la semana completo
* EEE → día de la semana abreviado
* HH → horas 00–23
* mm → minutos
* ss → segundos

{% hint style="info" %}
\*\*Nota\*\*
Se distingue mayúsculas/minúsculas; deben respetarse exactamente.
{% endhint %}
