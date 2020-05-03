# Config

### Descripción
Este comando es usado para configurar varios ajuestes sin nedesidad de realizar una configuración completa.
### Argumentos Opcionales
`list` - Este argumento es usado para mostrar la configuración actual del servidor.

`element` - Si es usado sin ningún otro argumento, mostrará la configuración acutal para ese elemento.


*Para configuración*

<!-- tabs:start -->
#### **Roles de Administrador**
## Elemento Configurable

### `admin`
## Función

**Cualquier usuario con cualquiera de esos roles hereda permisos de staff, pero también tendrá permiso para configurar ajustes del servidor.**

## Entradas Válidas

**Nombre del rol, ID o @mención**

## Uso

`config admin [add/remove/list] [rol]`

#### **Roles de Staff**

## Elemento Configurable

### `staff`
## Función

**Cualquier usuario con cualquera de esos roles tendrá permiso para aceptar y denegar sugerencia, y también para interactuar con estas de otras maneras.**

## Entradas Válidas

**Nombre del rol, ID o @mención**

## Uso

`config staff [add/remove/list] [rol]`

#### **Roles con Permiso para Sugerir**

## Elemento Configurable

### `allowed`
## Función

**Cualquier usuario con cualquera de esos roles (o un rol de staff/administrador) puede realizar sugerencias. Si no hay roles permitidos configurados todos los miembros pueden realizar sugerencias.**

?> ¡Esto es útil para bloquear las sugerencias a solo algunos miembros de tu servidor!

## Entradas Válidas

**Nombre del rol, ID or @mención**

## Uso

`config allowed [add/remove/list] [rol]`

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

**El canal donde se enviarán las sugerencias inmediatamente después de ser realizadas para que sean revisadas por el staff. (Únicamente si el modo está configurado en *revisión*)**

## Entradas Válidas

**Nombre del canal, ID o #mención**

## Uso

`config review [canal]`

#### **Canal de Sugerencias Aprobadas**

## Elemento Configurable

### `suggestions`
## Función

**El canal donde las sugerencias aprobadas son enviadas. (Si el modo está configurado como *autoaprobar* entonces todas las sugerencias son enviadas automáticamente a este canal)**

## Entradas Válidas

**Nombre del canal, ID o #mención**

## Uso

`config suggestions [canal]`

#### **Canal de Sugerencias Denegadas**

## Elemento Configurable

### `denied`
## Función

**El canal donde las sugerencias denegadas/borradas son enviadas.**

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

**El canal donde se enviarán todas las sugerencias que hayan sido marcadas como __implementadas__ usando el comando  [mark](es/staff/mark.md).**

**Usar** `none` **como canal eliminará el actual canal de archivo de sugerencias implementadas si hay alguno configurado.**

## Entradas Válidas

**Nombre del canal, ID, #mención o** `none`

## uso

`config implemented [canal]`

#### **Canal de Comandos de Sugerencias**

## Ekemento Configurable

### `commands`
## Función

**El canal donde el comando** `suggest` **puede ser usado. (Si esto no es configurado el comando `suggest` podrá ser usado en cualquier canal)**

?> ¡Esto es útil para mantener los comandos del bot lejos de los canales de chat!

## Entradas Válidas

**Nombre del canal, ID, #mención o** `none`

## Uso

`config commands [canal]`

#### **Emojis de Reacción**

## Elemento Configurable

### `emojis`
## Función

**Los emojis que deberían añadirse como reacción a las sugerencias aprobadas. Los predeterminados son 👍, 🤷, y 👎 para voto positivo, neutral y voto negativo respectivamente.**

**Seleccionar** `disable` **para un emote lo desactiva - lo que significa que no será añadido a futuras sugerencias aprobadas.**

**Los parámetros** `toggle`/`enable`/`disable` **editarán los ajustes que controlan las reacciones del feed de sugerencias - esto está *activado* de forma predeterminada.**

## Entradas válidas

**Unicode o emoji personalizado del servidor.**

## Uso

`config emojis [upvote/shrug/downvote/toggle/enable/disable] [emoji/disable]`

#### **Ajustes de Notificaciones**

## Elemento Configurable

### `notify`
## Función

**El elemento** `notify` **especifica si los miembros del servidor deberían ser notificados a través de MD cuando se realicen acciones en sus sugerencias o no.**

**Este ajuste está *activado* de forma predeterminada.**

## Entradas Válidas

`enable`, `disable`, **o** `toggle`

## Uso

`config notify [enable/disable/toggle]`

#### **Modo de Sugerencias**

## Elemento de Configuración

### `mode`
## Función

**El elemento** `mode` **configura el modo en el que se gestionan las sugerencias.**

**Ajustándolo a** `review` *(revisión)* **hará que todas las sugerencias pasen por un servicio de revisión antes de aparecer en el canal de sugerencias.**

**Ajustándolo a** `autoapprove` *(autoaprobar)* **hará que todas las sugerencias aparezcan directamente en el canal de sugerencias.**

## Entradas Válidas

`review` **o** `autoapprove`

## Uso

`config mode [review/autoapprove]`

#### **Auto-Limpieza del Canal de Sugerencias**

## Elemento Configurable

### `cleancommands`
## Función

**Este elemento especifica si los comandos de sugerencias y las respuestas del bot han de borrarse o no después de unos segundos.**

**Este ajuste está *desactivado* de forma predeterminada.**

?> ¡Este ajuste es útil para mantener limpio el canal de sugerencias!

## Entradas Válidas

`enable`, `disable` **o** `toggle`

## Uso

`config cleancommands [enable/disable/toggle]`

#### **Prefijo**

## Elemento Configurable

### `prefix`
## Función

**El prefijo por el que comienzan todos los comandos, por ejemplo: en** `.command` **el prefijo es** `.`

## Entradas Válidas

**Cualquier secuencia sin espacios**

## Uso

`config prefix [prefijo]`

<!-- tabs:end -->


### Uso
```
.config (elemento) (parámetros adicionales)
```
### Alias
`serverconfig`, `cfg`, `configure`
### Permisos Requeridos
Cualquier usuario con el permiso de **Administrar Servidor** o un rol de administrador configurado.
