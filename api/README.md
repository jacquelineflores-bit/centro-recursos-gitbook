# GlobalSuite® API

{% hint style="info" %}
Bienvenido a la API de GlobalSuite®, la solución GRC para optimizar los procesos de riesgos, seguridad, continuidad, auditoría y compliance en su negocio.
{% endhint %}

Mediante el uso de las APIs, puede integrar GlobalSuite® con el resto de aplicaciones, herramientas o sistemas de su ecosistema corporativo. Por ejemplo:

* Puede automatizar la importación de activos desde otras herramientas.
* Sincronizar información para exportarlos en otra herramienta para su gestión.
* Exportar registros para almacenarlos en un repositorio, o lago de datos (EDL).

Puede consultar la API de GlobalSuite® mediante el repositorio de documentación [API GlobalSuite®](https://demo-eu.globalsuitesolutions.com/docs/). También se puede realizar pruebas directamente para verificar las operaciones que proporciona, tanto de lectura, escritura, modificación o eliminación de datos.

NOTA: Si quiere comenzar a utilizar las APIs de GlobalSuite® póngase en contacto con su proveedor.

Existen entornos de demo que se pueden solicitar para revisar y realizar pruebas de integración sobre las APIs disponibles:

**Europa**:

* **URL (documentación API)**:

  * <https://demo-eu.globalsuitesolutions.com/docs>
* **URL (integración API)**:

  * <https://api-demo-eu.globalsuitesolutions.com/v1/>

**Latam**:

* **URL (documentación API)**:

  * <https://demo-la.globalsuitesolutions.com/docs>
* **URL (integración API)**:

  * [https://api-demo-eu.globalsuitesolutions.com/v1/](https://api-demo-la.globalsuitesolutions.com/v1/)

## Habilitar API Key

Las APIs de GlobalSuite® se utilizan de forma segura, previniendo usos no autorizados de las mismas. Para ello, es necesario crear una API Key o token que permita realizar las llamadas de forma autenticada.

Estas API Keys se generan con una validez o vigencia concreta (un rango de fechas) especificado por el cliente o integrador. Antes o después de las fechas indicadas, el API Key no será válido, y las llamadas a los endpoints devolverán el siguiente mensaje de error 403:

![](https://globalsuitesolutions.atlassian.net/wiki/download/attachments/266731551/image2021-9-2_11-38-45.png%3Fversion=1&modificationDate=1633944215000&cacheVersion=1&api=v2)

{% hint style="info" %}
\*\*NOTA\*\*: En la documentación de Swagger [API GlobalSuite®](https://demo-eu.globalsuitesolutions.com/docs/) puede consultar el listado de endpoints habilitados mediante este mecanismo.
{% endhint %}

#### Subentidades

En caso de tener habilitadas varias [Subentidades](https://help.globalsuitesolutions.com/es/globalsuite/v1/subentidades) en GlobalSuite®, se deberá generar un API Key específica para cada entidad que se quiera integrar con una herramienta o servicio propio o de terceros.

En GlobalSuite® la configuración es común a nivel de todas las entidades de una empresa, pero los datos y registros son específicos de cada una, por lo que si se quiere integrar un repositorio de información con algún apartado de la herramienta (por ejemplo, Inventario de Elementos) se deberá crear un API Key para cada entidad, ya que los elementos dados de alta con esa API Key, se crearán en la entidad que tenga configurada.

NOTA: Si no se dispone de múltiples entidades, no será necesario definir varias claves.

#### Buenas prácticas y consejos

* Asegúrese de utilizar un único API Key por aplicación o integración realizada.
* Cambie periódicamente el API Key utilizado para mayor seguridad.

## Usar la Documentación de API

En la documentación de la [API GlobalSuite®](https://demo-eu.globalsuitesolutions.com/docs/), se muestran los distintos items o modelos que se pueden consumir de manera automatizada.

Cada uno de estos recursos es una representación simbólica de un objeto del dominio de negocio de GlobalSuite®. Por ejemplo un Servicio, un Empleado, etc.

![](https://globalsuitesolutions.atlassian.net/wiki/download/attachments/266731551/image2021-7-5_10-40-22.png%3Fversion=1&modificationDate=1633944215000&cacheVersion=1&api=v2&width=859)

Para cada uno de los modelos, es posible consultar los endpoints u operaciones GET, PUT, POST y DELETE que estén permitidas:

![](https://globalsuitesolutions.atlassian.net/wiki/download/attachments/266731551/image2021-7-5_10-54-17.png%3Fversion=1&modificationDate=1633944215000&cacheVersion=1&api=v2&width=862)

Estos endpoints corresponden a las operaciones básicas CRUD (Create, Read, Update and Delete):

* GET: Endpoint para obtener uno o varios de los modelos a consultar, pudiendo realizar filtrados de dichas consultas.
* POST: Endpoint para crear un nuevo registro de un modelo concreto.
* PUT: Endpoint para modificar o actualizar alguno de los valores o campos del modelo.
* DELETE: Endpoint para eliminar un registro concreto del modelo.

La documentación de cada uno de estos endpoints incluye los parámetros, obligatorios u opcionales, que se pueden incluir en cada llamada:

![](https://globalsuitesolutions.atlassian.net/wiki/download/attachments/266731551/image2021-7-5_10-52-42.png%3Fversion=1&modificationDate=1633944215000&cacheVersion=1&api=v2&width=862)

También, en el propio explorador, se ven ejemplos de respuesta que se proporcionan en cada caso, incluyendo las respuestas correctas, o los mensajes de error en su caso.

![](https://globalsuitesolutions.atlassian.net/wiki/download/attachments/266731551/image2021-7-5_10-26-22.png%3Fversion=1&modificationDate=1633944215000&cacheVersion=1&api=v2&width=862)![](https://globalsuitesolutions.atlassian.net/wiki/download/attachments/266731551/image2021-7-5_10-49-13.png%3Fversion=1&modificationDate=1633944215000&cacheVersion=1&api=v2&width=862)

## Utilizar un cliente REST

Para realizar las llamadas a la API de GlobalSuite®, es posible utilizar distintos clientes que realicen las llamadas HTTP al servidor de GlobalSuite®. Es posible realizar tanto llamadas sencillas, como procesos más complejos utilizando algunas herramientas como cURL o [Postman](https://www.postman.com/).

![](https://globalsuitesolutions.atlassian.net/wiki/download/attachments/266731551/image2021-7-5_10-8-40.png%3Fversion=1&modificationDate=1633944215000&cacheVersion=1&api=v2&width=1188)

## Rate Limit

Para evitar problemas de rendimiento, o ataques de fuerza bruta del tipo DDoS o similar, se ha implementado un mecanismo de rate limit, que restringe el número de llamadas a la API que se pueden realizar en un período de tiempo.

Este límite es general, por lo que se tienen en cuenta el total de llamadas realizadas con el mismo API-Key aunque sean llamadas a distintos endpoints o registros.

Actualmente ese límite es de **180 llamadas en un minuto**.

En caso de superar ese límite, las siguientes llamadas devolverán el mensaje de error 429 "Too Many Attempts", para indicar que se ha superado la tasa límite, y será necesario esperar para poder continuar utilizándola.

![](https://globalsuitesolutions.atlassian.net/wiki/download/attachments/266731551/image2022-4-13_13-26-12.png%3Fversion=8&modificationDate=1693487682000&cacheVersion=1&api=v2&width=291)

## Ayuda: Documentación de Referencia

* Antes de utilizar las APIs de GlobalSUITE®, recomendamos familiarizarse con el [Manual de Usuario GlobalSuite®](https://help.globalsuitesolutions.com/es/globalsuite/v1/), ya que hay una gran relación entre la lógica de negocio y la API.
* Si se tiene alguna duda o posible problema con alguno de los endpoints disponibles en la [Documentación API GlobalSuite®](https://demo-eu.globalsuitesolutions.com/docs/), puede ponerse en contacto con nuestro [Centro de Soporte a Clientes](https://support.globalsuite.es/servicedesk/customer/user/login?destination=portals).
* Use la documentación de API de GlobalSuite® para encontrar referencias para la última versión disponible de la API REST.

## Certificación de seguridad GlobalSUITE® (CSWA)

Como parte del ciclo de mejora continua en nuestros procesos de desarrollo utilizados en GlobalSuite® hemos realizado una validación externa a través de una **auditoría de seguridad de Hacking Ético**.

Esta verificación ha sido llevada a cabo según los estándares **OWASP Top Ten 2017** y **API Security Top 10 2019**, integrando los controles propuestos por ambos estándares en nuestros procesos de verificación y cumplimiento.

Este proceso de auditoría ha permitido certificar la seguridad y resiliencia de GlobalSUITE®, trayendo consigo el **certificado CSWA**, en nuestros entornos SaaS y On Premise.

![](https://globalsuitesolutions.atlassian.net/wiki/download/attachments/266731551/unnamed.png%3Fversion=1&modificationDate=1633944215000&cacheVersion=1&api=v2&height=250)

## Versionado de API

Como parte del mantenimiento y servicio de las APIs que ofrece GlobalSuite® se incluye la gestión de versiones y el control de cambios de las mismas.

La API se ofrece siempre en su versión más actualizada (**Current**) que estará vigente hasta que se realice un evolutivo del producto que suponga un Breaking Change.

Este breaking change es una actualización que modifica la estructura de llamadas y/o respuestas de alguno de los endpoints ofrecidos.

En caso de que se produzca esta situación, la versión anterior pasará a un estado **Deprecated**, pero seguirá siendo accesible hasta que se vuelva a producir otro breaking change, para poder realizar adaptaciones (en caso de que sea necesario) para mantener las integraciones realizadas.

Las actualizaciones de versiones de GlobalSuite® serán notificadas en la propia herramienta tras una actualización y se podrán consultar en cualquier momento en el [Changelog GlobalSuite®](https://globalsuitesolutions.atlassian.net/wiki/spaces/CG)

#### Listado de versiones de API GlobalSuite®

| Versión | Publicación | Estado | Descripción |
| --- | --- | --- | --- |
| v0 | Octubre 2021 | Deprecated | Versión inicial del API. Disponible API de [Inventario](https://globalsuitesolutions.atlassian.net/wiki/spaces/GlobalSUITEes/pages/266864248/Inventario) |
| v1 | Abril 2022 | Current | Normalización de endpoints y verbos PUT/POST  Disponible API de [Controles](https://globalsuitesolutions.atlassian.net/wiki/spaces/GlobalSUITEes/pages/266864116/Gesti+n+de+Controles) |
|  | Abril 2023 |  | Disponible API de [Tickets](https://globalsuitesolutions.atlassian.net/wiki/spaces/GlobalSUITEes/pages/266863860/Tickets) |
|  | Julio 2023 |  | Disponible API de [Usuarios](https://globalsuitesolutions.atlassian.net/wiki/spaces/GlobalSUITEes/pages/266863797/Usuarios) |
|  | Diciembre 2023 |  | Disponible API de [Análisis de Riesgos](https://globalsuitesolutions.atlassian.net/wiki/spaces/GlobalSUITEes/pages/266863420/An+lisis+de+Riesgos) |
|  | Junio 2026 |  | Disponible API de [Gestor Documental](https://globalsuitesolutions.atlassian.net/wiki/spaces/GlobalSUITEes/pages/266864205/Gestor+Documental) |
