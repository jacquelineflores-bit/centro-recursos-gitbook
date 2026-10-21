# Guía de instalación y configuración del MCP GlobalSuite

Esta guía explica cómo conectar tu asistente de IA con GlobalSuite® mediante el MCP GlobalSuite, tanto si usas una cuenta propia como una cuenta gestionada por tu organización, y cómo se inicia sesión con tu usuario de GlobalSuite®.

* [Antes de empezar](#GuíadeinstalaciónyconfiguracióndelMCPGlobalSuite-Antesdeempezar)
  * [Dirección del MCP de tu entorno](#GuíadeinstalaciónyconfiguracióndelMCPGlobalSuite-DireccióndelMCPdetuentorno)
  * [Datos de conexión OAuth](#GuíadeinstalaciónyconfiguracióndelMCPGlobalSuite-DatosdeconexiónOAuth)
* [Inicio de sesión con tu usuario de GlobalSuite®](#GuíadeinstalaciónyconfiguracióndelMCPGlobalSuite-IniciodesesióncontuusuariodeGlobalSuite®)
* [Configuración por asistente](#GuíadeinstalaciónyconfiguracióndelMCPGlobalSuite-Configuraciónporasistente)
  * [Claude (web, escritorio y móvil)](#GuíadeinstalaciónyconfiguracióndelMCPGlobalSuite-Claude(web,escritorioymóvil))
  * [ChatGPT](#GuíadeinstalaciónyconfiguracióndelMCPGlobalSuite-ChatGPT)
  * [Cursor](#GuíadeinstalaciónyconfiguracióndelMCPGlobalSuite-Cursor)
  * [Microsoft Copilot Studio](#GuíadeinstalaciónyconfiguracióndelMCPGlobalSuite-MicrosoftCopilotStudio)
  * [Microsoft 365 Copilot](#GuíadeinstalaciónyconfiguracióndelMCPGlobalSuite-Microsoft365Copilot)
  * [GitHub Copilot (Visual Studio Code)](#GuíadeinstalaciónyconfiguracióndelMCPGlobalSuite-GitHubCopilot(VisualStudioCode))
* [Comprueba que funciona](#GuíadeinstalaciónyconfiguracióndelMCPGlobalSuite-Compruebaquefunciona)
* [Desconectar el MCP](#GuíadeinstalaciónyconfiguracióndelMCPGlobalSuite-DesconectarelMCP)
* [Solución de problemas](#GuíadeinstalaciónyconfiguracióndelMCPGlobalSuite-Solucióndeproblemas)

## Antes de empezar

Para conectar el MCP GlobalSuite necesitas:

* Un entorno de **GlobalSuite® Cloud** y un usuario activo con acceso a la información que quieres consultar.
* Un asistente de IA compatible, con un plan que permita añadir conectores o servidores MCP personalizados.
* La **dirección del MCP de tu entorno**.

### Dirección del MCP de tu entorno

Cada entorno de GlobalSuite® tiene su propia dirección de MCP, formada por el dominio con el que accedes a GlobalSuite® en el navegador seguido de `/mcp/mcp`:

{% hint style="info" %}
```
https://<dominio-de-tu-entorno>/mcp/mcp
```
{% endhint %}

Por ejemplo, en el entorno de demostración de GlobalSuite® la dirección es `https://demo.globalsuite.es/mcp/mcp`. Si tienes dudas sobre la dirección de tu entorno, consulta con el Soporte de GlobalSuite®.

**PENDIENTE DE CONFIRMAR CON INGENIERÍA: QUE LA RUTA /mcp/mcp ES LA MISMA EN TODOS LOS ENTORNOS CLOUD.**

### Datos de conexión OAuth

La mayoría de asistentes descubren estos datos automáticamente. Algunos, como Copilot Studio, te los piden al configurar el conector:

|  |  |
| --- | --- |
| **Dato** | **Valor** |
| **URL de autorización** | `https://<dominio-de-tu-entorno>/api/oauth/authorize` |
| **URL de token y de renovación** | `https://<dominio-de-tu-entorno>/api/oauth/token` |
| **URL de revocación** | `https://<dominio-de-tu-entorno>/api/oauth/revoke` |
| **Ámbitos (scopes)** | `mcp:read` y `offline_access`  **PENDIENTE: ÁMBITO NECESARIO PARA LAS ACCIONES DE ESCRITURA.** |
| **Método de verificación** | PKCE con S256 (obligatorio). |
| **Identificador de cliente** | ChatGPT: `chatgpt` · Cursor: `cursor` · Claude: no hace falta indicarlo.  **PENDIENTE: IDENTIFICADORES DE CLIENTE DE MICROSOFT COPILOT.** |

## Inicio de sesión con tu usuario de GlobalSuite®

La conexión se autoriza con el protocolo estándar OAuth. La primera vez que conectas el MCP, tu asistente abre la pantalla de inicio de sesión de GlobalSuite® —la misma que usas en la web— y entras con tu método habitual:

|  |  |
| --- | --- |
| **Tipo de usuario** | **Cómo inicias sesión** |
| **Usuario y contraseña** | Con tu usuario y contraseña de GlobalSuite®. |
| **Active Directory o LDAP** | Con tu usuario y contraseña del directorio corporativo, igual que en la web. |
| **Single Sign-On (SAML)** | A través del proveedor de identidad de tu organización. |
| **Doble factor (2FA)** | Si lo tienes activado, se te pide igual que en la web: código de tu aplicación de autenticación o código por correo electrónico. |

Al terminar vuelves automáticamente a tu asistente, sin pantallas adicionales. A partir de ese momento el asistente consulta GlobalSuite® con tu usuario, en tu empresa y tu sistema de gestión, y con tus mismos permisos.

* El acceso dura **60 minutos** y se renueva solo mientras uses el asistente.
* Si el conector pasa **más de 7 días sin usarse**, te pedirá iniciar sesión de nuevo.
* No necesitas tener GlobalSuite® abierto en el navegador para usar el MCP.

**PENDIENTE DE CONFIRMAR: CON QUÉ EMPRESA Y SISTEMA DE GESTIÓN ENTRA EL MCP CUANDO EL USUARIO TIENE ACCESO A VARIAS, Y CÓMO SE CAMBIA.**

## Configuración por asistente

Elige tu asistente. En las cuentas corporativas, normalmente un administrador debe habilitar o añadir primero el conector para toda la organización.

**PENDIENTE: CAPTURAS DE CONFIGURACIÓN EN CLAUDE Y CHATGPT (SESIÓN DE CAPTURAS REALES CON INICIO DE SESIÓN DEL PO).**

### Claude (web, escritorio y móvil)

**Cuenta propia (Pro o Max)**

1. Abre Claude y ve a **Configuración → Conectores** (Settings → Connectors).
2. Pulsa **Añadir** (o el icono +) y selecciona **Añadir conector personalizado** (Add custom connector).
3. Escribe un nombre (por ejemplo, «GlobalSuite») y pega la dirección del MCP de tu entorno. No hace falta rellenar la configuración avanzada.
4. Pulsa **Añadir** y después **Conectar**. Se abrirá la pantalla de GlobalSuite®: inicia sesión.
5. En cada conversación, activa el conector desde el botón **+** → **Conectores**.

**Cuenta de organización (Team o Enterprise)**

1. Un propietario de la organización añade el conector personalizado con la dirección del MCP desde la configuración de conectores de la organización.
2. Cada usuario va a **Configuración → Conectores**, busca GlobalSuite y pulsa **Conectar** para iniciar sesión con su propio usuario de GlobalSuite®.

Más información en la [ayuda de Claude](https://support.claude.com/) (conectores personalizados mediante MCP remoto).

### ChatGPT

ChatGPT necesita el **modo desarrollador** para añadir servidores MCP personalizados y un plan de pago (Plus, Pro, Business, Enterprise o Edu).

**Cuenta propia (Plus o Pro)**

1. Ve a **Configuración → Seguridad e inicio de sesión** y activa el **modo desarrollador** (Developer mode). Solo hay que hacerlo una vez.
2. En **Configuración → Complementos**, crea un conector nuevo y rellena:

   * **Nombre:** por ejemplo, «GlobalSuite».
   * **URL del servidor MCP:** la dirección del MCP de tu entorno.
   * **Autenticación:** OAuth. En la configuración avanzada de OAuth, escribe `chatgpt` como **ID de cliente** y deja el resto por defecto.
3. Pulsa **Crear** y después **Conectar** para iniciar sesión en GlobalSuite®.

**Cuenta de organización (Business, Enterprise o Edu)**

No podrás añadir el conector por tu cuenta: el administrador del espacio de trabajo debe habilitar el modo desarrollador y publicar el conector de GlobalSuite para los miembros. Después, cada usuario lo conecta con su propio usuario de GlobalSuite®. Más información en la [ayuda de OpenAI](https://help.openai.com/).

### Cursor

1. Abre el archivo de configuración `mcp.json`: global en `~/.cursor/mcp.json` (en Windows, `%USERPROFILE%\.cursor\mcp.json`) o por proyecto en `.cursor/mcp.json`. También puedes hacerlo desde **Cursor Settings → MCP → New MCP Server**.
2. Añade este bloque, sustituyendo la dirección por la de tu entorno, y guarda:

{% hint style="info" %}
```
{
"mcpServers": {
"globalsuite": {
"url": "https://<dominio-de-tu-entorno>/mcp/mcp",
"auth": {
"CLIENT\_ID": "cursor",
"scopes": ["mcp:read", "offline\_access"]
}
}
}
}
```
{% endhint %}

3. Reinicia Cursor. La primera vez se abrirá el navegador para que inicies sesión en GlobalSuite®. Cuando el servidor aparezca con un punto verde, ya está conectado.

### Microsoft Copilot Studio

1. Abre tu agente en Copilot Studio y ve a **Herramientas → Agregar una herramienta → Nueva herramienta → Model Context Protocol**.
2. Escribe un nombre y una descripción, y pega la dirección del MCP de tu entorno.
3. En autenticación, elige **OAuth 2.0 → Manual** y completa el identificador de cliente, la URL de autorización, la URL de token, la URL de actualización (la misma que la de token) y los ámbitos.
4. Copia la URL de retorno (callback) que muestra Copilot Studio y facilítasela al Soporte de GlobalSuite® para que la autorice.
5. Guarda la herramienta y publica el agente. La primera vez que se use, pedirá iniciar sesión en GlobalSuite®.

**PENDIENTE: IDENTIFICADOR DE CLIENTE (Y SECRETO SI APLICA) DE COPILOT STUDIO Y ALTA DE SU URL DE RETORNO; VALIDAR LOS PASOS CON UNA CUENTA REAL.**

### Microsoft 365 Copilot

Para usar GlobalSuite® desde Microsoft 365 Copilot, crea el agente en Copilot Studio como se indica arriba y publícalo en el canal de **Microsoft Teams y Microsoft 365 Copilot**. Los usuarios encontrarán el agente en Copilot y, la primera vez, iniciarán sesión con su usuario de GlobalSuite®.

**PENDIENTE: VALIDAR EL PROCEDIMIENTO DE PUBLICACIÓN EN MICROSOFT 365 COPILOT CON UNA CUENTA REAL.**

### GitHub Copilot (Visual Studio Code)

Añade el servidor en el archivo `.vscode/mcp.json` de tu proyecto o en la configuración de usuario de VS Code:

{% hint style="info" %}
```
{
"servers": {
"globalsuite": {
"type": "http",
"url": "https://<dominio-de-tu-entorno>/mcp/mcp"
}
}
}
```
{% endhint %}

Al iniciar el servidor, VS Code te pedirá iniciar sesión en GlobalSuite®. Si te solicita un identificador de cliente, usa el indicado en la tabla de datos de conexión.

**PENDIENTE: IDENTIFICADOR DE CLIENTE DE GITHUB COPILOT; VALIDAR LOS PASOS CON UNA CUENTA REAL.**

## Comprueba que funciona

Con el conector activo, escribe en tu asistente:

{% hint style="info" %}
```
¿Qué análisis de riesgos tengo en GlobalSuite?
```
{% endhint %}

Si todo está bien, el asistente te mostrará la lista de tus análisis de riesgos. Encontrarás muchos más ejemplos en [Casos de uso y ejemplos de prompts](casos-de-uso-y-ejemplos-de-prompts-del-mcp-globalsuite.md).

## Desconectar el MCP

|  |  |
| --- | --- |
| **Asistente** | **Cómo desconectarlo** |
| **Claude** | Configuración → Conectores → GlobalSuite → Desconectar. Para dejar de usarlo solo en una conversación, desactívalo en el botón + → Conectores. |
| **ChatGPT** | Configuración → Complementos → GlobalSuite → Desconectar o eliminar. |
| **Cursor y GitHub Copilot** | Elimina el bloque «globalsuite» del archivo de configuración y reinicia la aplicación. |
| **Copilot Studio** | El administrador elimina la herramienta del agente. |

En las cuentas corporativas, los administradores de Claude y ChatGPT pueden además limitar qué conectores están permitidos en la organización.

**PENDIENTE DE CONFIRMAR: SI SE PUEDE REVOCAR EL ACCESO DESDE GLOBALSUITE O BLOQUEAR EL MCP PARA UNA EMPRESA ENTERA.**

## Solución de problemas

|  |  |
| --- | --- |
| **Problema** | **Qué hacer** |
| **No aparece la opción de añadir conectores** | Comprueba que tu plan lo permite. En ChatGPT, activa el modo desarrollador. En cuentas corporativas, pide al administrador que añada o habilite el conector. |
| **Falla la conexión** | Revisa que la dirección es exactamente la de tu entorno, incluida la ruta final `/mcp/mcp`. |
| **Error al iniciar sesión** | Comprueba que tu usuario está activo y que puedes entrar en GlobalSuite® por la web con el mismo método. Si usas doble factor, ten a mano el código. |
| **Conecta, pero no responde con datos** | Desconecta y vuelve a conectar el MCP, inicia sesión y abre una conversación nueva con el conector activado. |
| **No encuentra un análisis, un requisito o un documento** | Escribe su nombre tal como aparece en GlobalSuite® y comprueba que tu usuario tiene acceso. Los documentos se buscan por el nombre del archivo, no por su contenido. |
| **La respuesta parece incompleta** | Con mucho volumen de datos, pide al asistente que revise todas las páginas de resultados, acota la pregunta (por análisis, categoría o elemento) o usa el modo de investigación de tu asistente. |
| **Aviso de demasiadas peticiones** | Has superado el límite de uso por minuto. Espera un momento y vuelve a intentarlo. |
| **Pide iniciar sesión de nuevo** | Es normal si el conector llevaba más de 7 días sin usarse. Vuelve a iniciar sesión. |

**Ten en cuenta:** las pantallas de configuración pertenecen a cada proveedor de IA y pueden cambiar sin previo aviso. Si algún paso no coincide, consulta la ayuda oficial de tu asistente o contacta con el Soporte de GlobalSuite®.
