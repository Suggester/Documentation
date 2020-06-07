# Mark
---
### Description
Modifie le statut d'une suggestion
### Arguments Requis
` ID de suggestion` - L'ID de la suggestion dont vous souhaitez changer le statut

`statut` - Le nouveau statut que vous souhaitez appliquer

| Argument              |                Définition                    |
|-----------------------|:--------------------------------------------:|
| `default`, `none`     | Remet le statut à zéro (aucun n'est affiché) |
| `no`                  | N'aura pas lieu                              |
| `working`, `progress` | En cours                                     |
| `implemented`, `done` | Implémenté                                   |

### Utilisation
```
.mark <ID de suggestion> <statut>
```
### Aliases
`status`
### Permission Requise
Toutes les personnes ayant la permission **Gérer le serveur**, un rôle admin configuré ou un rôle staff configuré.
