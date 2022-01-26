# Création et gestion d'une commande récurrente

Cette page explique comment mettre en place une commande récurrente pour un acheteur donné, incluant : la sélection des produits qui devront être automatiquement commandés pour l'acheteur, le rythme de ces commandes automatiques. Mais aussi, comment mettre en pause ou supprimer une commande récurrente.

{% hint style="warning" %}
Rappel : dans la première version du module, seuls les gestionnaires de boutiques en ligne peuvent mettre en place des commandes récurrentes, l'acheteur n'a pas la main directement dessus pour générer la mise en place de la commande récurrente.
{% endhint %}

**Rappel des choses à faire avant de passer aux étapes décrites ici :**

* [Activez les commandes récurrentes dans les paramètres de l'entreprise](broken-reference)
* Vérifiez ou mettez en place les [méthodes de paiement et de livraison](broken-reference) pour l'entreprise​
* [Contactez vos acheteurs pour connaître leurs coordonnées et préférences (option de paiement choisie, produits à commander et rythme de commande, ](broken-reference)etc.) et leur rappeler [ce qu'ils doivent faire de leur côté (création d'un compte utilisateurs, enregistrement d'une carte de crédit le cas échéant, etc.)​](broken-reference)
* [Ajoutez vos acheteurs à votre liste d'acheteurs](broken-reference)
* Créez au moins un [rythme d'abonnement​](broken-reference)

## 6) Créer une commande récurrente <a href="#6-create-subscriptions" id="6-create-subscriptions"></a>

Allez dans le menu général "Commandes" puis cliquez sur le sous-menu vert **Abonnements**.&#x20;

![](<../../.gitbook/assets/image (68).png>)

Cliquez ensuite sur "Nouvel abonnement" :&#x20;

![](<../../.gitbook/assets/image (70).png>)

**Acheteur :** Sélectionnez un acheteur dans la liste déroulante (seuls les acheteurs présents dans votre liste d'acheteurs peuvent être sélectionnés).

**Rythme d'abonnement :** Sélectionnez le rythme correspondant pour l'acheteur en question.

**Méthode de paiement :** pour rappel seuls Stripe et le paiement manuel (espèce, chèque, virement bancaire) peuvent être utilisés pour la mise en place de commandes récurrentes.

**Méthode de livraison :** Sélectionnez une méthode de livraison.

**Commence :** Il s'agit de la date de démarrage de la commande récurrente.&#x20;

{% hint style="danger" %}
Si cette date est postérieure à la date d'ouverture d'un cycle de vente en cours (non encore terminée) correspondant au rythme d'abonnement défini pour la commande récurrente, une commande sera automatiquement générée pour l'acheteur pour le cycle de vente en cours. Dans le cas contraire, la première commande automatique sera passée à l'ouverture du prochain cycle de vente correspondant au rythme d'abonnement choisi.&#x20;
{% endhint %}

**Termine :** Après cette date la commande récurrente ne sera plus générée. Ce champ peut être laissé vide et dans ce cas la commande se générera indéfiniment (mais cela peut être modifié par la suite).

{% hint style="danger" %}
Si la date de fin de la commande récurrente de l'acheteur se situe après la date de début d'un cycle de vente et avant la date de fin de celui-ci, il n'y aura pas de génération de commande sur ce cycle de vente. La dernière commande ne sera générée que pour le dernier cycle de vente qui ferme avant la fermeture de leur commande récurrente.
{% endhint %}

**Adresse :** Complétez les coordonnées de votre acheteur (s'il était déjà connu de la plateforme, donc si l'acheteur a un compte et à déjà passé commande et rempli son adresse donc, les champs seront pré-remplis).&#x20;

![](<../../.gitbook/assets/image (82).png>)

{% hint style="danger" %}
Attention : si vous mettez à jour les coordonnées d'un acheteur depuis votre liste d'acheteurs, ces modifications ne seront pas répercutées sur les commandes récurrentes paramétrées. Vous devrez donc aussi préciser ces changements ici.
{% endhint %}

**Ajouter des produits :** Vous pouvez ajouter des produits proposé par le distributeur à condition que ces produits soient planifiés à la vente dans un cycle de vente à venir, et que ce cycle de vente corresponde au rythme d'abonnement choisi par l'acheteur.&#x20;

![](<../../.gitbook/assets/image (47).png>)

{% hint style="danger" %}
Vous ne pouvez pas ajouter un produit si ce dernier n'est pas proposé à la vente dans un cycle de vente futur correspondant au rythme d'abonnement de l'acheteur ! Un message d'erreur s'affichera le cas échéant.
{% endhint %}

#### Vérifier et enregistrer : relisez le tout et cliquez sur créer un abonnement ou annuler. <a href="#summary" id="summary"></a>

{% hint style="info" %}
Attention : si vous avez un cycle de vente en cours correspondant au rythme d'abonnement de la nouvelle commande récurrente saisie, dès la création de la commande récurrente, une commande va être générée et l'acheteur recevra un email de confirmation. Si vous ne souhaitez pas que la première commande automatique soit générée sur le cycle de vente en cours, assurez-vous de ne pas avoir de cycle de vente ouvert, ou mettez une date de début de commande récurrent postérieure à la fin du cycle de vente en cours.
{% endhint %}

**Que se passe-t-il si le prix d'un produit figurant dans une commande récurrente change ?**&#x20;

Les prix des produits dans les commandes récurrentes seront mis à jour selon les prix en vigeur dans le cycle de vente correspondant au déclenchement d'une nouvelle commande automatique. L'acheteur sera donc, à chaque nouvelle commande passée automatiquement en son nom, notifié de la commande passée pour lui et des prix appliqués.&#x20;

**Que se pass-t-il si un produit figurant dans une commande récurrente n'est pas disponible pour un cycle de vente donné ?**&#x20;

Dans ce cas, l'acheteur sera alerté de l'indisponibilité de certains produits dans sa confirmation de commande.&#x20;

## 7) Modifier la commande récurrente d'un acheteur <a href="#7-edit-a-customers-subscription" id="7-edit-a-customers-subscription"></a>

### Modifier tout l'abonnement <a href="#edit-the-base-subscription" id="edit-the-base-subscription"></a>

Depuis la page **Abonnements**, cliquez sur le bouton "modifier" à côté de la commande que vous souhaitez modifier.

![](<../../.gitbook/assets/image (83).png>)

A partir de là vous pouvez modifier les produits de la commande récurrente, la méthode de livraison ou de paiement, ainsi que les dates de début et de fin.&#x20;

{% hint style="info" %}
**Vous ne pouvez pas modifier le rythme d'abonnement**. Pour cela vous devez recréer une commande récurrente avec un nouveau rythme et supprimer l'ancienne.
{% endhint %}

### Modifier une commande automatique planifiée spécifique <a href="#edit-one-specific-order" id="edit-one-specific-order"></a>

Dans la colonne "commandes", cliquez sur le numéro affiché (qui représente le nombre de commandes planifiée dans le cadre de la commande récurrente. Ce nombre correspond à tous les cycles de vente à venir correspondant au rythme d'abonnement de la commande récurrente). Vous accéderez ainsi à la liste de toutes les commandes planifiées pour les prochaines cycles de vente, et vous pourrez en modifier/annuler une en particulier.&#x20;

![](<../../.gitbook/assets/image (46).png>)

### Supprimer une commande récurrente <a href="#delete-a-subscription" id="delete-a-subscription"></a>

Depuis la page **Abonnements**, cliquez sur la croix à côté de la commande récurrente. Cela supprimera définitivement la commande.

Si vous supprimez une commande alors qu'un cycle de vente est toujours ouvert, un message vous avertira afin de vous laisser l'option de garder la commande liée ou de la supprimer également. \
\


![](<../../.gitbook/assets/image (55).png>)

### Mettre en pause une commande récurrente <a href="#pause-a-subscription" id="pause-a-subscription"></a>

Depuis la page **Abonnements**, cliquez sur le bouton pause à droite de la commande que vous voulez mettre en pause. Cela stoppera les commandes automatiques de cette commande récurrente jusqu'à ce que vous cliquiez sur le bouton play (qui a remplacé le bouton pause une fois que vous avez cliqué dessus).

Si vous mettez en pause une commande alors qu'un cycle de vente est toujours ouvert, un message vous avertira afin de vous laisser l'option de garder la commande liée ou de la mettre en pause également. Et inversement si vous relancez la commande récurrente alors qu'un cycle de vente est ouvert.&#x20;



## 8) Comment sont traitées les commandes récurrentes par la plateforme ? <a href="#8-how-subscriptions-are-processed" id="8-how-subscriptions-are-processed"></a>

Une fois une commande récurrente en place pour un acheteur donné, comment cette commande est-elle traitée par le système à chaque ouverture / fermeture d'un cycle de vente ?

**1) Un cycle de vente correspondant au rythme d'abonnement de la commande récurrente est ouvert :**

* Une commande est automatiquement générée pour tous les acheteurs qui ont une commande récurrente programmée pour ce rythme d'abonnement. Un email les notifiant qu'une nouvelle commande va être passée en leur nom leur est adressé.
* Le stock des produits commandés diminue du nombre d'unités correspondant.
* Un email résumant toutes les commandes passés automatiquement ainsi que celles qui on eu des problèmes (stock insuffisant par exemple) est envoyé au responsable de la boutique.
* Les acheteurs peuvent modifier la commande automatique passée en leur nom jusqu'à la fin du cycle de vente si vous leur en avez laissé la possibilité dans vos [paramètres de boutique](broken-reference).

{% hint style="info" %}
N'oubliez pas que si vous créer une nouvelle commande récurrente pour un acheteur, et que la date de début correspond à un cycle de vente en cours, une commande automatique sera immédiatement générée pour cet acheteur.
{% endhint %}

**2) Le cycle de vente ferme**

* Les commandes générées automatiquement sont alors confirmées et l'acheteur reçoit un email de confirmation de commande.
* Si l'acheteur paye par carte de crédit (via Stripe) sa carte est alors débitée du montant final de la commande.
* Le responsable de la boutique (contact saisi dans "notifications" dans le sous menu "utilisateurs" du paramétrage d'une entreprise) reçoit un email récapitulatif des commandes passées automatiquement et des éventuelles erreurs, comme par exemple des cartes qui n'ont pas pu être débitées.

### Planifier les commandes récurrentes <a href="#planning-for-future-subscriptions" id="planning-for-future-subscriptions"></a>

Si vous proposez à vos acheteurs de passer automatiquement des commandes dans votre boutique, (soit via la commercialisation d'une formule d'abonnement, soit pour leur éviter simplement d'avoir à repasser la même commande toutes les semaines par exemple s'ils commandent leur pain de 2kg toutes les semaines), vous avez plusieurs manières de planifier vos cycles de vente futurs en lien avec l'offre que vous leur proposez :

* Vous pouvez prévoir à l'avance tous les cycles de vente de la saison par exemple, en "dupliquant" un cycle de vente type, caler les dates d'ouverture / fermeture des cycles et de remise des produits correspondantes, et associer à chaque cycle les rythmes d'abonnement concernés. Attention, il ne faudra pas oublier de vérifier la disponibilité des produits avant chaque ouverture automatique d'un cycle de vente planifié !
* Vous pouvez aussi créer les cycles de vente au fil de l'eau, d'une semaine sur l'autre, en associant sur chaque nouveau cycle les rythmes d'abonnement concernés.
