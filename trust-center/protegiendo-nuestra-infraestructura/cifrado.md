# Cifrado

## En tránsito

Todos los datos de los clientes transmitidos a nuestros servidores a través de redes públicas están protegidos mediante sólidos protocolos de cifrado. Todas las conexiones a los servidores utilizan cifrado robusto en la capa de transporte (TLS 1.2 y TLS 1.3) con cifrados sólidos en todas las conexiones, incluido el acceso web y el acceso de API.

Para el cifrado de las conexiones https utilizamos certificados digitales emitidos por la entidades de confianza utilizando un cifrado con RSA de 2048 bits.

### Protocolos

|  |  |  |
| --- | --- | --- |
| **Protocolo** | **¿Soportado?** | **Suite de Cifrado** |
| TLS 1.3 | Si | TLS\_AES\_128\_GCM\_SHA256   TLS\_AES\_256\_GCM\_SHA384 |
| TLS 1.2 | Si | TLS\_ECDHE\_RSA\_WITH\_AES\_256\_GCM\_SHA384  TLS\_ECDHE\_RSA\_WITH\_AES\_128\_GCM\_SHA256 |
| TLS 1.1 | No | N/A |
| TLS 1.0 | No | N/A |
| SSL 3 | No | N/A |

Esto garantiza una conexión segura, ya que permite la autenticación de ambas partes involucradas en la conexión y cifra los datos que se transferirán.

Nuestros servicios de correo electrónico utilizados en la plataforma GlobalSuite utilizan TLS de forma predeterminada. TLS cifra y envía el correo electrónico de forma segura, lo que mitiga las interceptaciones entre los servidores de correo en los que los servicios admiten este protocolo.

## En reposo

Los sistemas de almacenamiento de información disponen de cifrado en reposo utilizando un algoritmo AES de 256 bits.

Este nivel de cifrado garantiza que los datos estén protegidos mientras están almacenados en discos, bases de datos, volúmenes o cualquier otro tipo de almacenamiento persistente.

También se disponen de servicios de gestión de claves criptográficas (ej. KMS) que se encargan de custodiar y gestionar secretos utilizados para el cifrado en reposo.
