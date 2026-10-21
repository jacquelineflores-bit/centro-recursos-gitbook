# GlobalSuite API: casos de uso

## Qué es la API de GlobalSuite y cuándo utilizarla

La API de GlobalSuite permite conectar la plataforma con otros sistemas corporativos para consultar, crear, actualizar o relacionar información de negocio. En la práctica, evita trabajos manuales repetitivos y facilita que GlobalSuite se mantenga sincronizada con herramientas como CMDB, ITSM, soluciones de compras, repositorios documentales, data lakes, cuadros de mando o plataformas de cumplimiento.

|  |  |
| --- | --- |
| **Necesidad** | **Qué aporta la API** |
| Importar información | Crear o actualizar registros en GlobalSuite a partir de datos mantenidos en otro sistema, por ejemplo activos, empleados, proveedores o evidencias. |
| Consultar información | Extraer datos de GlobalSuite para analizarlos, consolidarlos o mostrarlos en otros sistemas corporativos. |
| Mantener relaciones | Vincular registros entre sí, por ejemplo proveedores con servicios, activos con amenazas, tickets con responsables o evidencias con controles. |
| Ejecutar procesos | Lanzar acciones o cálculos concretos, como solicitudes de cálculo de riesgo o cálculos de impacto asociados a continuidad. |
| Automatizar reporting | Preparar integraciones con repositorios de datos, dashboards o informes ejecutivos sin depender únicamente de exportaciones manuales. |

|  |
| --- |
| **Idea clave** La API no debe entenderse solo como una lista de endpoints técnicos. Cada endpoint representa una capacidad funcional de GlobalSuite: inventario, riesgos, tickets, proveedores, evidencias, procesos, servicios, usuarios o configuración. |

## Antes de empezar: acceso, seguridad y límites

Antes de diseñar una integración conviene validar cuatro aspectos: entorno, autenticación, alcance de datos y límites de uso.

|  |  |
| --- | --- |
| **Aspecto** | **Qué debe validarse** |
| Entorno de documentación | La documentación de referencia se consulta en Swagger UI. En demo Europa puede utilizarse https://demo-eu.globalsuitesolutions.com/docs. En otros entornos debe sustituirse por la URL publicada para el cliente o región correspondiente. |
| URL de integración | Las llamadas reales deben dirigirse a la URL de API del entorno correspondiente, por ejemplo https://api-demo-eu.globalsuitesolutions.com/v1/ para demo Europa. |
| API Key | Las llamadas autenticadas requieren una API Key o token con vigencia definida. Si la clave está fuera de su rango de validez, la API devolverá un error 403. |
| Subentidades | Si el cliente trabaja con varias subentidades, normalmente debe generarse una API Key específica para cada entidad que se quiera integrar, ya que los datos son propios de cada una. |
| Rate limit | El límite indicado en la página actual es de 180 llamadas por minuto por API Key. Si se supera, la API puede responder con 429 “Too Many Attempts”. |
| Versionado | La API se ofrece en versión Current. Si se produce un breaking change, la versión anterior puede pasar a Deprecated para dar margen a adaptar las integraciones. |

|  |
| --- |
| **Recomendación de arranque** Probar siempre en un entorno de demo o laboratorio antes de conectar sistemas productivos. El primer objetivo no debería ser automatizar todo, sino validar un flujo pequeño y controlado con datos representativos. |

## Cómo leer la documentación Swagger

Swagger UI muestra los modelos y operaciones disponibles. Para usuarios funcionales, lo importante no es memorizar la sintaxis, sino entender qué representa cada operación y qué impacto tiene sobre los datos.

|  |  |
| --- | --- |
| **Elemento** | **Cómo interpretarlo** |
| Recurso o modelo | Objeto de negocio de GlobalSuite: activo, ticket, proveedor, empleado, evidencia, servicio, proceso, control, etc. |
| Método GET | Consulta uno o varios registros. Suele utilizarse para listados, filtros, validaciones previas y extracción de datos. |
| Método POST | Crea un registro o ejecuta una acción de negocio. También puede utilizarse para asociar objetos o lanzar cálculos. |
| Método PUT | Actualiza un registro o una relación existente. Debe utilizarse con especial cuidado para no sobrescribir información. |
| Método DELETE | Elimina o desasocia un registro. Debe limitarse a procesos controlados y con validaciones previas. |
| Parámetros en ruta | Valores como {modelId}, {objectId}, {analysisId} o {riskId} identifican el registro concreto sobre el que se actúa. |
| Parámetros de consulta | Filtros, ordenación, paginación o relaciones ampliadas. En algunos listados puede usarse expand para traer información relacionada, si el endpoint lo permite. |

