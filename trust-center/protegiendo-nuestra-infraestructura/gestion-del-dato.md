# Gestión del dato

## Soberanía del dato

En GlobalSuite concebimos la soberanía del dato como la capacidad de nuestros clientes para mantener el **control efectivo sobre el uso de su información**, garantizando que los datos se utilizan **exclusivamente para los fines necesarios para la prestación de los servicios contratados** y no son objeto de **usos secundarios no autorizados**, como el entrenamiento de modelos de inteligencia artificial, su reutilización con otros fines o cualquier tratamiento ajeno a la operación del servicio.

Este compromiso se fundamenta en el principio de **limitación de la finalidad** y se integra de manera transversal en nuestros procesos técnicos, organizativos y contractuales. En consecuencia, los datos de cliente no se emplean para finalidades adicionales o analíticas no esenciales, salvo que exista una **autorización expresa, específica y documentada** por parte del cliente, cuando sea legalmente procedente.

## Localización del dato

Los datos gestionados por GlobalSuite se almacenan y procesan **exclusivamente dentro de la Unión Europea**, sin que nuestros tratamientos requieran la realización de transferencias internacionales de datos.

La información se aloja en centros de datos ubicados en distintas regiones europeas, operados por proveedores de primer nivel como **Digital Realty**, **Amazon Web Services (AWS)** en sus regiones europeas y **Microsoft Azure** en regiones igualmente situadas dentro de la UE.

Este modelo garantiza que los datos permanecen bajo **jurisdicción europea** y sujetos al marco normativo aplicable en materia de protección de datos.

[Ver subencargados de tratamiento.](../compliance-y-gestion-de-riesgos/encargados-de-tratamiento-de-datos-personales.md)

## Arquitectura de almacenamiento de información

Para asegurar su disponibilidad, nuestra información se encuentra en nuestros [centros de datos](descripcion-general-de-la-infraestructura.md).

Disponemos de una arquitectura compuesta por distintos nodos de almacenamiento lo cual nos brinda una adecuada capacidad de procesamiento y garantiza la disponibilidad del dato, proporcionando una primera línea de protección contra riesgos medioambientales o desastres naturales contra una o varias zonas de disponibilidad.

## Backups y Recuperación de Datos

Disponemos de procesos de respaldo de información que permiten recuperar los datos ante un incidente de seguridad.

Las copias de seguridad de GlobalSuite siguen una estrategia 3-2-1-0. Esto implica mantener al menos tres copias de cada dato, almacenadas en dos tipos de soportes o ubicaciones distintas, con al menos una copia en un emplazamiento alternativo y garantizando, además, que todas las copias han sido verificadas y están libres de errores (*zero errors*) antes de considerarse válidas.

Las copias de seguridad están cifradas en reposo mediante AES-256 y almacenadas en repositorios inmutables que garantizan la integridad de los datos y previenen su eliminación o manipulación por parte de actores malintencionados o software no autorizado.

Todas las copias se someten a procesos de validación periódicos para asegurar su consistencia y su correcta restauración en caso necesario. Las instantáneas se retienen durante 30 días, en línea con nuestra estrategia de continuidad y con un RPO inferior a 12 horas.

Para reforzar la seguridad del entorno de respaldo, la infraestructura de copias de seguridad opera sobre redes segregadas y el servicio de backup y replicación incorpora capacidades avanzadas de detección de malware, contribuyendo a la protección temprana frente a amenazas.

## Datos en el proceso de desarrollo

En GlobalSuite Solutions aplicamos una estrategia de desarrollo seguro diseñada para garantizar que la información de nuestros clientes permanece protegida en todas las fases del ciclo de vida del software. Uno de los principios fundamentales de esta estrategia es que **ningún dato real de producción se utiliza en entornos no productivos**, como desarrollo, pruebas o validaciones preproductivas.

Todos los datos empleados en estos entornos son **datos desnaturalizados, anonimizados o generados sintéticamente**, para evitar cualquier posibilidad de exposición de información confidencial o sensible. Como medida preventiva adicional, el equipo de desarrollo **no tiene acceso directo a los datos productivos**, y solo personal estrictamente autorizado del área de operaciones, bajo procedimientos controlados y auditados, puede acceder a ellos cuando es imprescindible para la continuidad del servicio.

La infraestructura de desarrollo, pruebas y producción se encuentra completamente **segregada**, tanto a nivel lógico como a nivel de red. Esto garantiza que el movimiento lateral entre entornos sea imposible y que cualquier proceso automatizado (como CI/CD) opere exclusivamente con artefactos y datos no sensibles.

Todo acceso y actividad sobre entornos relacionados con datos, independientemente de si son productivos o no, queda **registrado, monitorizado y sujeto a auditoría**, lo que garantiza trazabilidad total y capacidad de detección temprana de comportamientos anómalos.

Además, los procesos de construcción y despliegue de software integran controles de seguridad continua: revisiones de código, análisis automatizados, validaciones, pruebas y controles de integridad que aseguran que el tratamiento de datos en el proceso de desarrollo sea siempre seguro, controlado y alineado con los estándares más exigentes de protección.

Con este conjunto de medidas garantizamos que, incluso durante el desarrollo interno de la plataforma, los datos de nuestros clientes están completamente protegidos y se mantienen bajo principios estrictos de confidencialidad, integridad y minimización.
