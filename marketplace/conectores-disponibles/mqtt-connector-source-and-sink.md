# MQTT Connector (Source and Sink)

|  |  |
| --- | --- |
|  | **Conector para intercambiar telemetría industrial, eventos IoT y señales de dispositivos entre GlobalSuite y MQTT en los escenarios habilitados.**  **Etiquetas:** Mensajería | Integración | Source y Sink | IoT |

|  |  |
| --- | --- |
| Herramienta o sistema | MQTT |
| Fabricante de la herramienta | Estándar / protocolo abierto |
| Proveedor del conector | Confluent, Inc |
| Nombre del conector | MQTT Connector (Source and Sink) |
| Tipo de conector | Source y Sink |
| Etiquetas | Mensajería | Integración | Source y Sink | IoT |
| Información que maneja | telemetría industrial, eventos IoT y señales de dispositivos |

## Detalles

El conector MQTT Connector (Source and Sink) permite intercambiar información entre GlobalSuite y MQTT, combinando flujos de entrada y salida según el caso de uso.

Facilita mantener alineados telemetría industrial, eventos IoT y señales de dispositivos en ambos entornos, con especial aplicación en escenarios de seguimiento de activos industriales, alertas de operación, trazabilidad de dispositivos y continuidad operativa.

## Características

* Intercambio bidireccional de telemetría industrial, eventos IoT y señales de dispositivos entre GlobalSuite y MQTT, según el flujo habilitado.
* Captura o entrega de telemetría, señales industriales o eventos de dispositivos para casos operativos.
* Mapeo de dispositivos, activos, plantas o líneas de producción con entidades gestionadas en GlobalSuite.
* Soporte a alertas sobre disponibilidad, seguridad, continuidad o comportamiento anómalo.
* Configuración por origen, dispositivo o variable para limitar el alcance a información relevante.

## Beneficios clave

* Permite llevar datos de planta, dispositivos o activos conectados a procesos de riesgo, continuidad o mantenimiento.
* Acelera la detección de anomalías operativas que puedan afectar a servicios críticos.
* Facilita relacionar telemetría con activos, controles, ubicaciones o responsables.
* Reduce la distancia entre equipos OT, IT, seguridad y cumplimiento.
* Apoya casos de continuidad operativa, seguridad industrial y seguimiento de activos en tiempo real.

## Instalación

|  |
| --- |
| **Nota de configuración:** Antes de activar la integración, valida credenciales, permisos, alcance funcional y una prueba de datos con el área responsable. |

1. Accede al Marketplace de GlobalSuite® y selecciona MQTT Connector (Source and Sink).
2. Configura la conexión con MQTT: URL o endpoint, credenciales, permisos y entorno.
3. Define la dirección de cada flujo y el alcance funcional: telemetría industrial, eventos IoT y señales de dispositivos, filtros y frecuencia.
4. Configura el mapeo de campos para la entrada, la salida o ambos escenarios.
5. Ejecuta pruebas separadas por dirección, valida resultados y activa la integración.

## Más información

<https://mqtt.org/>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando MQTT y GlobalSuite deban intercambiar información en ambos sentidos, por ejemplo para seguimiento de activos industriales, alertas de operación, trazabilidad de dispositivos y continuidad operativa. Conviene separar claramente qué datos entran, qué datos salen y quién es responsable de resolver discrepancias.
