# SAP HANA Connector (Source and Sink)

|  |  |
| --- | --- |
|  | **Conector para intercambiar datos de procesos SAP, maestros y objetos de negocio entre GlobalSuite y SAP HANA en los escenarios habilitados.**  **Etiquetas:** SaaS | APIs | Source y Sink | SAP | Mensajería |

|  |  |
| --- | --- |
| Herramienta o sistema | SAP HANA |
| Fabricante de la herramienta | SAP SE |
| Proveedor del conector | SAP SE |
| Nombre del conector | SAP HANA Connector (Source and Sink) |
| Tipo de conector | Source y Sink |
| Etiquetas | SaaS | APIs | Source y Sink | SAP | Mensajería |
| Información que maneja | datos de procesos SAP, maestros y objetos de negocio |

## Detalles

El conector SAP HANA Connector (Source and Sink) permite intercambiar información entre GlobalSuite y SAP HANA, combinando flujos de entrada y salida según el caso de uso.

Facilita mantener alineados datos de procesos SAP, maestros y objetos de negocio en ambos entornos, con especial aplicación en escenarios de sincronización de datos maestros, eventos de procesos, conciliación operativa y trazabilidad de controles sobre procesos SAP.

## Características

* Intercambio bidireccional de datos de procesos SAP, maestros y objetos de negocio entre GlobalSuite y SAP HANA, según el flujo habilitado.
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

1. Accede al Marketplace de GlobalSuite® y selecciona SAP HANA Connector (Source and Sink).
2. Configura la conexión con SAP HANA: URL o endpoint, credenciales, permisos y entorno.
3. Define la dirección de cada flujo y el alcance funcional: datos de procesos SAP, maestros y objetos de negocio, filtros y frecuencia.
4. Configura el mapeo de campos para la entrada, la salida o ambos escenarios.
5. Ejecuta pruebas separadas por dirección, valida resultados y activa la integración.

## Más información

<https://docs.confluent.io/cloud/current/connectors/overview.html>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando SAP HANA y GlobalSuite deban intercambiar información en ambos sentidos, por ejemplo para sincronización de datos maestros, eventos de procesos, conciliación operativa y trazabilidad de controles sobre procesos SAP. Conviene separar claramente qué datos entran, qué datos salen y quién es responsable de resolver discrepancias.
