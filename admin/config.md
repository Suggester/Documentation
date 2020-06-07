# Config

### Descripción
Configura opciones individuales para el bot.
### Argumentos Opcionales
`list` - Muestra la configuración actual del servidor.

`elemento` - El ajuste a cambiar

`...entrada` - El valor del ajuste que te gustaría cambiar. Dejarlo en blanco mostrará el ajuste actual.


*Para configuración*

<!-- tabs:start -->
#### **Roles de Administrador**
## Elemento Configurable

### `admin`
## Función

**El rol de administrador hereda automáticamente todos los permisos del staff y la habilidad de configurar los ajustes del servidor.**

## Entradas Válidas

**Nombre del rol, ID o @mención**

## Uso

`config admin [<add|remove|list> <rol>]`

#### **Roles de Staff**

## Elemento Configurable

### `staff`
## Función

**Los roles de staff otorgan el permiso de interactuar con las sugerencias (aprobar, denegar, etc.).**

## Entradas Válidas

**Nombre del rol, ID o @mención**

## Uso

`config staff [<add|remove|list> <rol>]`

#### **Roles con Permiso para Sugerir**

## Elemento Configurable

### `allowed`
## Función

**Cualquier usuario con cualquera de esos roles puede realizar sugerencias. Si se deja en blanco, todos los miembros podrán realizar sugerencias**

?> ¡Esto es útil para bloquear las sugerencias a miembros específicos de tu servidor!

## Entradas Válidas

**Nombre del rol, ID or @mención**

## Uso

`config allowed [<add|remove|list> <rol>]`

#### **Rol de Sugerencias Aprobadas**

## Elemento Configurable

### `approvedrole`
## Función

**Cuando la sugerencia de algún miembro es aprobada recibirá automáticamente este rol.**

**Usar** `none` **como valor eliminará el rol de sugerencias aprobadas si está configurado.**

## Entradas Válidas

**Nombre del rol, ID,  @mención** o `none`

## Uso

`config approvedrole [rol]`

#### **Canal de Revisión**

## Elemento Configurable

### `review`
## Función

**El canal donde se enviarán las sugerencias para que sean revisadas por el staff. (Únicamente si el modo está configurado en *revisión*)**

## Entradas Válidas

**Nombre del canal, ID o #mención**

## Uso

`config review [canal]`

#### **Canal de Sugerencias Aprobadas**

## Elemento Configurable

### `suggestions`
## Función

**El canal donde las sugerencias aprobadas son enviadas. (Si el modo está configurado como *autoaprobar*  todas las sugerencias serán enviadas automáticamente a este canal)**

## Entradas Válidas

**Nombre del canal, ID o #mención**

## Uso

`config suggestions [canal]`

#### **Canal de Sugerencias Denegadas**

## Elemento Configurable

### `denied`
## Función

**El canal donde son enviadas las sugerencias que son denegadas o borradas.**

**Usar** `none` **como canal eliminará el canal de sugerencias denegadas si está configurado.**

## Entradas Válidas

**Nombre del canal, ID, #mención o** `none`

## Uso

`config denied [`canal`]`

#### **Canal de Registros**

## Elemento Configurable

### `logs`
## Función

**El canal donde se registrarán todas las acciones que se tomen en las sugerencias.**

**Usar** `none` **como canal eliminará el canal de registros si hay alguno configurado.**

## Entradas válidas

**Nombre del canal, ID, #mención o** `none`

## Uso

`config logs [canal]`

#### **Canal de Archivo de Sugerencias Implementadas**

## Elemento Configurable

### `implemented`
## Función

**El canal donde se enviarán todas las sugerencias que hayan sido marcadas como __implementadas__.**

**Usar** `none` **como canal eliminará el actual canal de archivo de sugerencias implementadas si hay alguno configurado.**

## Entradas Válidas

**Nombre del canal, ID, #mención o** `none`

## uso

`config implemented [canal]`

#### **Canal de Comandos de Sugerencias**

## Ekemento Configurable

### `commands`
## Función

**El canal donde el comando** `suggest` **puede ser usado. (Si esto no es configurado el comando** `suggest` **podrá ser usado en cualquier canal)**

?> ¡Esto es útil para mantener los comandos del bot lejos de los canales de chat!

**Usar** `none` **eliminará el canal si está configurado.**

## Entradas Válidas

**Nombre del canal, ID, #mención o** `none`

## Uso

`config commands [canal]`

#### **Emojis de Reacción**

## Elemento Configurable

### `emojis`
## Función

**Las reacciones que se añadirán a las sugerencias aprobadas. Por defecto serán usados 👍, 🤷, y 👎**

**Seleccionar** `disable` **lo desactivará, lo que significa que no será añadido a futuras sugerencias aprobadas.**

## Entradas válidas

**Unicode o emoji personalizado del servidor.**

## Uso

`config emojis [<upvote|shrug|downvote|toggle|enable|disable>] [emoji|disable]`

#### **Ajustes de Notificaciones**

## Elemento Configurable

### `notify`
## Función

**El elemento** `notify` **especifica si los miembros del servidor serán notificados a través de MD cuando se realicen acciones en sus sugerencias o no.**

**Este ajuste está *activado* de forma predeterminada.**

## Entradas Válidas

`enable`, `disable` **o** `toggle`

## Uso

`config notify [enable|disable|toggle]`

#### **Modo de Sugerencias**

## Elemento de Configuración

### `mode`
## Función

**El elemento** `mode` **configura el modo en el que se gestionan las sugerencias.**

**Ajustándolo a** `review` *(revisión)* **enviará todas las sugerencias al canal de revisión antes de aparecer en el canal de sugerencias.**

**Ajustándolo a** `autoapprove` *(autoaprobar)* *enviará todas las sugerencias al canal de sugerencias.**

## Entradas Válidas

`review` **o** `autoapprove`

## Uso

`config mode [review|autoapprove]`

#### **Auto-Limpieza del Canal de Sugerencias**

## Elemento Configurable

### `cleancommands`
## Función

**Esto borrará automáticamente los comandos de sugerenicas y las respuestas del bot al rato de usarse el comando.**

**Este ajuste está *desactivado* de forma predeterminada.**

?> ¡Este ajuste es útil para mantener limpio el canal de sugerencias!

## Entradas Válidas

`enable`, `disable` **o** `toggle`

## Uso

`config cleancommands [enable|disable|toggle]`

#### **Prefijo**

## Elemento Configurable

### `prefix`
## Función

**El prefijo por el que comienzan todos los comandos.**

**El prefijo predeterminado es** `.`

## Entradas Válidas

**Cualquier secuencia sin espacios**

## Uso

`config prefix [prefijo]`

<!-- tabs:end -->


### Uso
```
.config <elemento> [parámetros adicionales]
```
### Alias
`serverconfig`, `cfg`, `configure`
### Permisos Requeridos
El usuario debe tener el permiso de **Administrar Servidor** o un rol de administrador configurado.
