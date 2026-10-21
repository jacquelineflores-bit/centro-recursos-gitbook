# SFTP Connector (Source and Sink)

|  |  |
| --- | --- |
|  | **Conector para intercambiar ficheros, evidencias, documentos y objetos de almacenamiento entre GlobalSuite y SFTP en los escenarios habilitados.**  **Etiquetas:** Almacenamiento | Cloud | Source y Sink |

|  |  |
| --- | --- |
| Herramienta o sistema | SFTP |
| Fabricante de la herramienta | Estándar / protocolo abierto |
| Proveedor del conector | Confluent, Inc |
| Nombre del conector | SFTP Connector (Source and Sink) |
| Tipo de conector | Source y Sink |
| Etiquetas | Almacenamiento | Cloud | Source y Sink |
| Información que maneja | ficheros, evidencias, documentos y objetos de almacenamiento |

## Detalles

El conector SFTP Connector (Source and Sink) permite intercambiar información entre GlobalSuite y SFTP, combinando flujos de entrada y salida según el caso de uso.

Facilita mantener alineados ficheros, evidencias, documentos y objetos de almacenamiento en ambos entornos, con especial aplicación en escenarios de retención de evidencias, intercambio de ficheros con terceros, archivo documental y explotación analítica posterior.

## Características

* Intercambio bidireccional de ficheros, evidencias, documentos y objetos de almacenamiento entre GlobalSuite y SFTP, según el flujo habilitado.
* Gestión de rutas, carpetas, contenedores o prefijos para ordenar la información por proceso o periodo.
* Compatibilidad con usos de archivo, intercambio de evidencias, respaldo documental o explotación posterior.
* Definición de formatos, filtros y criterios de selección para limitar el volumen importado o exportado.
* Trazabilidad sobre qué ficheros se han procesado, cuándo y con qué resultado.

## Beneficios clave

* Facilita conservar evidencias y documentación en repositorios corporativos ya gobernados.
* Reduce cargas manuales de ficheros y mejora la organización por proceso, tercero, control o periodo.
* Apoya políticas de retención, auditoría y respaldo documental con menor esfuerzo operativo.
* Permite compartir información con áreas internas o terceros usando ubicaciones controladas.
* Mejora la preparación de datos para reporting, data lake o análisis posteriores.

## Instalación

|  |
| --- |
| **Nota de configuración:** Antes de activar la integración, valida credenciales, permisos, alcance funcional y una prueba de datos con el área responsable. |

1. Accede al Marketplace de GlobalSuite® y selecciona SFTP Connector (Source and Sink).
2. Configura la conexión con SFTP: URL o endpoint, credenciales, permisos y entorno.
3. Define la dirección de cada flujo y el alcance funcional: ficheros, evidencias, documentos y objetos de almacenamiento, filtros y frecuencia.
4. Configura el mapeo de campos para la entrada, la salida o ambos escenarios.
5. Ejecuta pruebas separadas por dirección, valida resultados y activa la integración.

## Más información

<https://docs.confluent.io/cloud/current/connectors/overview.html>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando SFTP y GlobalSuite deban intercambiar información en ambos sentidos, por ejemplo para retención de evidencias, intercambio de ficheros con terceros, archivo documental y explotación analítica posterior. Conviene separar claramente qué datos entran, qué datos salen y quién es responsable de resolver discrepancias.