Referencia Swagger: [API GlobalSuite - Swagger UI](https://demo-eu.globalsuitesolutions.com/docs/)

## Casos de uso por área funcional

Los siguientes ejemplos sirven para entender qué problemas de negocio puede resolver la API y qué endpoints revisar en Swagger para aterrizar cada integración.

### 1. Sincronizar el inventario de activos desde una CMDB o herramienta ITSM

|  |  |
| --- | --- |
| **Objetivo de negocio** | Mantener en GlobalSuite un inventario actualizado de activos, categorías, dimensiones y dependencias sin realizar cargas manuales recurrentes. |
| **Ejemplo de escenario** | El equipo de IT mantiene servidores, aplicaciones o servicios técnicos en una CMDB. GlobalSuite necesita esos activos para análisis de riesgos, BIA, cumplimiento o reporting. |
| **Flujo recomendado** | 1) Consultar catálogos y dimensiones disponibles. 2) Buscar si el activo ya existe. 3) Crear o actualizar el activo. 4) Mantener dependencias y dimensiones. 5) Registrar trazabilidad en el sistema origen. |
| **Beneficio para el usuario** | Reduce la duplicidad de inventarios, mejora la calidad del dato y permite que análisis de riesgos, continuidad y cumplimiento partan de una base común. |

|  |  |  |
| --- | --- | --- |
| **Método** | **Endpoint** | **Uso orientativo** |
| **GET** | /assets | Consultar activos existentes y evitar duplicados. |
| **POST** | /assets | Crear nuevos activos que deben gestionarse en GlobalSuite. |
| **PUT** | /assets/{modelId} | Actualizar atributos de un activo ya existente. |
| **GET** | /categories | Consultar categorías de activos disponibles. |
| **GET** | /dimensions | Consultar dimensiones y niveles aplicables. |
| **POST** | /assets/{modelId}/dependency/{objectId} | Crear dependencias entre activos. |
| **PUT** | /assets/{modelId}/dimensions/{objectId} | Actualizar valores de dimensión del activo. |

|  |
| --- |
| **Recomendación** En activos y tickets pueden existir campos o estructuras configurables. El mapeo de datos debe validarse con la configuración concreta del cliente y con la documentación Swagger del entorno. |

### 2. Crear y actualizar tickets desde herramientas externas

|  |  |
| --- | --- |
| **Objetivo de negocio** | Conectar GlobalSuite con herramientas de soporte, auditoría, compliance o gestión de acciones para que los tickets se creen y mantengan sincronizados. |
| **Ejemplo de escenario** | Una herramienta externa detecta una incidencia, hallazgo o acción correctiva. La organización quiere gestionarla en GlobalSuite con responsables, evidencias, relaciones y seguimiento. |
| **Flujo recomendado** | 1) Identificar el tipo de ticket y sus campos. 2) Crear el ticket. 3) Asociar responsables, empleados, ficheros o relaciones. 4) Actualizar el ticket cuando cambie el estado en el sistema externo. |
| **Beneficio para el usuario** | Permite centralizar el seguimiento en GlobalSuite sin obligar a los equipos a introducir manualmente información que ya existe en otras herramientas. |

|  |  |  |
| --- | --- | --- |
| **Método** | **Endpoint** | **Uso orientativo** |
| **GET** | /ticketTypes | Consultar tipos de ticket disponibles. |
| **GET** | /ticketTypes/{modelId}/fields | Consultar campos configurados para un tipo de ticket. |
| **GET** | /tickets | Buscar tickets existentes o consultar su estado. |
| **POST** | /tickets | Crear un ticket nuevo. |
| **PUT** | /tickets/{modelId} | Actualizar datos del ticket. |
| **POST** | /tickets/{modelId}/owners/{objectId} | Asociar responsables al ticket. |
| **POST** | /tickets/{modelId}/files | Adjuntar documentación o evidencias al ticket. |
| **POST** | /tickets/{modelId}/ticketRelations/{objectId} | Relacionar el ticket con otros registros. |

