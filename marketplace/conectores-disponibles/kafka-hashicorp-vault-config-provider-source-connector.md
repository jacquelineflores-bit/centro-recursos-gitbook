# Kafka Hashicorp Vault Config Provider Source Connector

|  |  |
| --- | --- |
|  | **Secrets Provider for Hashicorp Vault**  **Etiquetas:** Integración | Proveedor de configuración / secretos |

|  |  |
| --- | --- |
| Herramienta o sistema | Kafka Hashicorp Vault Config Provider |
| Fabricante de la herramienta | Confluent, Inc |
| Proveedor del conector | Confluent, Inc |
| Nombre del conector | Kafka Hashicorp Vault Config Provider Source Connector |
| Tipo de conector | Proveedor de configuración / secretos |
| Etiquetas | Integración | Proveedor de configuración / secretos |
| Información que maneja | credenciales, parámetros seguros y referencias de configuración |

## Detalles

El conector Kafka Hashicorp Vault Config Provider Source Connector permite referenciar de forma controlada credenciales y parámetros de configuración usados por integraciones de GlobalSuite.

Está orientado a reducir la exposición de secretos y facilitar escenarios de gestión segura de credenciales, segregación de responsabilidades, rotación de claves y reducción de exposición de secretos.

## Características

* Gestión controlada de credenciales, parámetros seguros y referencias de configuración usados por integraciones y conexiones técnicas.
* Referencia segura a credenciales sin incorporarlas directamente en configuraciones visibles.
* Soporte a rotación, segregación de responsabilidades y control centralizado de accesos.
* Reducción de exposición de claves en procesos de integración y pruebas.
* Facilita auditoría técnica sobre qué secreto se usa y con qué integración.

## Beneficios clave

* Reduce el riesgo de exposición de credenciales en configuraciones o documentación operativa.
* Facilita rotación de claves y cumplimiento de políticas internas de seguridad.
* Separa responsabilidades entre quien administra secretos y quien configura integraciones.
* Mejora la auditabilidad del uso de credenciales en conexiones críticas.
* Permite escalar integraciones manteniendo un modelo de seguridad más controlado.

## Instalación

|  |
| --- |
| **Nota de configuración:** Antes de activar la integración, valida credenciales, permisos, alcance funcional y una prueba de datos con el área responsable. |

1. Accede al Marketplace de GlobalSuite® y selecciona Kafka Hashicorp Vault Config Provider Source Connector.
2. Configura la referencia al repositorio seguro utilizado para Kafka Hashicorp Vault Config Provider.
3. Define permisos, nombres de secreto, alcance y entorno de uso.
4. Asocia las referencias seguras a las integraciones que las necesiten.
5. Guarda, valida la conexión y revisa que no se almacenen credenciales en texto claro.

## Más información

<https://www.vaultproject.io/>

## Uso recomendado en GlobalSuite

Utiliza este conector cuando debas gestionar credenciales o parámetros sensibles de forma centralizada, por ejemplo para gestión segura de credenciales, segregación de responsabilidades, rotación de claves y reducción de exposición de secretos. Define políticas de acceso, rotación y revisión periódica con el equipo de seguridad.
