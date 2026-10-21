# Usuarios

##### **NOTA:** Esta opción está disponible para los usuarios Administrador Global y Administrador.

En este tipo de empresa es posible crear tres tipos de usuarios:

### **Administrador Global**

Es el rol de usuario con todos los permisos para tener posibilidad de administrar y parametrizar el entorno, además tendrá acceso a la visualización y gestión de comunicaciones. Podrá asignar denuncias a los gestores.

![](../.gitbook/assets/259817591-image2019-4-8-13-41-8.png)

### **Administrador**

Es el rol de usuario con todos los permisos para tener posibilidad de administrar y parametrizar el entorno. A diferencia del anterior rol, no tendrá acceso a la visualización de las comunicaciones, ni a la asignación de estas a los gestores.

![](../.gitbook/assets/259817591-image2019-4-8-13-42-6.png)

### Consulting

Usuario que tendrá la posibilidad de acceder a uno o varios canales de comunicación, dentro de estos, tendrá acceso a la visualización y gestión de comunicaciones. Podrá asignar comunicaciones a los gestores. Este usuario solo podrá realizar todas las acciones anteriores, en empresas Consulting (Canales de Comunicación) a las que un Administrador Global o Administrador le haya dado acceso.

![](../.gitbook/assets/259817591-image2019-2-25-12-6-49.png)

Como ejemplo de creación de un usuario Consulting, se deben poner los siguientes datos para darle acceso a uno o varios canales..

![](../.gitbook/assets/259817591-image2019-4-8-13-43-35.png)

### Gestor Consulting

Usuario que tendrá la posibilidad de acceder a uno o varios canales de comunicación en los que se le haya incluido, y dentro de estos, únicamente tendrá acceso a la visualización y gestión de las comunicaciones que se le asignen directamente (ver [Comunicaciones](../empresa-consulting/comunicaciones.md)). Este usuario solo se le podrán asignar comunicaciones en empresas Consulting (Canales de Comunicación) a las que un Administrador Global o Administrador le haya dado acceso.

![](../.gitbook/assets/259817591-image2020-7-9-11-21-53.png)

##### Restablecer Contraseña

Es posible restablecer la contraseña a un usuario, a través del botón correspondiente disponible en su ficha. Al pulsarlo, se generará una nueva contraseña temporal que se le enviará por correo (el usuario deberá cambiarla en el primer acceso.

![](../.gitbook/assets/259817591-image2020-7-24-9-35-24.png)

Esto únicamente es posible para los usuarios que acceden a través de autenticación local (con usuario y contraseña propios de la aplicación).

Las contraseñas introducidas deben cumplir la siguiente política de contraseñas seguras para usuarios locales:

* Caducidad: las contraseñas tendrán una caducidad máxima de 180 días (6 meses).
* Complejidad: Tener al menos 13 caracteres y contener minúsculas, mayúsculas, números y símbolos ($, &amp;, @, ., #).
* Histórico de últimas contraseñas: Cuando se solicite cambio de contraseña la nueva deberá ser distinta a la actual y no debe coincidir con las cinco últimas contraseñas utilizadas.
* Bloqueo de usuarios: Ante un número de intentos fallidos consecutivos en el proceso de autenticarse, el usuario quedará bloqueado temporalmente.

En caso de que el usuario tenga autenticación por otro mecanismo (como ADFS), no podrá restaurarse la contraseña.

![](../.gitbook/assets/259817591-image2020-7-24-9-39-22.png)

##### Notificaciones

Aparte de las notificaciones que reciben los usuarios Gestores cuando se les asigna una comunicación, todos los tipos de usuario recibirán las notificaciones que tengan configuradas en cada entorno (ver apartado [Configuraciones](../empresa-consulting/configuraciones-consulting.md)).

En cualquier caso, cada usuario podrá desactivar de forma centralizada las notificaciones que recibe, en el apartado Mi Perfil, además de poder cambiar su contraseña:

![](../.gitbook/assets/259817591-image2019-9-24-19-14-24.png)

**Conflicto de Intereses**

Además, cuando el Conflicto de Intereses está habilitado en el apartado de [Configuraciones > Preguntas](https://help.globalsuitesolutions.com/canal-comunicaciones/configuraciones-consulting#ConfiguracionesConsulting-Preguntas), es posible configurar qué usuarios de los que tienen acceso a las denuncias (los roles Administrador Global, Gestor o Consulting a nivel organizativo superior en caso de tener múltiples canales) van a estar incluidos en el conflicto de intereses y serán visibles para el denunciante.

Para ello, accediendo al formulario de estos usuarios (salvo los de rol Administrador, que en ningún caso tienen acceso a las denuncias) se podrá habilitar o deshabilitar el que sea susceptible de tener un conflicto de intereses.

![image-20240223-084748.png](https://changelog.globalsuitesolutions.com/__attachments/412844090/image-20240223-084748.png?inst-v=5452cb2b-281a-4c57-91b5-7f7ad2b3f90f)

Esto es así para que en los casos que también existan usuarios independientes o de terceros que no estarían involucrados, estos no aparezcan para el denunciante.