|  |
| --- |
| **Recomendación** La API de tickets es amplia porque depende de tipos configurables, permisos, relaciones y campos dinámicos. Conviene empezar por un único tipo de ticket y ampliar después. |

### 3. Consultar análisis de riesgos y automatizar cálculos

|  |  |
| --- | --- |
| **Objetivo de negocio** | Extraer información de análisis de riesgos o lanzar cálculos desde procesos automatizados, por ejemplo para alimentar informes, auditorías o cuadros de mando. |
| **Ejemplo de escenario** | Un equipo necesita consolidar activos, amenazas, controles y riesgos en un repositorio corporativo o lanzar un recálculo cuando se actualiza información clave. |
| **Flujo recomendado** | 1) Identificar el análisis. 2) Consultar activos incluidos. 3) Consultar amenazas, controles y riesgos relacionados. 4) Ejecutar solicitudes de cálculo cuando proceda. 5) Explotar resultados en reporting. |
| **Beneficio para el usuario** | Mejora la trazabilidad del análisis, habilita automatización de reporting y reduce tiempos en revisiones periódicas de riesgos. |

|  |  |  |
| --- | --- | --- |
| **Método** | **Endpoint** | **Uso orientativo** |
| **GET** | /analysis/{modelId}/assets | Consultar activos incluidos en un análisis. |
| **GET** | /analysis/{modelId}/controls | Consultar controles asociados al análisis. |
| **POST** | /analysis/{modelId}/controls | Incorporar controles al análisis si aplica. |
| **POST** | /analysis/{modelId}/assets/{assetId}/threats/{threatId}/calculateRequest | Solicitar cálculo asociado a una amenaza. |
| **POST** | /analysis/{modelId}/calculateThreatSimulationRequest | Lanzar una simulación de amenazas. |
| **POST** | /analysis/{modelId}/calculateControlSimulationRequest | Lanzar una simulación de controles. |
| **GET** | /analysisCatalogs/{modelId}/threats/{threatId}/controls | Consultar controles de catálogo asociados a amenazas. |

|  |
| --- |
| **Recomendación** Las operaciones de cálculo deben tratarse como procesos de negocio. Antes de automatizarlas, conviene validar cuándo se deben ejecutar y qué datos quedan modificados o recalculados. |

### 4. Consolidar resultados de BIA y cálculos de impacto

|  |  |
| --- | --- |
| **Objetivo de negocio** | Automatizar cálculos relacionados con continuidad de negocio, como MTPD o RTO impactado, a partir de criterios configurados en GlobalSuite. |
| **Ejemplo de escenario** | La organización necesita recalcular impactos tras cambios en procesos, activos o dependencias, o consolidar resultados para reporting de continuidad. |
| **Flujo recomendado** | 1) Verificar la configuración BIA y los criterios de cálculo. 2) Enviar la petición de cálculo correspondiente. 3) Revisar el resultado en GlobalSuite y en los informes asociados. |
| **Beneficio para el usuario** | Ayuda a mantener actualizados los indicadores de continuidad sin depender únicamente de revisiones manuales. |

|  |  |  |
| --- | --- | --- |
| **Método** | **Endpoint** | **Uso orientativo** |
| **POST** | /calculateAccumulatedMtpd | Calcular MTPD acumulado. |
| **POST** | /calculateImpactedMtpd | Calcular MTPD impactado. |
| **POST** | /calculateImpactedRto | Calcular RTO impactado. |

|  |
| --- |
| **Recomendación** Estos cálculos dependen de la configuración funcional del BIA. Deben probarse con datos controlados antes de automatizar ejecuciones masivas. |

### 5. Sincronizar procesos, servicios y relaciones de negocio

