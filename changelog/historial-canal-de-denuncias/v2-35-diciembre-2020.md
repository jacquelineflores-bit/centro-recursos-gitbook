# v2.35 (Diciembre 2020)

Funcionalidades y mejoras incluidas:

- Mejoras de **seguridad** en la gestión de usuarios y contraseñas. Nueva política de contraseñas:

* Las contraseñas tendrán una caducidad máxima de 180 días (6 meses).
* Cuando se solicite cambio de contraseña se deberán cumplir los siguientes requisitos:

  * Debe ser distinta a la actual
  * Debe tener al menos 13 caracteres y contener minúsculas, mayúsculas, números y símbolos ($, &, @, ., #)
  * Tampoco debe coincidir con las cinco últimas contraseñas utilizadas

- **Bloqueo** de usuarios: Ante un número de intentos fallidos consecutivos en el proceso de autenticarse, el usuario quedará bloqueado temporalmente.

- Configuración de **Datos Personales del Comunicador** a la hora de crear denuncias.

* Permite definir qué campos y qué datos personales puede completar, y cuáles debe completar por ser obligatorios, el comunicador que registra una denuncia (cuando esta no es anónima).

- Personalización de textos de Condiciones de Uso:

* Además de la posibilidad de subir un documento personalizado de las Condiciones de Uso, es posible configurar el mensaje que aparece en la petición de aceptación.

- Configuración del **DashBoard** inicial:

* Personalización de las gráficas que se muestran en la vista inicial, pudiendo activarlas/desactivarlas, y cambiar el orden en el que se muestran.
* Actualmente está disponible para empresas Administradoras. En próximas actualizaciones se liberará para los canales finales, con nuevas estadísticas.

- Mejoras internas y resolución de errores.
