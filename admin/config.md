# Config

### Description
Cette commande est utilisée pour définir divers paramètres sans recommencer l'installation complète.

### Arguments Facultatifs
`list` - Cet argument est utilisé pour afficher la configuration actuelle.

`element` - Si ceci est utilisé sans autre argument, cela affichera les paramètres actuels pour l'élément spécifié.


*Pour la configuration*

<!-- tabs:start -->
#### **Rôles Admins**
## Élément de configuration

### `admin`
## Utilité

**Quiconque ayant un de ces rôles dispose des permissions staff, mais a également la possibilité de modifier la configuration du serveur.**

## Entrées Valides

**Nom d'un rôle, ID, ou @mention**

## Utilisation

`config admin [add/remove/list] [role]`

#### **Rôles Staff**

## Élément de configuration

### `staff`
## Utilité

**Quiconque ayant un de ces rôles dispose de la permission d'approuver et de refuser des suggestions, ainsi qu'intéragir avec ces dernières par d'autres moyens.**

## Entrées Valides

**Nom d'un rôle, ID, ou @mention**

## Utilisation

`config staff [add/remove/list] [role]`

#### **Rôles Autorisés à Suggérer**

## Élément de configuration

### `allowed`
## Utilité

**Quiconque ayant un de ces rôles (ou un rôle staff/admin) peut soumettre des suggestions. Si aucun rôle n'est défini, tout le monde pourra soumettre des suggestions.**

?> C'est très pratique pour limiter l'envoi de suggestions à certaines personnes!

## Entrées Valides

**Nom d'un rôle, ID, ou @mention**

## Utilisation

`config allowed [add/remove/list] [role]`

#### **Rôle de suggestion approuvée**

## Élément de configuration

### `approvedrole`
## Utilité

**Quand la suggestion d'un membre est approuvée, son auteur(e) recevra ce rôle.**

**Utiliser** `none` **comme rôle retirera l'ancien si il y en a un défini.**

## Entrées Valides

**Nom d'un rôle, ID, ou @mention**

## Utilisation

`config approvedrole [role]`

#### **Channel de Review**

## Élément de configuration

### `review`
## Utilité

**C'est le channel où seront envoyées toutes les suggestions en attente d'approbation par le staff (uniquement si le mode est défini sur *review*)**

## Entrées Valides

**Nom d'un channel, ID, ou #mention**

## Utilisation

`config review [channel]`

#### **Channel des Suggestions Approuvées**

## Élément de configuration

### `suggestions`
## Utilité

**Le channel où les suggestions approuvées sont postées (si le mode est défini sur *autoapprove*, les suggestions seront automatiquement postées dans ce channel)**

## Entrées Valides

**Nom d'un channel, ID, ou #mention**

## Utilisation

`config suggestions [channel]`

#### ** Channel des Suggestions Refusées**

## Élément de configuration

### `denied`
## Utilité

**Le channel où sont postées les suggestions refusées/supprimées.**

**Utiliser** `none` ** comme channel retirera l'ancien si il y en a un défini.**

## Entrées Valides

**Nom d'un channel, ID, #mention ou** `none`

## Utilisation

`config denied [channel]`

#### **Channel de Logs**

## Élément de configuration

### `logs`
## Utilité

**Le channel où toutes les actions prises sur des suggestions seront logguées.**

**Utiliser** `none` **comme channel retirera l'ancien si il y en a un défini.**

## Entrées Valides

**Nom d'un channel, ID, #mention ou** `none`

## Utilisation

`config logs [channel]`

#### **Channel d'Archive des Suggestions Implementées**

## Élément de configuration

### `implemented`
## Utilité

**Le channel où toutes les suggestions marquées comme __Implémentées__ via la commande [mark](fr/staff/mark.md) seront envoyées.**

**Utiliser** `none` **comme channel retirera l'ancien si il y en a un défini.**

## Entrées Valides

**Nom d'un channel, ID, #mention ou** `none`

## Utilisation

`config implemented [channel]`

#### **Channel des Commandes de Suggestion**

## Élément de configuration

### `commands`
## Utilité

**Le channel où la commande** `suggest` **peut être utilisée (si ce n'est pas défini, la commande pourra être utilisée dans n'importe quel channel)**

?> C'est très pratique pour garder les commandes de suggestion hors des channels de chat!

**Utiliser** `none` **comme channel retirera l'ancien si il y en a un défini.**

## Entrées Valides

**Nom d'un channel, ID, #mention ou** `none`

## Utilisation

`config commands [channel]`

#### **Émojis de réaction**

## Élément de configuration

### `emojis`
## Utilité

**Les émojis affichés en réactions sur les  suggestions approuvées. Par défaut, 👍, 🤷, et 👎 représentent respectivement un avis positif (pour/upvote), sans opinion (shrug) et un avis négatif (contre/downvote).**

**Selectionner** `disable` **pour un des trois émojis le désactivera, ce qui signifie qu'il ne sera pas ajouté sur les futures suggestions approuvées.**

**Les paramètres** `toggle`**,** `enable` **et** `disable` **modifieront le paramètre qui fait que les réactions sont ajoutées dans le fil de suggestions (activé par défaut).**

## Entrées Valides

**Émoji Unicode ou personalisé provenant du serveur**

## Utilisation

`config emojis [upvote/shrug/downvote/toggle/enable/disable] [emoji/disable]`

#### **Paramètres de Notifications**

## Élément de configuration

### `notify`
## Utilité

**L'élément** `notify` **précise si les membres du serveur doivent être notifiés ou non via MP lorsque des actions sont prises sur leurs suggestions.**

**C'est activé par défaut.**

## Entrées Valides

`enable`, `disable` **ou** `toggle`

## Utilisation

`config notify [enable/disable/toggle]`

#### **Mode de Suggestion**

## Élément de configuration

### `mode`
## Utilité

**L'élément** `mode` **détermine le mode de gestion des suggestions.**

**Définir ce paramètre sur** `review` **fera passer toutes les suggestions dans un processus d'approbation avant de les envoyer dans le channel des suggestions approuvées.**

**Définir ce paramètre sur** `autoapprove` **enverra automatiquement les suggestions soumises dans le fil de suggestions.**

## Entrées Valides

`review` **ou** `autoapprove`

## Utilisation

`config mode [review/autoapprove]`

#### **Nettoyage Automatique des Commandes de Suggestion**

## Élément de configuration

### `cleancommands`
## Utilité

**Cet élément détermine si les commandes de suggestions et leurs réponses doivent être suprimées après quelques secondes.**

**C'est desactivé par défaut.**

?> C'est utile pour garder vos channels propres! 

## Entrées Valides
`enable`, `disable` **ou** `toggle`

## Utilisation

`config cleancommands [enable/disable/toggle]`

#### **Préfixe**

## Élément de configuration

### `prefix`
## Utilité

**Le préfixe avec lequel toutes les commandes commencent.**

**Exemple: dans** `.commande` **le préfixe est** `.`

## Entrées Valides

**N'importe quelle chaîne de caractères sans espace**

## Utilisation

`config prefix [prefix]`

<!-- tabs:end -->


### Utilisation
```
.config (élément) (paramètres)
```
### Aliases
`serverconfig`, `cfg`, `configure`
### Permission Requise
Toutes les personnes ayant la permission **Gérer le serveur**, ou le rôle admin configuré.