|  |  |
| --- | --- |
| **Objetivo de negocio** | Conectar el mapa de procesos y servicios de GlobalSuite con inventarios corporativos, catálogos de servicios o repositorios de arquitectura empresarial. |
| **Ejemplo de escenario** | El área de negocio mantiene procesos y servicios en una herramienta corporativa, pero GlobalSuite los necesita para continuidad, riesgos, cumplimiento y cuadros de mando. |
| **Flujo recomendado** | 1) Consultar procesos y servicios existentes. 2) Crear o actualizar información básica cuando proceda. 3) Mantener empleados, stakeholders, entradas, acciones y salidas. 4) Consolidar métricas hacia reporting. |
| **Beneficio para el usuario** | Facilita una visión común entre gestión de servicios, continuidad, riesgos y reporting ejecutivo. |

|  |  |  |
| --- | --- | --- |
| **Método** | **Endpoint** | **Uso orientativo** |
| **GET** | /processes | Consultar procesos de negocio. |
| **GET** | /processes/{modelId} | Consultar el detalle de un proceso. |
| **GET** | /processes/{modelId}/employees | Consultar empleados asociados al proceso. |
| **GET** | /processes/{modelId}/inputActionOutput | Consultar entradas, acciones y salidas del proceso. |
| **GET** | /services | Consultar servicios. |
| **POST** | /services | Crear servicios. |
| **PUT** | /services/{modelId} | Actualizar datos de un servicio. |

|  |
| --- |
| **Recomendación** Conviene definir qué sistema es maestro para cada dato. La API debe sincronizar información, no generar conflictos entre fuentes. |

### 6. Mantener proveedores, acuerdos, servicios y SLAs

|  |  |
| --- | --- |
| **Objetivo de negocio** | Integrar la gestión de proveedores de GlobalSuite con herramientas de compras, TPRM, due diligence o sistemas maestros de terceros. |
| **Ejemplo de escenario** | Compras mantiene el maestro de proveedores, mientras GlobalSuite gestiona riesgos, evidencias, acuerdos, contactos, servicios afectados y seguimiento. |
| **Flujo recomendado** | 1) Buscar o crear proveedor. 2) Mantener contactos y acuerdos. 3) Asociar servicios y SLAs. 4) Adjuntar documentación. 5) Registrar trazas de seguimiento. |
| **Beneficio para el usuario** | Permite conectar gobierno de terceros, compras y riesgo operacional, evitando que los equipos mantengan datos de proveedores en silos separados. |

|  |  |  |
| --- | --- | --- |
| **Método** | **Endpoint** | **Uso orientativo** |
| **GET** | /suppliers | Consultar proveedores existentes. |
| **POST** | /suppliers | Crear un proveedor. |
| **PUT** | /suppliers/{modelId} | Actualizar información del proveedor. |
| **GET** | /suppliers/{modelId}/agreements | Consultar acuerdos del proveedor. |
| **POST** | /suppliers/{modelId}/contacts | Crear contactos asociados. |
| **POST** | /suppliers/{modelId}/files | Adjuntar documentación. |
| **GET** | /suppliers/{modelId}/services | Consultar servicios relacionados. |
| **POST** | /suppliers/{modelId}/slas | Crear SLAs del proveedor. |
| **POST** | /suppliers/{modelId}/tracings | Registrar seguimientos o trazas. |

|  |
| --- |
| **Recomendación** Antes de crear proveedores de forma automática, definir reglas de deduplicación: NIF/CIF, DUNS, nombre normalizado, país, grupo empresarial u otros identificadores disponibles. |

### 7. Gestionar evidencias y cumplimiento desde repositorios externos

|  |  |
| --- | --- |
| **Objetivo de negocio** | Automatizar la carga o actualización de evidencias y su asociación con controles, roles o empleados responsables. |
| **Ejemplo de escenario** | Un repositorio documental, herramienta de auditoría o solución de compliance genera evidencias que deben vincularse con controles gestionados en GlobalSuite. |
| **Flujo recomendado** | 1) Consultar tipos de evidencia. 2) Crear o actualizar evidencia. 3) Adjuntar archivos si procede. 4) Asociar la evidencia a controles y responsables. 5) Revisar trazabilidad y permisos. |
| **Beneficio para el usuario** | Mejora la preparación de auditorías y reduce la pérdida de evidencias dispersas en carpetas o herramientas no conectadas. |

