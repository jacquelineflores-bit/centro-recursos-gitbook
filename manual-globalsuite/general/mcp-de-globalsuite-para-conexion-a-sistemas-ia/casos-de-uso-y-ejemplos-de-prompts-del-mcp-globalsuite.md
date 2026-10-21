# Casos de uso y ejemplos de prompts del MCP GlobalSuite

Estos prompts son puntos de partida para sacar el máximo partido al MCP GlobalSuite. Cópialos tal cual o adáptalos a tu caso: cambia lo que va entre [corchetes] por el nombre de tu análisis, tu elemento o tu normativa. Funcionan con cualquier asistente compatible.

*Las capturas de esta página son respuestas reales de Claude y de ChatGPT con el MCP GlobalSuite conectado a un entorno demo de GlobalSuite®. Tus respuestas variarán según tus datos y el asistente que uses.*

* [Consejos para obtener mejores respuestas](#CasosdeusoyejemplosdepromptsdelMCPGlobalSuite-Consejosparaobtenermejoresrespuestas)
* [1. Primeros pasos](#CasosdeusoyejemplosdepromptsdelMCPGlobalSuite-1.Primerospasos)
* [2. Inventario de activos](#CasosdeusoyejemplosdepromptsdelMCPGlobalSuite-2.Inventariodeactivos)
* [3. Análisis de riesgos](#CasosdeusoyejemplosdepromptsdelMCPGlobalSuite-3.Análisisderiesgos)
* [4. Controles y planes de tratamiento](#CasosdeusoyejemplosdepromptsdelMCPGlobalSuite-4.Controlesyplanesdetratamiento)
* [5. Compliance](#CasosdeusoyejemplosdepromptsdelMCPGlobalSuite-5.Compliance)
* [6. Gestor Documental](#CasosdeusoyejemplosdepromptsdelMCPGlobalSuite-6.GestorDocumental)
* [7. Gráficas y cuadros de mando](#CasosdeusoyejemplosdepromptsdelMCPGlobalSuite-7.Gráficasycuadrosdemando)
* [8. Informes y plantillas](#CasosdeusoyejemplosdepromptsdelMCPGlobalSuite-8.Informesyplantillas)
* [9. Acciones de escritura](#CasosdeusoyejemplosdepromptsdelMCPGlobalSuite-9.Accionesdeescritura)
* [10. Novedades de GlobalSuite®](#CasosdeusoyejemplosdepromptsdelMCPGlobalSuite-10.NovedadesdeGlobalSuite®)
* [Si la respuesta no es completa](#CasosdeusoyejemplosdepromptsdelMCPGlobalSuite-Silarespuestanoescompleta)

## Consejos para obtener mejores respuestas

* **Llama a las cosas como en GlobalSuite®.** Usa el nombre exacto del análisis, la evaluación normativa o el elemento: el asistente lo busca por su nombre.
* **Pide el formato que necesitas:** una tabla, una gráfica, un Excel, un Word o un resumen para dirección.
* **Empieza por lo general y profundiza.** Pregunta primero por el estado de un análisis y después por los riesgos o controles que te interesen.
* **Con mucho volumen de datos, acota o investiga.** Limita la pregunta a un análisis, una categoría o un elemento, o activa el modo de investigación de tu asistente (por ejemplo, Investigación en Claude o Investigación profunda en ChatGPT) y pídele que revise todas las páginas de resultados.
* **Pídele que te diga qué ha revisado.** En consultas que cruzan muchos datos, pide que indique qué elementos, riesgos o requisitos ha consultado: así sabrás si la respuesta está completa. Con los mismos datos, cada asistente y cada modelo pueden llegar a conclusiones distintas.
* **Revisa siempre el resultado.** La IA puede equivocarse; contrasta los datos importantes en GlobalSuite®.

## 1. Primeros pasos

### Qué puede hacer el conector

{% hint style="info" %}
```
¿Qué información de GlobalSuite puedes consultar y qué acciones puedes
hacer con el conector?
```
{% endhint %}

**ChatGPT**

![Respuesta real con lo que el asistente puede consultar y hacer con el conector.](../../.gitbook/assets/2171043841-mcp-real-p01-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con lo que el asistente puede consultar y hacer con el conector.](../../.gitbook/assets/2171043841-mcp-real-p01-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Resumen de tu sistema de gestión

{% hint style="info" %}
```
Hazme un resumen del estado de mi sistema de gestión en GlobalSuite:
análisis de riesgos activos, evaluaciones normativas con su grado de
cumplimiento y los tres puntos que requieren más atención.
```
{% endhint %}

*Herramientas: get\_all\_risk\_analysis · list\_compliance\_evaluations*

**ChatGPT**

![Respuesta real con un resumen ejecutivo del sistema de gestión.](../../.gitbook/assets/2171043841-mcp-real-c14-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con un resumen ejecutivo del sistema de gestión.](../../.gitbook/assets/2171043841-mcp-real-c14-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Revisa la calidad de tus datos

{% hint style="info" %}
```
Revisa la calidad de los datos del análisis [nombre] antes de presentarlo
al comité: elementos sin valorar o sin categoría, controles duplicados o
con nombres de prueba y acciones del plan de tratamiento sin responsable o
sin plazo. Dame una tabla con cada problema, cuántos casos hay y cómo lo
corregirías.
```
{% endhint %}

*Herramientas: get\_all\_risk\_analysis · get\_elements\_by\_analysis · get\_controls*

**ChatGPT**

![Respuesta real con una revisión de la calidad de los datos de un análisis de riesgos antes de un comité.](../../.gitbook/assets/2171043841-mcp-real-c16-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con una revisión de la calidad de los datos de un análisis de riesgos antes de un comité.](../../.gitbook/assets/2171043841-mcp-real-c16-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Localiza tus análisis

{% hint style="info" %}
```
Lista mis análisis de riesgos activos con su responsable, su metodología y
su nivel de riesgo aceptable.
```
{% endhint %}

*Herramientas: get\_all\_risk\_analysis*

**ChatGPT**

![Respuesta real con los análisis de riesgos activos, su responsable, su metodología y su nivel de riesgo aceptable.](../../.gitbook/assets/2171043841-mcp-real-c17-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con los análisis de riesgos activos, su responsable, su metodología y su nivel de riesgo aceptable.](../../.gitbook/assets/2171043841-mcp-real-c17-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

## 2. Inventario de activos

### Elementos más críticos

{% hint style="info" %}
```
¿Cuáles son los [10] elementos más críticos de [mi inventario / el análisis
«nombre»]? Ordénalos por importancia y dime cómo están valorados en
confidencialidad, integridad y disponibilidad.
```
{% endhint %}

*Herramientas: get\_elements o get\_elements\_by\_analysis · get\_methodology\_elements*

**ChatGPT**

![Respuesta real con los elementos más críticos del análisis y su valoración de confidencialidad, integridad y disponibilidad.](../../.gitbook/assets/2171043841-mcp-real-c01-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con los elementos más críticos del análisis y su valoración de confidencialidad, integridad y disponibilidad.](../../.gitbook/assets/2171043841-mcp-real-c01-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Elementos sin valorar

{% hint style="info" %}
```
¿Qué elementos de la categoría [Software] no tienen valoradas la
confidencialidad, la integridad o la disponibilidad?
```
{% endhint %}

*Herramientas: get\_categories · get\_elements*

**ChatGPT**

![Respuesta real con los elementos de Software sin confidencialidad, integridad o disponibilidad.](../../.gitbook/assets/2171043841-mcp-real-c22-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con los elementos de Software sin confidencialidad, integridad o disponibilidad.](../../.gitbook/assets/2171043841-mcp-real-c22-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Elementos de un responsable

{% hint style="info" %}
```
¿Qué elementos del inventario tiene asignados [propietario] y cuál es su
importancia?
```
{% endhint %}

*Herramientas: get\_elements*

**ChatGPT**

![Respuesta real con los elementos de un responsable y su importancia.](../../.gitbook/assets/2171043841-mcp-real-p02-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con los elementos de un responsable y su importancia.](../../.gitbook/assets/2171043841-mcp-real-p02-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Qué significa cada nivel

{% hint style="info" %}
```
Explícame qué criterio define cada nivel de [disponibilidad] en la
metodología de mi inventario.
```
{% endhint %}

*Herramientas: get\_methodology\_elements*

**ChatGPT**

![Respuesta real con el criterio de cada nivel de disponibilidad.](../../.gitbook/assets/2171043841-mcp-real-p03-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con el criterio de cada nivel de disponibilidad.](../../.gitbook/assets/2171043841-mcp-real-p03-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

## 3. Análisis de riesgos

### Riesgos de un elemento

{% hint style="info" %}
```
¿Qué riesgos tiene el elemento [nombre] en el análisis [nombre]? Dime su
nivel de riesgo y de riesgo residual y cuáles debería tratar primero.
```
{% endhint %}

*Herramientas: get\_elements\_by\_analysis · get\_element\_threats · get\_methodology\_risks*

**ChatGPT**

![Respuesta real con los riesgos de un elemento, su nivel de riesgo y de riesgo residual y la prioridad de tratamiento.](../../.gitbook/assets/2171043841-mcp-real-c03-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con los riesgos de un elemento, su nivel de riesgo y de riesgo residual y la prioridad de tratamiento.](../../.gitbook/assets/2171043841-mcp-real-c03-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Riesgos críticos de un análisis

{% hint style="info" %}
```
Identifica los riesgos con riesgo residual [Muy alto] del análisis [nombre]
y agrúpalos por elemento. Revisa todas las páginas de resultados.
```
{% endhint %}

*Herramientas: get\_elements\_by\_analysis · get\_element\_threats · get\_methodology\_risks · Recomendado: modo de investigación*

**ChatGPT**

![Respuesta real con los riesgos de nivel residual alto agrupados por elemento.](../../.gitbook/assets/2171043841-mcp-real-p04-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con los riesgos de nivel residual alto agrupados por elemento.](../../.gitbook/assets/2171043841-mcp-real-p04-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Elementos por encima del riesgo aceptable

{% hint style="info" %}
```
¿Qué elementos del análisis [nombre] superan su nivel de riesgo aceptable?
Ordénalos de mayor a menor riesgo e indica cuáles no tienen ningún control
asociado.
```
{% endhint %}

*Herramientas: get\_all\_risk\_analysis · get\_elements\_by\_analysis · get\_element\_threats · get\_threat\_controls*

**ChatGPT**

![Respuesta real con los elementos que superan el nivel de riesgo aceptable y sus controles.](../../.gitbook/assets/2171043841-mcp-real-c18-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con los elementos que superan el nivel de riesgo aceptable y sus controles.](../../.gitbook/assets/2171043841-mcp-real-c18-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Cómo se calcula el riesgo

{% hint style="info" %}
```
Explícame cómo se calcula el riesgo residual en la metodología del análisis
[nombre] y qué significa cada nivel.
```
{% endhint %}

*Herramientas: get\_risk\_analysis · get\_methodology\_risks*

**ChatGPT**

![Respuesta real que explica el cálculo del riesgo residual y el significado de cada nivel.](../../.gitbook/assets/2171043841-mcp-real-c19-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real que explica el cálculo del riesgo residual y el significado de cada nivel.](../../.gitbook/assets/2171043841-mcp-real-c19-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Dónde no están actuando los controles

{% hint style="info" %}
```
¿En qué elementos del análisis [nombre] el riesgo residual es igual al
riesgo? Indica si esos riesgos tienen controles asociados.
```
{% endhint %}

*Herramientas: get\_elements\_by\_analysis · get\_element\_threats · get\_threat\_controls · Recomendado: modo de investigación*

**ChatGPT**

![Respuesta real con los elementos cuyo riesgo residual es igual al riesgo.](../../.gitbook/assets/2171043841-mcp-real-p05-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con los elementos cuyo riesgo residual es igual al riesgo.](../../.gitbook/assets/2171043841-mcp-real-p05-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

## 4. Controles y planes de tratamiento

### Controles de un riesgo

{% hint style="info" %}
```
Para el riesgo [nombre] del elemento [nombre] en el análisis [nombre], ¿qué
controles hay implantados y cuáles están en plan de tratamiento?
```
{% endhint %}

*Herramientas: get\_element\_threats · get\_threat\_controls*

**ChatGPT**

![Respuesta real con los controles implantados y en plan de tratamiento de los riesgos más altos de dos elementos.](../../.gitbook/assets/2171043841-mcp-real-c04-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con los controles implantados y en plan de tratamiento de los riesgos más altos de dos elementos.](../../.gitbook/assets/2171043841-mcp-real-c04-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Controles que cubren más riesgos críticos

{% hint style="info" %}
```
Identifica los controles que mitigan el mayor número de riesgos con nivel
[Muy alto] en el análisis [nombre] y ordénalos de más a menos riesgos
cubiertos.
```
{% endhint %}

*Herramientas: get\_elements\_by\_analysis · get\_element\_threats · get\_threat\_controls · Recomendado: modo de investigación*

**ChatGPT**

![Respuesta real con los controles ordenados por número de riesgos altos cubiertos.](../../.gitbook/assets/2171043841-mcp-real-c10-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con los controles ordenados por número de riesgos altos cubiertos.](../../.gitbook/assets/2171043841-mcp-real-c10-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Plan de tratamiento pendiente

{% hint style="info" %}
```
¿Qué controles del plan de tratamiento del análisis [nombre] tienen el
plazo vencido o no tienen responsable? Dame una tabla.
```
{% endhint %}

*Herramientas: get\_controls*

**ChatGPT**

![Respuesta real con los controles del plan de tratamiento con el plazo vencido o sin responsable.](../../.gitbook/assets/2171043841-mcp-real-c20-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con los controles del plan de tratamiento con el plazo vencido o sin responsable.](../../.gitbook/assets/2171043841-mcp-real-c20-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Controles más débiles

{% hint style="info" %}
```
Lista los [10] controles del análisis [nombre] con menor madurez y dime qué
acciones tienen abiertas.
```
{% endhint %}

*Herramientas: get\_controls · get\_methodology\_controls*

**ChatGPT**

![Respuesta real con los controles de menor madurez y sus acciones.](../../.gitbook/assets/2171043841-mcp-real-p06-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con los controles de menor madurez y sus acciones.](../../.gitbook/assets/2171043841-mcp-real-p06-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Interpretar la madurez de un control

{% hint style="info" %}
```
El control [nombre] del análisis [nombre] tiene madurez [Baja]. ¿Qué
criterio define ese nivel en mi metodología y qué haría falta para subirlo
al siguiente?
```
{% endhint %}

*Herramientas: get\_controls · get\_methodology\_controls*

**ChatGPT**

![Respuesta real con el criterio de madurez de un control y cómo subirlo de nivel.](../../.gitbook/assets/2171043841-mcp-real-p07-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con el criterio de madurez de un control y cómo subirlo de nivel.](../../.gitbook/assets/2171043841-mcp-real-p07-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Evidencias de los controles

{% hint style="info" %}
```
¿Qué evidencias tengo registradas y a qué controles están vinculadas? Dime
también qué controles implantados del análisis [nombre] no tienen ninguna
evidencia.
```
{% endhint %}

*Herramientas: get\_evidences · get\_controls · get\_threat\_controls*

**ChatGPT**

![Respuesta real con las evidencias registradas, sus controles y los controles implantados sin evidencia.](../../.gitbook/assets/2171043841-mcp-real-c21-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con las evidencias registradas, sus controles y los controles implantados sin evidencia.](../../.gitbook/assets/2171043841-mcp-real-c21-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

## 5. Compliance

### Estado de cumplimiento

{% hint style="info" %}
```
¿Cuál es el grado de cumplimiento de mis evaluaciones normativas? Hazme una
gráfica ordenada de mayor a menor y dime dónde debería centrarme.
```
{% endhint %}

*Herramientas: list\_compliance\_evaluations*

**ChatGPT**

![Respuesta real con una gráfica del grado de cumplimiento de las evaluaciones normativas.](../../.gitbook/assets/2171043841-mcp-real-c05-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con una gráfica del grado de cumplimiento de las evaluaciones normativas.](../../.gitbook/assets/2171043841-mcp-real-c05-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Brechas de una normativa

{% hint style="info" %}
```
Analiza las brechas de la evaluación [nombre de la normativa]. ¿Qué
apartados tienen menor cumplimiento, cuáles no tienen controles ni
evidencias y qué me recomiendas priorizar?
```
{% endhint %}

*Herramientas: list\_compliance\_evaluations · get\_compliance\_requirements\_tree*

**ChatGPT**

![Respuesta real con el análisis de brechas de una evaluación de ISO 27001.](../../.gitbook/assets/2171043841-mcp-real-c06-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con el análisis de brechas de una evaluación de ISO 27001.](../../.gitbook/assets/2171043841-mcp-real-c06-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Cumplimiento por dominio en una gráfica de radar

{% hint style="info" %}
```
Hazme una gráfica de radar con el grado de cumplimiento de cada dominio de
la evaluación [nombre de la normativa] y dime cuáles son los tres dominios
más débiles y qué harías primero.
```
{% endhint %}

*Herramientas: list\_compliance\_evaluations · get\_compliance\_requirements\_tree*

**ChatGPT**

![Respuesta real con una gráfica de radar del cumplimiento por dominio del Anexo A de ISO 27001.](../../.gitbook/assets/2171043841-mcp-real-c13-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con una gráfica de radar del cumplimiento por dominio del Anexo A de ISO 27001.](../../.gitbook/assets/2171043841-mcp-real-c13-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Requisitos sobre un tema

{% hint style="info" %}
```
¿Qué evaluaciones normativas tienen requisitos sobre [copias de seguridad]?
Resume su grado de cumplimiento en cada una.
```
{% endhint %}

*Herramientas: search\_compliance\_evaluations\_by\_requirement · get\_compliance\_requirements\_tree*

**ChatGPT**

**PENDIENTE: CAPTURA DE CHATGPT CUANDO SU CONECTOR PUEDA CONSULTAR LAS EVALUACIONES NORMATIVAS.**

**Claude**

![Respuesta real con las evaluaciones que tienen requisitos sobre copias de seguridad y su grado de cumplimiento.](../../.gitbook/assets/2171043841-mcp-real-p08-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Dónde más se aplica un control

{% hint style="info" %}
```
¿En qué otras normativas y requisitos se aplica el control [nombre]?
```
{% endhint %}

*Herramientas: get\_compliance\_requirements\_tree · get\_compliance\_common\_controls*

**PENDIENTE: CAPTURAS EN CHATGPT Y CLAUDE CUANDO EL ENTORNO DE DEMOSTRACIÓN TENGA CONTROLES VINCULADOS A LOS REQUISITOS DE SUS EVALUACIONES NORMATIVAS.**

### Qué se está haciendo en un apartado

{% hint style="info" %}
```
¿Qué no conformidades, hallazgos o acciones hay asociados a los requisitos
del apartado [A.9] de [ISO 27001]?
```
{% endhint %}

*Herramientas: get\_compliance\_requirements\_tree · get\_compliance\_requirements\_tickets*

**PENDIENTE: CAPTURAS EN CHATGPT Y CLAUDE CUANDO EL ENTORNO DE DEMOSTRACIÓN TENGA NO CONFORMIDADES, HALLAZGOS O ACCIONES VINCULADOS A LOS REQUISITOS.**

## 6. Gestor Documental

**PENDIENTE DE CORREGIR: EN LAS PRUEBAS DEL 29/09/2026, CLAUDE (CLAUDE.AI) LEYÓ Y RESUMIÓ EL DOCUMENTO, PERO CHATGPT Y CLAUDE CODE SOLO RECIBIERON SUS DATOS BÁSICOS, SIN EL CONTENIDO (read\_gd\_document). EN DEMO NO HAY NINGUNA POLÍTICA DE SEGURIDAD, Y LA BÚSQUEDA POR «POLÍTICA» DEVOLVIÓ ERROR EN CLAUDE CODE. ESTÁ EN EL CORREO A PACO CERRO.**

### Buscar y resumir un documento

{% hint style="info" %}
```
Busca en el gestor documental el documento [política de copias de
seguridad] y resúmeme sus puntos clave.
```
{% endhint %}

*Herramientas: search\_gd\_documents · read\_gd\_document*

**ChatGPT**

**Claude**

![Respuesta real que busca un documento en el Gestor Documental y resume su contenido.](../../.gitbook/assets/2171043841-mcp-real-c09-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Comparar un documento con un requisito

{% hint style="info" %}
```
Compara el documento [nombre] con el requisito [A.5.1] de [ISO 27001] e
indica qué le falta para evidenciar su cumplimiento.
```
{% endhint %}

*Herramientas: search\_gd\_documents · read\_gd\_document · get\_compliance\_requirements\_tree*

**PENDIENTE: CAPTURAS EN CHATGPT Y CLAUDE CUANDO SE CORRIJA LA LECTURA DE DOCUMENTOS DEL GESTOR DOCUMENTAL DESDE EL MCP.**

### Revisar las evidencias de un apartado

{% hint style="info" %}
```
Revisa los documentos asociados a los requisitos del apartado [A.8] de [ISO
27001] y dime si evidencian su cumplimiento.
```
{% endhint %}

*Herramientas: get\_compliance\_requirements\_tree · read\_gd\_document*

**PENDIENTE: CAPTURAS EN CHATGPT Y CLAUDE CUANDO SE CORRIJA LA LECTURA DE DOCUMENTOS DEL GESTOR DOCUMENTAL DESDE EL MCP.**

## 7. Gráficas y cuadros de mando

### Inventario por categoría

{% hint style="info" %}
```
Hazme una gráfica de [barras / sectores] con los elementos de mi inventario
agrupados por categoría.
```
{% endhint %}

*Herramientas: get\_elements · get\_categories*

**ChatGPT**

![Respuesta real con una gráfica de barras de los elementos del inventario agrupados por categoría.](../../.gitbook/assets/2171043841-mcp-real-c02-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con una gráfica de barras de los elementos del inventario agrupados por categoría.](../../.gitbook/assets/2171043841-mcp-real-c02-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Mapa de calor de riesgos

{% hint style="info" %}
```
Crea un mapa de calor de probabilidad e impacto con los riesgos del
elemento [nombre] del análisis [nombre]. Indica cuántos riesgos caen en
cada celda y cuáles están en la zona roja.
```
{% endhint %}

*Herramientas: get\_element\_threats · get\_methodology\_risks*

**ChatGPT**

![Respuesta real con un mapa de calor de probabilidad e impacto de los riesgos de un elemento.](../../.gitbook/assets/2171043841-mcp-real-c11-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con un mapa de calor de probabilidad e impacto de los riesgos de un elemento.](../../.gitbook/assets/2171043841-mcp-real-c11-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Cuadro de mando de un análisis

{% hint style="info" %}
```
Prepara un cuadro de mando visual del análisis [nombre] con el número de
elementos por categoría, la distribución de los elementos por nivel de
importancia y los cinco elementos más críticos con su valoración.
```
{% endhint %}

*Herramientas: get\_elements\_by\_analysis · get\_element\_threats · get\_controls · Recomendado: modo de investigación*

**ChatGPT**

![](../../.gitbook/assets/2171043841-mcp-real-c12-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![](../../.gitbook/assets/2171043841-mcp-real-c12-claude.png)

*Cuadro de mando que Claude generó como artefacto con el MCP GlobalSuite · entorno de demostración*

## 8. Informes y plantillas

### Rellenar la plantilla de importación

Adjunta al chat la plantilla de importación de tu análisis (la obtienes en Data Import) y pide al asistente que la complete. Después revisa el archivo e impórtalo desde Data Import.

{% hint style="info" %}
```
Te adjunto la plantilla de importación de GlobalSuite. Rellénala con una
propuesta de riesgos, su valoración y un control para cada uno, para los
elementos [nombres] del análisis [nombre]. Usa los niveles de la plantilla
y no repitas riesgos que ya existan.
```
{% endhint %}

*Herramientas: get\_elements\_by\_analysis · get\_element\_threats*

**ChatGPT**

![Respuesta real que devuelve la plantilla de importación rellenada con riesgos, valoraciones y controles propuestos.](../../.gitbook/assets/2171043841-mcp-real-c07-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real que devuelve la plantilla de importación rellenada con riesgos, valoraciones y controles propuestos.](../../.gitbook/assets/2171043841-mcp-real-c07-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Informe con tu plantilla Word

{% hint style="info" %}
```
Genera el informe de la plantilla que te adjunto para los elementos
[nombres] del análisis [nombre]. Respeta su estructura, sus textos y su
formato, y rellena cada apartado con los datos de GlobalSuite.
```
{% endhint %}

*Herramientas: get\_elements\_by\_analysis · get\_element\_threats · get\_threat\_controls · get\_methodology\_risks*

**ChatGPT**

![Respuesta real que genera un informe Word con la plantilla del cliente.](../../.gitbook/assets/2171043841-mcp-real-c08-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real que genera un informe Word con la plantilla del cliente.](../../.gitbook/assets/2171043841-mcp-real-c08-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Informe ejecutivo para dirección

{% hint style="info" %}
```
Redacta en Word un informe ejecutivo de dos páginas del estado de
cumplimiento de [ISO 27001] para el comité de dirección, con conclusiones y
próximos pasos.
```
{% endhint %}

*Herramientas: list\_compliance\_evaluations · get\_compliance\_requirements\_tree · get\_compliance\_requirements\_tickets*

**ChatGPT**

![Respuesta real con el informe ejecutivo de cumplimiento en Word.](../../.gitbook/assets/2171043841-mcp-real-p13-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

**PENDIENTE: CAPTURA DE CLAUDE.**

### Exportar a Excel

{% hint style="info" %}
```
Exporta a una hoja de cálculo los controles del análisis [nombre] con su
tipo, su responsable, su plazo y su madurez.
```
{% endhint %}

*Herramientas: get\_controls*

**ChatGPT**

![Respuesta real con la exportación a Excel de los controles de un análisis.](../../.gitbook/assets/2171043841-mcp-real-c23-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con la exportación a Excel de los controles de un análisis.](../../.gitbook/assets/2171043841-mcp-real-c23-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

## 9. Acciones de escritura

En Inventario, Análisis de Riesgos y Controles también puedes pedirle al asistente que actúe: dar de alta y modificar elementos, valorarlos, crear riesgos, planes de tratamiento, acciones y evidencias, o recalcular un análisis. Los ejemplos de este apartado se hicieron en el entorno de demostración, con datos ficticios.

### Cómo se confirman los cambios

El conector no pide confirmación por sí mismo: la pide el asistente, y cada uno lo hace a su manera.

* **ChatGPT** muestra una tarjeta «¿Permitir que ChatGPT use GlobalSuite?» con «Permitir una vez» y «Denegar» antes de algunas acciones, como modificar un elemento, sacarlo de un análisis o borrarlo. No la muestra en todas: en nuestras pruebas creó y valoró elementos, riesgos y acciones sin pedirla.
* **Claude** depende del modo de permisos que elijas: en el modo que pide permiso, lo solicita para cada herramienta y te enseña los datos que va a enviar; en el modo automático no pregunta. Además, no hace borrados permanentes: te propone marcar el elemento como obsoleto, que se puede revertir.

Para trabajar con seguridad:

* **Pide primero una propuesta.** Añade «no lo apliques hasta que te lo confirme» y revisa la tabla antes de decir «Aplícala», como en los ejemplos.
* **Sé concreto en los borrados.** Di exactamente qué elemento quieres eliminar o sacar de un análisis; evita peticiones abiertas como «borra lo que no se usa».
* **Sacar un elemento de un análisis elimina sus riesgos en ese análisis.** Si vuelve a entrar, habrá que crearlos de nuevo.
* **Comprueba el resultado en GlobalSuite®.**

**ChatGPT**

![Confirmación que pide el asistente antes de una acción de escritura.](../../.gitbook/assets/2171043841-mcp-real-confirmacion-chatgpt.png)

*Tarjeta de confirmación de ChatGPT antes de un borrado · entorno de demostración*

**Claude**

![Confirmación que pide el asistente antes de una acción de escritura.](../../.gitbook/assets/2171043841-mcp-real-confirmacion-claude.png)

*Aviso de permiso de Claude antes de una modificación · entorno de demostración*

### Dar de alta un elemento

{% hint style="info" %}
```
Da de alta en el inventario el elemento [Plataforma de nóminas en la nube]
en la categoría [Software], con propietario [Dirección de RRHH] y la
descripción [Servicio SaaS de gestión de nóminas y portal del empleado].
```
{% endhint %}

*Herramientas: get\_categories · get\_elements · create\_element*

**ChatGPT**

![Respuesta real al dar de alta un elemento en el inventario.](../../.gitbook/assets/2171043841-mcp-real-e01-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real al dar de alta un elemento en el inventario.](../../.gitbook/assets/2171043841-mcp-real-e01-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Proponer y aplicar la valoración de un elemento

{% hint style="info" %}
```
Propón una valoración de confidencialidad, integridad y disponibilidad para
[Plataforma de nóminas en la nube] según los criterios de mi metodología.
Muéstramela en una tabla con la justificación y no la apliques hasta que te
lo confirme.
```
{% endhint %}

Cuando la revises:

{% hint style="info" %}
```
Aplícala.
```
{% endhint %}

*Herramientas: get\_methodology\_elements · update\_element\_dimension · calculate\_element\_dimensions*

**ChatGPT**

![Respuesta real con la propuesta de valoración de un elemento y su aplicación.](../../.gitbook/assets/2171043841-mcp-real-e02-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con la propuesta de valoración de un elemento y su aplicación.](../../.gitbook/assets/2171043841-mcp-real-e02-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

![Respuesta real con la propuesta de valoración de un elemento y su aplicación.](../../.gitbook/assets/2171043841-mcp-real-e02-claude-2.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Modificar un elemento

{% hint style="info" %}
```
Cambia el nombre de [Plataforma de nóminas en la nube] a [Plataforma de
nóminas y portal del empleado (SaaS)] y añade a su descripción que [el
proveedor está certificado en ISO 27001].
```
{% endhint %}

*Herramientas: get\_elements · update\_element*

**ChatGPT**

![Respuesta real al cambiar el nombre y la descripción de un elemento.](../../.gitbook/assets/2171043841-mcp-real-e03-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real al cambiar el nombre y la descripción de un elemento.](../../.gitbook/assets/2171043841-mcp-real-e03-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Añadir elementos a un análisis

{% hint style="info" %}
```
Añade [Plataforma de nóminas y portal del empleado (SaaS)] y [Servicio Help
Desk] al análisis [nombre].
```
{% endhint %}

*Herramientas: get\_elements · get\_elements\_by\_analysis · add\_element\_to\_analysis*

**ChatGPT**

![Respuesta real al añadir elementos a un análisis de riesgos.](../../.gitbook/assets/2171043841-mcp-real-e04-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real al añadir elementos a un análisis de riesgos.](../../.gitbook/assets/2171043841-mcp-real-e04-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Proponer y crear riesgos valorados

{% hint style="info" %}
```
Propón los tres riesgos más relevantes para [Plataforma de nóminas y portal
del empleado (SaaS)] en el análisis [nombre], con su probabilidad y su
impacto según los criterios de la metodología. Enséñamelos y, cuando te los
confirme, créalos y calcula su nivel de riesgo.
```
{% endhint %}

Cuando los revises:

{% hint style="info" %}
```
Adelante.
```
{% endhint %}

*Herramientas: get\_methodology\_fields · get\_methodology\_risks · create\_risk · update\_risk\_dimension · calculate\_risk\_dimensions*

**ChatGPT**

![Respuesta real con la propuesta de riesgos de un elemento y su creación.](../../.gitbook/assets/2171043841-mcp-real-e05-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con la propuesta de riesgos de un elemento y su creación.](../../.gitbook/assets/2171043841-mcp-real-e05-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

![Respuesta real con la propuesta de riesgos de un elemento y su creación.](../../.gitbook/assets/2171043841-mcp-real-e05-claude-2.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Crear un plan de tratamiento y asociarlo a los riesgos

{% hint style="info" %}
```
Para los riesgos de [Plataforma de nóminas y portal del empleado (SaaS)]
que superen el nivel de riesgo aceptable del análisis [nombre], crea un
plan de tratamiento con responsable [CISO], plazo [31/03/2027] y un coste
estimado razonable, y asócialo a esos riesgos.
```
{% endhint %}

*Herramientas: get\_element\_threats · create\_control · link\_control\_to\_risk*

En el ejemplo de Claude ningún riesgo superaba el nivel aceptable, así que no creó el plan y propuso uno para que lo confirmaras.

**ChatGPT**

![Respuesta real al crear un plan de tratamiento para los riesgos que superan el nivel aceptable.](../../.gitbook/assets/2171043841-mcp-real-e06-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real al crear un plan de tratamiento para los riesgos que superan el nivel aceptable.](../../.gitbook/assets/2171043841-mcp-real-e06-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Registrar acciones en un plan de tratamiento

{% hint style="info" %}
```
Añade a ese plan de tratamiento dos acciones: [Revisar el informe SOC 2 del
proveedor], con plazo [15/12/2026], y [Activar el inicio de sesión único
con MFA], con plazo [31/01/2027].
```
{% endhint %}

*Herramientas: create\_control\_action*

**ChatGPT**

![Respuesta real al registrar acciones en un plan de tratamiento.](../../.gitbook/assets/2171043841-mcp-real-e07-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real al registrar acciones en un plan de tratamiento.](../../.gitbook/assets/2171043841-mcp-real-e07-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Subir una evidencia

{% hint style="info" %}
```
Crea la evidencia [Certificado ISO 27001 del proveedor de nóminas], súbele
el archivo adjunto y vincúlala al plan de tratamiento de [la plataforma de
nóminas].
```
{% endhint %}

*Herramientas: create\_evidence · upload\_evidence\_file · link\_evidence\_to\_control*

En ChatGPT adjunta el fichero al mensaje. En Claude Code, indica el nombre del fichero de tu carpeta de trabajo.

**ChatGPT**

![Respuesta real al crear una evidencia, subir su fichero y vincularla a un control.](../../.gitbook/assets/2171043841-mcp-real-e08-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real al crear una evidencia, subir su fichero y vincularla a un control.](../../.gitbook/assets/2171043841-mcp-real-e08-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Recalcular un análisis

{% hint style="info" %}
```
Recalcula el análisis [nombre] y, cuando termine, dime qué elementos
superan el nivel de riesgo aceptable.
```
{% endhint %}

*Herramientas: recalculate\_analysis · get\_analysis\_calculation\_status · get\_elements\_by\_analysis*

**ChatGPT**

![Respuesta real al recalcular un análisis y revisar los elementos que superan el nivel aceptable.](../../.gitbook/assets/2171043841-mcp-real-e09-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real al recalcular un análisis y revisar los elementos que superan el nivel aceptable.](../../.gitbook/assets/2171043841-mcp-real-e09-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Sacar un elemento de un análisis

{% hint style="info" %}
```
El [Servicio Help Desk] ya no forma parte del alcance del análisis
[nombre]. Sácalo del análisis.
```
{% endhint %}

*Herramientas: get\_element\_threats · remove\_element\_from\_analysis*

Al sacar un elemento de un análisis se eliminan sus riesgos en ese análisis. En el ejemplo de Claude el elemento tenía un riesgo, así que Claude pidió confirmación antes de sacarlo.

**ChatGPT**

![Respuesta real al sacar un elemento del alcance de un análisis.](../../.gitbook/assets/2171043841-mcp-real-e10-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real al sacar un elemento del alcance de un análisis.](../../.gitbook/assets/2171043841-mcp-real-e10-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

![Respuesta real al sacar un elemento del alcance de un análisis.](../../.gitbook/assets/2171043841-mcp-real-e10-claude-2.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Eliminar un elemento del inventario

{% hint style="info" %}
```
Elimina del inventario el elemento [Servidor de nóminas antiguo (en
desmantelamiento)].
```
{% endhint %}

*Herramientas: get\_elements · delete\_element*

El borrado es permanente y no se puede deshacer. ChatGPT lo hace después de su tarjeta de confirmación; Claude no hace borrados permanentes y te propone marcar el elemento como obsoleto.

**ChatGPT**

![Respuesta real a la petición de eliminar un elemento del inventario.](../../.gitbook/assets/2171043841-mcp-real-e11-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real a la petición de eliminar un elemento del inventario.](../../.gitbook/assets/2171043841-mcp-real-e11-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

![Respuesta real a la petición de eliminar un elemento del inventario.](../../.gitbook/assets/2171043841-mcp-real-e11-claude-2.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

![Respuesta real a la petición de eliminar un elemento del inventario.](../../.gitbook/assets/2171043841-mcp-real-e11-claude-3.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Del diagnóstico a la acción: planes para los riesgos sin tratar

{% hint style="info" %}
```
Revisa los riesgos del análisis [nombre] que superan el nivel de riesgo
aceptable y no tienen ningún plan de tratamiento. Propón un plan para cada
uno (nombre, responsable, plazo y coste estimado) y, cuando te lo confirme,
créalos y asócialos.
```
{% endhint %}

Cuando los revises:

{% hint style="info" %}
```
Adelante, créalos.
```
{% endhint %}

*Herramientas: get\_elements\_by\_analysis · get\_element\_threats · get\_threat\_controls · create\_control · link\_control\_to\_risk*

**ChatGPT**

![Respuesta real con la propuesta y la creación de planes de tratamiento para los riesgos sin tratar.](../../.gitbook/assets/2171043841-mcp-real-e12-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con la propuesta y la creación de planes de tratamiento para los riesgos sin tratar.](../../.gitbook/assets/2171043841-mcp-real-e12-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

![Respuesta real con la propuesta y la creación de planes de tratamiento para los riesgos sin tratar.](../../.gitbook/assets/2171043841-mcp-real-e12-claude-2.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Alta masiva desde un Excel

{% hint style="info" %}
```
Da de alta en el inventario los elementos del Excel adjunto con su
valoración y añádelos al análisis [nombre]. Al terminar, dime cuáles se han
creado y si alguno ha fallado.
```
{% endhint %}

*Herramientas: get\_categories · create\_element · update\_element\_dimension · calculate\_element\_dimensions · add\_element\_to\_analysis*

**ChatGPT**

![Respuesta real al dar de alta y valorar los elementos de un Excel.](../../.gitbook/assets/2171043841-mcp-real-e13-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real al dar de alta y valorar los elementos de un Excel.](../../.gitbook/assets/2171043841-mcp-real-e13-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Valorar una dimensión multinivel

{% hint style="info" %}
```
Valora la dimensión [Tipos de datos tratados] del elemento [nombre] con
[Datos personales] y [Datos financieros].
```
{% endhint %}

*Herramientas: get\_methodology\_elements · update\_element\_dimension*

**PENDIENTE: CAPTURAS EN CHATGPT Y CLAUDE CUANDO SE CORRIJA LA VALORACIÓN DE DIMENSIONES MULTINIVEL DESDE EL MCP.**

## 10. Novedades de GlobalSuite®

### Novedades de una versión

{% hint style="info" %}
```
¿Qué novedades trae la versión [7.11] de GlobalSuite? Resúmelas por módulo
en una tabla.
```
{% endhint %}

*Herramientas: get\_changelog*

**ChatGPT**

![Respuesta real con las novedades de una versión de GlobalSuite resumidas por módulo.](../../.gitbook/assets/2171043841-mcp-real-c15-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con las novedades de una versión de GlobalSuite resumidas por módulo.](../../.gitbook/assets/2171043841-mcp-real-c15-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

### Cuándo llegó una funcionalidad

{% hint style="info" %}
```
¿En qué versión de GlobalSuite se incorporó [el módulo de
Automatizaciones]?
```
{% endhint %}

*Herramientas: search\_changelog*

**ChatGPT**

![Respuesta real con la versión en la que llegó una funcionalidad.](../../.gitbook/assets/2171043841-mcp-real-p14-chatgpt.png)

*Respuesta real en ChatGPT con el MCP GlobalSuite · entorno de demostración*

**Claude**

![Respuesta real con la versión en la que llegó una funcionalidad.](../../.gitbook/assets/2171043841-mcp-real-p14-claude.png)

*Respuesta real en Claude con el MCP GlobalSuite · entorno de demostración*

## Si la respuesta no es completa

GlobalSuite® entrega los resultados por páginas para no saturar al asistente. En preguntas sobre muchos datos —todo un análisis, todo el inventario o varias normativas—, el asistente puede quedarse con la primera página si no se le pide lo contrario. Para asegurarte de que la respuesta es completa:

* Pídele explícitamente que **revise todas las páginas de resultados** y que te diga cuántos registros ha analizado.
* **Acota la pregunta** a un análisis, una categoría, un elemento o un apartado de la normativa.
* Activa el **modo de investigación** de tu asistente, que dedica más tiempo y más consultas a recorrer toda la información antes de responder.

**Ten en cuenta:** los ejemplos de esta página se han obtenido con datos del entorno de demostración de GlobalSuite®. Las respuestas de tu asistente variarán según tus datos, tu metodología y el modelo de IA que utilices. Revisa siempre la información antes de tomar decisiones o de aplicar cambios.
