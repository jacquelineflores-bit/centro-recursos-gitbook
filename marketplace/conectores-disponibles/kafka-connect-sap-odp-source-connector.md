# Kafka Connect SAP ODP Source Connector

|  |  |
| --- | --- |
|  | **Conector para incorporar en GlobalSuite datos de procesos SAP, maestros y objetos de negocio procedentes de SAP ODP.**  **Etiquetas:** Bases de datos | Source | SAP |

|  |  |
| --- | --- |
| Herramienta o sistema | SAP ODP |
| Fabricante de la herramienta | SAP SE |
| Proveedor del conector | Rahul Bhattacharya |
| Nombre del conector | Kafka Connect SAP ODP Source Connector |
| Tipo de conector | Source |
| Etiquetas | Bases de datos | Source | SAP |
| Información que maneja | datos de procesos SAP, maestros y objetos de negocio |

## Detalles

El conector Kafka Connect SAP ODP Source Connector permite incorporar a GlobalSuite información procedente de SAP ODP relacionada con datos de procesos SAP, maestros y objetos de negocio.

Está orientado a mantener actualizados procesos de gestión, evidencias e indicadores sin depender de cargas manuales, especialmente en escenarios de sincronización de datos maestros, eventos de procesos, conciliación operativa y trazabilidad de controles sobre procesos SAP.

## Características

* Incorporación configurable de datos de procesos SAP, maestros y objetos de negocio desde SAP ODP hacia los procesos de GlobalSuite.
* Integración de objetos de negocio, datos maestros o eventos de procesos SAP con procesos GRC.
* Mapeo de campos funcionales para alinear sociedad, centro, proveedor, activo, control o documento.
* Soporte a conciliaciones, seguimiento de aprobaciones y evidencias sobre procesos críticos.
* Configuración por entidad, objeto o servicio para adaptar el alcance al proceso de negocio.

## Beneficios clave

* Alinea procesos GRC con datos maestros y eventos de negocio ya existentes en SAP.
* Reduce duplicidades entre equipos funcionales, riesgos, cumplimiento y áreas operativas.
* Facilita controles sobre procesos críticos como compras, proveedores, activos, finanzas o producción.
* Mejora la trazabilidad entre transacciones, aprobaciones, evidencias y responsables.
* Permite acelerar conciliaciones y análisis sin depender de exportaciones manuales recurrentes.

## Instalación

|  |
| --- |
| **Nota de configuración:** Antes de activar la integración, valida credenciales, permisos, alcance funcional y una prueba de datos con el área responsable. |

1. Accede al Marketplace de GlobalSuite® y selecciona Kafka Connect SAP ODP Source Connector.
2. Configura la conexión con SAP ODP: URL o endpoint, credenciales, permisos y entorno.
3. Define el alcance funcional de la sincronización: datos de procesos SAP, maestros y objetos de negocio, filtros y frecuencia.
4. Mapea los campos recibidos con las entidades, evidencias o procesos correspondientes de GlobalSuite.
5. Ejecuta una prueba, revisa los registros sincronizados y activa la integración.

## Más información

<https://init-software.de>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando necesites incorporar información de SAP ODP en procesos de GlobalSuite, por ejemplo para sincronización de datos maestros, eventos de procesos, conciliación operativa y trazabilidad de controles sobre procesos SAP. Antes de publicarlo, acuerda con el área propietaria qué datos son necesarios, con qué frecuencia deben actualizarse y quién revisará los resultados.