|  |  |  |
| --- | --- | --- |
| **Método** | **Endpoint** | **Uso orientativo** |
| **GET** | /evidenceTypes | Consultar tipos de evidencia. |
| **GET** | /evidences | Buscar evidencias existentes. |
| **POST** | /evidences | Crear una evidencia. |
| **PUT** | /evidences/{modelId} | Actualizar una evidencia. |
| **POST** | /evidences/{modelId}/files | Adjuntar ficheros a la evidencia. |
| **POST** | /evidences/{modelId}/controls/{objectId} | Asociar evidencia a un control. |
| **POST** | /evidences/{modelId}/roles/{objectId}/employees/{employeeId} | Asignar empleados a roles relacionados con la evidencia. |

|  |
| --- |
| **Recomendación** La integración debe respetar permisos, sensibilidad documental y criterios de vigencia de evidencias. |

### 8. Mantener usuarios, empleados y roles alineados

|  |  |
| --- | --- |
| **Objetivo de negocio** | Asegurar que las personas y roles usados en GlobalSuite están alineados con fuentes corporativas de identidad o recursos humanos. |
| **Ejemplo de escenario** | RR. HH. o IAM mantiene altas, bajas y cambios de empleados. GlobalSuite necesita esos datos para responsables, permisos, filtros, aprobaciones o asignaciones en módulos funcionales. |
| **Flujo recomendado** | 1) Consultar empleados y usuarios existentes. 2) Crear o actualizar registros. 3) Revisar roles y asignaciones. 4) Gestionar bajas de forma controlada. |
| **Beneficio para el usuario** | Evita desalineaciones entre personas reales, responsables funcionales y usuarios dados de alta en GlobalSuite. |

|  |  |  |
| --- | --- | --- |
| **Método** | **Endpoint** | **Uso orientativo** |
| **GET** | /users | Consultar usuarios de la aplicación. |
| **POST** | /users | Crear usuarios si el flujo definido lo permite. |
| **PUT** | /users/{modelId} | Actualizar datos de un usuario. |
| **GET** | /employees | Consultar empleados. |
| **POST** | /employees | Crear empleados. |
| **PUT** | /employees/{modelId} | Actualizar datos de un empleado. |
| **GET** | /configRoles | Consultar roles configurados. |

|  |
| --- |
| **Recomendación** Si se usa SCIM u otro flujo de identidad, la API debe plantearse como complemento y no como mecanismo paralelo que genere incoherencias. |

## Diseño recomendado de una integración

Para pasar de un caso de uso a una integración estable, se recomienda seguir un enfoque incremental:

1. Definir el objetivo funcional: qué dato se quiere consultar, crear, actualizar o relacionar y por qué aporta valor al proceso.
2. Identificar el sistema maestro de cada dato: por ejemplo, CMDB para activos técnicos, compras para proveedores o IAM para usuarios.
3. Revisar el modelo en Swagger: campos obligatorios, parámetros, ejemplos de respuesta, errores y relaciones disponibles.
4. Preparar el mapeo de datos: equivalencias entre campos del sistema origen y campos de GlobalSuite, incluyendo catálogos, dimensiones y valores configurables.
5. Validar permisos y alcance de la API Key: entidad, subentidad, vigencia, operaciones permitidas y datos visibles.
6. Probar con un subconjunto reducido: pocos registros, entorno de demo y validación funcional por usuarios clave.
7. Incorporar controles técnicos: paginación, reintentos, tratamiento de errores 403/429, logs y alertas de integración.
8. Documentar la integración: responsable, frecuencia, endpoints usados, reglas de deduplicación, sistema maestro y procedimiento ante errores.

|  |
| --- |
| **Patrón recomendado** En integraciones de alta criticidad, utilizar primero GET para validar el estado actual, después POST solo si el registro no existe y PUT únicamente cuando se haya confirmado el registro objetivo. Este patrón reduce duplicados y actualizaciones no deseadas. |

## Buenas prácticas de explotación

