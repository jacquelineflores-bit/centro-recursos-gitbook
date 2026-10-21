# Rabbit MQ Sink Connector

|  |  |
| --- | --- |
|  | **Conector para enviar desde GlobalSuite mensajes, eventos y notificaciones de negocio hacia Rabbit MQ o hacia el sistema destino definido.**  **Etiquetas:** Integración | Sink | Mensajería | Cloud |

|  |  |
| --- | --- |
| Herramienta o sistema | Rabbit MQ |
| Fabricante de la herramienta | Confluent Cloud |
| Proveedor del conector | Confluent Cloud |
| Nombre del conector | Rabbit MQ Sink Connector |
| Tipo de conector | Sink |
| Etiquetas | Integración | Sink | Mensajería | Cloud |
| Información que maneja | mensajes, eventos y notificaciones de negocio |

## Detalles

El conector Rabbit MQ Sink Connector permite enviar desde GlobalSuite hacia Rabbit MQ información relacionada con mensajes, eventos y notificaciones de negocio.

Es útil cuando Rabbit MQ debe actuar como sistema de destino, explotación, archivo o monitorización para casos de orquestación entre aplicaciones, alertas operativas, integración con sistemas legacy y automatización de procesos.

## Características

* Envío controlado de mensajes, eventos y notificaciones de negocio desde GlobalSuite hacia Rabbit MQ o hacia el repositorio destino definido.
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

1. Accede al Marketplace de GlobalSuite® y selecciona Rabbit MQ Sink Connector.
2. Configura el destino en Rabbit MQ: URL o endpoint, credenciales, permisos y entorno.
3. Define qué información se enviará: mensajes, eventos y notificaciones de negocio, filtros, formato y periodicidad.
4. Mapea los campos de GlobalSuite con la estructura esperada por el sistema destino.
5. Ejecuta una prueba, revisa la recepción en destino y activa la integración.

## Más información

<https://www.rabbitmq.com/>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando necesites enviar información de GlobalSuite a Rabbit MQ, por ejemplo para orquestación entre aplicaciones, alertas operativas, integración con sistemas legacy y automatización de procesos. Antes de publicarlo, valida con el equipo propietario del sistema destino el formato esperado, permisos, frecuencia y criterios de calidad.
