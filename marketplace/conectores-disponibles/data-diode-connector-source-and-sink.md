# Data Diode Connector (Source and Sink)

|  |  |
| --- | --- |
|  | **Conector para intercambiar indicadores, hallazgos y evidencias de seguridad entre GlobalSuite y Data Diode en los escenarios habilitados.**  **Etiquetas:** Mensajería | Integración | Source y Sink | CDC | Seguridad |

|  |  |
| --- | --- |
| Herramienta o sistema | Data Diode |
| Fabricante de la herramienta | Confluent, Inc |
| Proveedor del conector | Confluent, Inc |
| Nombre del conector | Data Diode Connector (Source and Sink) |
| Tipo de conector | Source y Sink |
| Etiquetas | Mensajería | Integración | Source y Sink | CDC | Seguridad |
| Información que maneja | indicadores, hallazgos y evidencias de seguridad |

## Detalles

El conector Data Diode Connector (Source and Sink) permite intercambiar información entre GlobalSuite y Data Diode, combinando flujos de entrada y salida según el caso de uso.

Facilita mantener alineados indicadores, hallazgos y evidencias de seguridad en ambos entornos, con especial aplicación en escenarios de evaluación de terceros, priorización de vulnerabilidades, seguimiento de planes de tratamiento y reporting de postura de seguridad.

## Características

* Intercambio bidireccional de indicadores, hallazgos y evidencias de seguridad entre GlobalSuite y Data Diode, según el flujo habilitado.
* Asociación de hallazgos con proveedores, activos, riesgos o controles para facilitar su seguimiento.
* Actualización de indicadores de exposición, criticidad o cumplimiento con criterios definidos por la organización.
* Soporte a filtros por alcance, criticidad, origen o responsable para concentrarse en lo realmente accionable.
* Trazabilidad de cambios para evidenciar evolución de la postura de seguridad y justificar decisiones.

## Beneficios clave

* Permite priorizar proveedores, activos o vulnerabilidades con información objetiva y actualizada.
* Reduce el tiempo dedicado a recopilar evidencias técnicas para evaluaciones, auditorías o comités de riesgo.
* Facilita detectar cambios relevantes de postura de seguridad antes de que impacten en el negocio.
* Ayuda a justificar planes de tratamiento y responsables con datos trazables.
* Mejora la coordinación entre seguridad, riesgos, compras y áreas propietarias del servicio.

## Instalación

|  |
| --- |
| **Nota de configuración:** Antes de activar la integración, valida credenciales, permisos, alcance funcional y una prueba de datos con el área responsable. |

1. Accede al Marketplace de GlobalSuite® y selecciona Data Diode Connector (Source and Sink).
2. Configura la conexión con Data Diode: URL o endpoint, credenciales, permisos y entorno.
3. Define la dirección de cada flujo y el alcance funcional: indicadores, hallazgos y evidencias de seguridad, filtros y frecuencia.
4. Configura el mapeo de campos para la entrada, la salida o ambos escenarios.
5. Ejecuta pruebas separadas por dirección, valida resultados y activa la integración.

## Más información

<https://docs.confluent.io/cloud/current/connectors/overview.html>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando Data Diode y GlobalSuite deban intercambiar información en ambos sentidos, por ejemplo para evaluación de terceros, priorización de vulnerabilidades, seguimiento de planes de tratamiento y reporting de postura de seguridad. Conviene separar claramente qué datos entran, qué datos salen y quién es responsable de resolver discrepancias.
