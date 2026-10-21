# Kafka Connect IBM MQ Sink for z-OS Connector

|  |  |
| --- | --- |
|  | **Conector para enviar desde GlobalSuite mensajes, eventos y notificaciones de negocio hacia IBM MQ for z/OS o hacia el sistema destino definido.**  **Etiquetas:** Mensajería | Integración | Sink |

|  |  |
| --- | --- |
| Herramienta o sistema | IBM MQ for z/OS |
| Fabricante de la herramienta | IBM |
| Proveedor del conector | Confluent, Inc |
| Nombre del conector | Kafka Connect IBM MQ Sink for z/OS Connector |
| Tipo de conector | Sink |
| Etiquetas | Mensajería | Integración | Sink |
| Información que maneja | mensajes, eventos y notificaciones de negocio |

## Detalles

El conector Kafka Connect IBM MQ Sink for z/OS Connector permite enviar desde GlobalSuite hacia IBM MQ for z/OS información relacionada con mensajes, eventos y notificaciones de negocio.

Es útil cuando IBM MQ for z/OS debe actuar como sistema de destino, explotación, archivo o monitorización para casos de orquestación entre aplicaciones, alertas operativas, integración con sistemas legacy y automatización de procesos.

## Características

* Envío controlado de mensajes, eventos y notificaciones de negocio desde GlobalSuite hacia IBM MQ for z/OS o hacia el repositorio destino definido.
* Tratamiento de mensajes o eventos de aplicaciones corporativas, sistemas legacy o servicios de negocio.
* Configuración de colas, canales o filtros para dirigir cada evento al proceso correspondiente.
* Soporte a automatizaciones, notificaciones, conciliaciones y coordinación entre sistemas.
* Trazabilidad de entrega y errores para facilitar seguimiento operativo y soporte.

## Beneficios clave

* Conecta aplicaciones corporativas y sistemas legacy sin depender de integraciones punto a punto difíciles de mantener.
* Permite automatizar avisos, eventos y cambios de estado entre áreas o herramientas.
* Reduce esperas y reprocesos en flujos operativos donde varias aplicaciones deben coordinarse.
* Mejora la trazabilidad de entregas y errores para soporte y continuidad del servicio.
* Facilita incorporar sistemas existentes a procesos de GlobalSuite sin rediseñar todo el ecosistema.

## Instalación

|  |
| --- |
| **Nota de configuración:** Antes de activar la integración, valida credenciales, permisos, alcance funcional y una prueba de datos con el área responsable. |

1. Accede al Marketplace de GlobalSuite® y selecciona Kafka Connect IBM MQ Sink for z/OS Connector.
2. Configura el destino en IBM MQ for z/OS: URL o endpoint, credenciales, permisos y entorno.
3. Define qué información se enviará: mensajes, eventos y notificaciones de negocio, filtros, formato y periodicidad.
4. Mapea los campos de GlobalSuite con la estructura esperada por el sistema destino.
5. Ejecuta una prueba, revisa la recepción en destino y activa la integración.

## Más información

<https://www.ibm.com/products/mq>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando necesites enviar información de GlobalSuite a IBM MQ for z/OS, por ejemplo para orquestación entre aplicaciones, alertas operativas, integración con sistemas legacy y automatización de procesos. Antes de publicarlo, valida con el equipo propietario del sistema destino el formato esperado, permisos, frecuencia y criterios de calidad.
