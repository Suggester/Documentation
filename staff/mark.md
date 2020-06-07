# Mark
---
### Descripción
Este comando se usa para cambiar el estado de una sugerencia.
### Argumentos Requeridos

`suggestionID` - El ID de la sugerencia.

`estado` - El estado que quieres usar.

| Argumento              |                Significado                                    |
|-----------------------|:---------------------------------------------------------:|
| `default`, `none`     | Restaura el estado al predeterminado (no muestra ninguno) |
| `no`                  | No Sucederá                                               |
| `working`, `progress` | En Progreso                                               |
| `implemented`, `done` | Implementada                                              |


### Uso
```
.mark <suggestionID> <status>
```
### Alias
`status`
### Permisos Requeridos
El usuario debe tener el permiso de **Administrar Servidor** o un rol de staff configurado.