|  |  |
| --- | --- |
| **Práctica** | **Por qué es importante** |
| Una API Key por integración | Facilita trazabilidad, revocación y control de límites. Evita reutilizar la misma clave para procesos con finalidades distintas. |
| Rotación periódica de claves | Planificar renovación antes de la fecha de caducidad para evitar interrupciones. |
| Control del rate limit | Agrupar llamadas, paginar correctamente y espaciar procesos batch para no superar 180 llamadas por minuto por API Key. |
| No automatizar DELETE sin validación | Las eliminaciones o desasociaciones deben requerir controles adicionales o flujos de aprobación. |
| Registrar trazabilidad | Guardar en logs qué se envió, cuándo, por qué endpoint y cuál fue la respuesta. |
| Diseñar reglas de deduplicación | Antes de crear registros, buscar coincidencias por identificadores funcionales. |
| Validar catálogos y configuración | No asumir que categorías, campos, dimensiones o tipos de ticket son iguales en todos los clientes. |
| Gestionar errores de negocio | Distinguir errores de autenticación, permisos, límites, validación de datos y recursos no encontrados. |

## Mapa de áreas funcionales y endpoints

La siguiente tabla resume las áreas funcionales identificadas en la guía comercial y muestra ejemplos de endpoints que pueden revisarse en Swagger. No es un catálogo exhaustivo de parámetros ni de respuestas.

|  |  |  |
| --- | --- | --- |
| **Área funcional** | **N.º ops.** | **Ejemplos de endpoints** |
| Usuarios y seguridad de cuenta | 5 | GET /users, POST /users, GET /users/{modelId}, DELETE /users/{modelId}... |
| Tickets | 28 | GET /tickets, POST /tickets, GET /tickets/{modelId}, PUT /tickets/{modelId}... |
| Activos (inventario) | 32 | GET /assetAttributes, GET /assetAttributes/{modelId}, GET /assets, POST /assets... |
| Análisis de riesgos | 23 | GET /analysis/{modelId}/assets, POST /analysis/{modelId}/assets/{assetId}/controls/{controlId}/calculateRequest, POST /analysis/{modelId}/assets/{assetId}/threats/{threatId}/calculateRequest, GET /analysis/{modelId}/assets/{assetId}/threats/{threatId}/controls... |
| BIA, encuestas y cálculos de impacto | 3 | POST /calculateAccumulatedMtpd, POST /calculateImpactedMtpd, POST /calculateImpactedRto |
| Procesos, servicios y consolidación | 12 | GET /processes, GET /processes/{modelId}, GET /processes/{modelId}/employees, GET /processes/{modelId}/inputActionOutput... |
| Empleados y roles | 12 | GET /configRoles, GET /employees, POST /employees, GET /employees/{modelId}... |
| Empresas | 5 | POST /companies/copyCompany, GET /companies/{modelId}/analysis, PUT /companies/{modelId}/analysis, GET /companies/{modelId}/roles... |
| Cumplimiento ENS y evaluaciones | 17 | PUT /controls/{modelId}, GET /evidenceTypes, GET /evidences, POST /evidences... |
| Cuadros de mando | 1 | GET /dashboard/{modelId}/updatedDate/{objectId} |
| Informes, métricas y proyectos | 1 | DELETE /testplans/{modelId}/processes/{objectId} |
| Proveedores | 30 | GET /suppliers, POST /suppliers, PUT /suppliers/{modelId}, GET /suppliers/{modelId}... |
| Catálogos y árbol de riesgos | 1 | GET /risks |
| Configuración, metodología y reglas | 11 | GET /connectionsPrefixes, GET /controlLevels, GET /controlLevels/{modelId}, GET /methodologies/{modelId}... |

## Ayuda y referencias

* La documentación Swagger debe ser la referencia final para parámetros obligatorios, estructura del cuerpo de petición, respuestas y errores.
* Antes de utilizar la API, conviene revisar el Manual de Usuario de GlobalSuite para entender la lógica funcional del módulo que se vaya a integrar.
* Si un endpoint no responde como se espera, validar primero API Key, entorno, entidad/subentidad, permisos, rate limit y datos de prueba.
* Para dudas o incidencias, canalizar la consulta a través del proveedor o del Centro de Soporte a Clientes de GlobalSuite.

Enlaces de referencia:

[Swagger demo Europa](https://demo-eu.globalsuitesolutions.com/docs/)

[Manual de Usuario GlobalSuite](https://help.globalsuitesolutions.com/es/globalsuite/v1/)

[Changelog GlobalSuite](https://changelog.globalsuitesolutions.com/changelog/)
