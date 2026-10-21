# Kafka Connect JSON Schema Converter Source Connector

|  |  |
| --- | --- |
|  | **Conector para incorporar en GlobalSuite mensajes, eventos y notificaciones de negocio procedentes de JSON Schema Converter.**  **Etiquetas:** Mensajería | Integración | Source |

|  |  |
| --- | --- |
| Herramienta o sistema | JSON Schema Converter |
| Fabricante de la herramienta | Estándar / protocolo abierto |
| Proveedor del conector | Confluent, Inc |
| Nombre del conector | Kafka Connect JSON Schema Converter Source Connector |
| Tipo de conector | Source |
| Etiquetas | Mensajería | Integración | Source |
| Información que maneja | mensajes, eventos y notificaciones de negocio |

## Detalles

El conector Kafka Connect JSON Schema Converter Source Connector permite incorporar a GlobalSuite información procedente de JSON Schema Converter relacionada con mensajes, eventos y notificaciones de negocio.

Está orientado a mantener actualizados procesos de gestión, evidencias e indicadores sin depender de cargas manuales, especialmente en escenarios de orquestación entre aplicaciones, alertas operativas, integración con sistemas legacy y automatización de procesos.

## Características

* Incorporación configurable de mensajes, eventos y notificaciones de negocio desde JSON Schema Converter hacia los procesos de GlobalSuite.
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

1. Accede al Marketplace de GlobalSuite® y selecciona Kafka Connect JSON Schema Converter Source Connector.
2. Configura la conexión con JSON Schema Converter: URL o endpoint, credenciales, permisos y entorno.
3. Define el alcance funcional de la sincronización: mensajes, eventos y notificaciones de negocio, filtros y frecuencia.
4. Mapea los campos recibidos con las entidades, evidencias o procesos correspondientes de GlobalSuite.
5. Ejecuta una prueba, revisa los registros sincronizados y activa la integración.

## Más información

<https://docs.confluent.io/platform/current/schema-registry/connect.html>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando necesites incorporar información de JSON Schema Converter en procesos de GlobalSuite, por ejemplo para orquestación entre aplicaciones, alertas operativas, integración con sistemas legacy y automatización de procesos. Antes de publicarlo, acuerda con el área propietaria qué datos son necesarios, con qué frecuencia deben actualizarse y quién revisará los resultados.
