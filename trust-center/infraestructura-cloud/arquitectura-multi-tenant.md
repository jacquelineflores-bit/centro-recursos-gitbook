# Arquitectura Multi-Tenant

Nuestros productos se encuentran implementados en una arquitectura SaaS multi-tenant. Esto quiere decir que cada uno de nuestros clientes, que denominaremos “tenants”, accederá a una versión de la aplicación que contendrá sus configuraciones y datos, mientras se comparte la infraestructura subyacente.

Si bien es cierto que se comparte parte de la infraestructura, en todo caso se garantizan los recursos, la seguridad y la privacidad. Dependiendo del modelo de licenciamiento escogido se podrán tener recursos aislados de cómputo, almacenamiento o configuración para adaptarse a las necesidades de nuestros clientes.

Dentro del aplicativo, cada tenant dispondrá de una serie de configuraciones, información y preferencias en su instancia, que serán únicas para él y que es lo que conocemos como “Contexto del Tenant”.

### ¿Qué es el contexto del tenant?

En un entorno multi-tenant, el contexto del tenant se refiere a la información y las configuraciones específicas de GlobalSuite de un inquilino particular dentro de un sistema que comparte ciertos recursos. Este concepto permite que cada tenant tenga sus datos y configuraciones aisladas mientras se comparte la infraestructura subyacente.

¿Qué incluye este contexto del Tenant en GlobalSuite?

* **Datos del Tenant:** Cada tenant tiene su propio conjunto de datos, aislados de los del resto de tenants, asegurando la privacidad y seguridad de la información.
* **Configuraciones del Tenant:** Es posible que cada tenant disponga de ciertas configuraciones específicas: filtrado de IPs, rutas de acceso personalizadas, aspectos parametrizados de look and feel, integraciones con elementos de infraestructura, preferencias de usuario, etc.
* **Autenticación y autorización:** El contexto del tenant ayuda a gestionar la autenticación y autorización, asegurando que los usuarios únicamente tengan acceso a los datos y funcionalidades permitidas dentro de su propio tenant incluyendo, por ejemplo, servicios de gestión de identidades.
* **Aislamiento de seguridad:** El contexto del tenant implica un aseguramiento de datos en términos de seguridad para que los tentant no puedan acceder a datos o configuraciones de otros tenant.

Nuestros servicios seguirán principalmente dos tipos de arquitectura, no obstante ambos disponen de mecanismos para aislar los datos de cada tenant para garantizar la seguridad y la privacidad.
