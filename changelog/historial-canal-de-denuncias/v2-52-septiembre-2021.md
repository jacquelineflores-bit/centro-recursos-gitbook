# v2.52 (Septiembre 2021)

Funcionalidades y mejoras incluidas:

- **Doble Factor de Autenticación**: Se ha incorporado la funcionalidad de incorporar un segundo factor de autenticación en la herramienta GlobalSUITE Whistleblower Channel.

* De manera adicional al mecanismo de autenticación actual (local, Active Directory, o ADFS Single Sign-On) se puede activar un segundo factor de autenticación mediante TOTP (Time-Based One-Time Password).  
  Este mecanismo permite sincronizar algún dispositivo para introducir un código numérico que cambia cada 30 segundos, y que será solicitado en el momento que el usuario realiza login en la herramienta.
* Esta configuración se puede activar si así se requiere, bien de forma opcional, o habilitarlo de forma obligatoria, en cuyo caso a los usuarios tendrán que configurarlo en el siguiente acceso.
* Cuenta con mecanismos de seguridad para poder acceder una única vez a la herramienta (Códigos de Recuperación), así como poder desactivarse para un usuario concreto en caso de pérdida o borrado del dispositivo asociado.

*Para activar el Doble Factor de Autenticación mediante TOTP, debe realizar los siguientes pasos:*

*1. Instalar y utilizar alguna de las aplicaciones que permiten gestionar este doble factor. Algunas de ellas son:*

* *Google Authenticator (*[*Apple Store*](https://apps.apple.com/es/app/google-authenticator/id388497605)*,*[*Play Store*](https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2&hl=es&gl=US))*)*
* *Microsoft Authenticator (*[*Apple Store*](https://apps.apple.com/es/app/microsoft-authenticator/id983156458)*,*[*Play Store*](https://play.google.com/store/apps/details?id=com.azure.authenticator&hl=es&gl=US)*)*
* *FreeOTP (*[*Apple Store*](https://apps.apple.com/us/app/freeotp-authenticator/id872559395)*,*[*Play Store*](https://play.google.com/store/apps/details?id=org.fedorahosted.freeotp&hl=es&gl=US)*)*
* *Otros*

*2. Una vez la tenga instalada, mediante la aplicación debe escanear el código QR que le aparece en pantalla, o introducir la "Cadena de secreto" de forma textual.*

*3. Una vez enlazado, deberá introducir el token o código temporal que se genera en la aplicación, y pulsar el botón "Activar".*  
*IMPORTANTE: Este token cambia cada 30 segundos, por lo que una vez pasado ese tiempo, dejará de ser válido.*

*4. Por último, deberá almacenar de forma segura los códigos de recuperación. Estos códigos le servirán para autenticarse una única vez en WhistleblowerChannel en caso de pérdida del dispositivo o borrado de la aplicación.*

 - Mejoras de usabilidad en el **Timeline**: Se ha mejorado la visualización de los seguimientos del timeline de una comunicación. Además, los comentarios introducidos se muestran estructurados en caso de tener varias líneas.

- Mejoras internas y resolución de errores.

**Resumen de nuevas funcionalidades versión v2.52**

![](../.gitbook/assets/260473438-globalsuite-whistleblower-channel-changelog-v2-52.mp4)

## Vídeos

{% file src="../.gitbook/assets/260473438-globalsuite-whistleblower-channel-changelog-v2-52.mp4" %}
GlobalSuite Whistleblower Channel - Changelog v2.52.mp4
{% endfile %}
