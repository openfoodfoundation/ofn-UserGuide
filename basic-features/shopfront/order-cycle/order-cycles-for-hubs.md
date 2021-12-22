# Cycles de commande (pour les Hubs)

{% hint style="warning" %}
Lisez la suite si vous avez sélectionné le profil d'entreprise " Hub producteur ou non producteur ".&#x20;

Visitez cette page si vous vous êtes inscrit en tant que " boutique de producteur " et que vous souhaitez configurer un cycle de commande pour votre vitrine.
{% endhint %}

Vous ouvrez votre boutique en créant un cycle de commande. Lorsque vous créez un cycle de commande, vous choisissez quand votre boutique est ouverte, quels produits seront mis en ligne et quels frais vous appliquerez.

**Pourquoi des cycles de commande ?**

Certains hubs peuvent souhaiter avoir une boutique en ligne ouverte en permanence, et remplir les commandes une par une, au fur et à mesure qu'elles sont reçues. Cependant, de nombreux hubs fonctionnent selon un système de commande périodique, qui leur permet de traiter les commandes en vrac, ce qui rend leurs activités de production, d'emballage et de distribution plus efficaces (et réduit les frais généraux associés).&#x20;

Par exemple, un cycle de commande peut être ouvert pendant deux semaines. À la fin de la quinzaine, toutes les commandes seront emballées et livrées à la même heure le mercredi suivant. Une fois que ce lot de commandes aura été livré, un nouveau cycle de commande pourra être rouvert.&#x20;

Démonstration rapide de la mise en place d'un nouveau cycle de commande :

![](../../../.gitbook/assets/ordercyclehub.gif)

## Visualiser les cycles de commande

Vous pouvez créer un cycle de commande et consulter les cycles de commande précédents en cliquant sur **Gérer les cycles de commande** dans votre tableau de bord.

![](../../../.gitbook/assets/ordercycledash.jpg)

Ou à partir du menu horizontal en haut de la page.

![](<../../../.gitbook/assets/ordercycle1 (2).jpg>)

{% hint style="warning" %}
Vous ne pourrez pas publier un cycle de commande en direct tant que vous n'aurez pas configuré au moins une méthode de paiement et d'expédition pour votre entreprise.
{% endhint %}

## Créer un nouveau cycle de commande

La première étape consiste à sélectionner un coordinateur pour votre cycle de commande. Seule l'entreprise qui coordonne un cycle de commande a le droit de modifier et de gérer **tous** les aspects du cycle de vente. Les autres entreprises impliquées dans un cycle de commande (en tant que fournisseurs ou distributeurs uniquement) auront un accès restreint.&#x20;

Pour plus d'informations sur la gestion inter-entreprises dans le contexte des cycles de commande, cliquez ici.

![](../../../.gitbook/assets/ordercycle2.jpg)

Une fois que le coordinateur du cycle de commande a été choisi, le processus de mise en place est divisé en trois étapes :

### 1) Paramètres généraux

![](../../../.gitbook/assets/ordercycle3.jpg)

**Nom (**_**obligatoire**_**)** : Donnez au cycle de commande un nom qui a du sens pour vous. Nous vous recommandons de suivre un protocole de dénomination cohérent, par exemple FoodHub\_Week27\_2014. Nous vous recommandons également d'inclure le nom de votre hub dans le nom du cycle de commande, afin que le service d'assistance OFN puisse identifier vos cycles de commande si vous avez besoin d'aide.&#x20;

**Ouverture des commandes** : Il s'agit de la date et de l'heure à laquelle votre magasin OFN sera ouvert, visible et commencera à accepter les commandes des clients.&#x20;

**Fermeture des commandes** : Il s'agit de la date (et de l'heure) à laquelle votre boutique OFN fermera et cessera d'accepter des commandes. Si vous avez l'intention d'avoir un cycle de commande ouvert en permanence, sélectionnez une date de fermeture bien éloignée dans le temps.&#x20;

**Programmation** : Laissez vide, sauf si proposez des abonnements.&#x20;

**Ajouter les frais du coordinateur** : En tant que hub, le coordinateur est très probablement vous-même. Vous pouvez appliquer ici vos frais d'entreprise, qui font office de majoration. Les frais seront calculés en fonction du calculateur sélectionné dans Frais d'entreprise. Vous ne pouvez appliquer des frais d'entreprise que s'ils ont déjà été créés.

### 2) Produits entrants

![](../../../.gitbook/assets/ordercycle4.jpg)

Sur cette page, vous pouvez sélectionner les producteurs, et leurs produits, qui seront disponibles dans ce cycle de commande. Dans le menu déroulant, vous verrez tous les producteurs qui vous ont donné l'autorisation d'ajouter leurs produits à votre cycle de commande (voir la section **Autorisations d'entreprise**). Après avoir sélectionné un fournisseur et cliqué sur Ajouter un fournisseur, tous les produits associés à ce fournisseur seront visibles. Cochez les produits que vous souhaitez ajouter au magasin, ou cliquez sur Sélectionner tout.

{% hint style="info" %}
Les produits qui sont en rupture de stock (c'est-à-dire que leur valeur "en stock" est nulle) sont inclus dans cette liste. S'ils sont ajoutés à un cycle de commande, ils n'apparaîtront pas sur votre vitrine. Il est toujours bon de vérifier les niveaux de stock.
{% endhint %}

Le champ "**Détails de réception**" est facultatif. Les informations ajoutées dans ce champ seront automatiquement ajoutées à tout courriel envoyé aux producteurs à la fin d'un cycle de commande (après avoir cliqué sur "Notifier les producteurs"). Il peut être judicieux d'indiquer ici l'adresse exacte de livraison des produits avant leur distribution aux clients.&#x20;

Le bouton "**Ajouter des frais**" de cette section, situé à la fin de l'entrée de chaque producteur dans le tableau, vous permet d'ajouter différents frais d'entreprise à différents fournisseurs. Par exemple, le transport de farine ou de produits lourds vers les clients peut être plus coûteux pour un hub que pour une salade. Par conséquent, un hub peut, de manière transparente, ajouter des frais d'entreprise légèrement plus élevés à toutes les marchandises fournies par le meunier que par le producteur de salades.&#x20;

Sélectionnez le nom de l'entreprise dans la première case déroulante, puis cliquez sur le nom de la redevance d'entreprise dans la deuxième case déroulante. Dans l'exemple ci-dessous, un frais d'entreprise nommé OrderAdmin est appliqué au producteur de fruits.

![Apply enterprise fee to incoming supplier](../../../.gitbook/assets/Enterprise-Fee.png)

{% hint style="warning" %}
Ces frais seront appliqués à tous les produits du producteur de fruits qui sont achetés. Les frais sont calculés selon le calculateur de frais qui a été sélectionné lors de la création des frais d'entreprise.
{% endhint %}

### 3) Produits sortants

Ici, vous pouvez sélectionner un ou plusieurs hub-distributeurs. Tous les hubs choisis pour être distributeur dans ce cycle de commande auront une façade ouverte pour la durée du cycle de commande. Dans un **modèle simple**, un seul hub est listé comme distributeur unique pour le cycle de commande. Sélectionnez le hub, et cochez la case "Sélectionner tout" pour ajouter tous les produits entrants à la vitrine. Pour plus de flexibilité, le même cycle de commande peut avoir **plusieurs distributeurs**. Dans ce cas, vous pouvez sélectionner un sous-ensemble différent de produits entrants disponibles pour chaque distributeur, et/ou ajouter des dates de livraison différentes pour chacun d'entre eux.

![](../../../.gitbook/assets/oc3.jpg)

La colonne des **balises** vous permet de marquer vos cycles de commande afin de personnaliser leur visibilité ou leur invisibilité pour certains clients. Voir balises et règles de balisage pour plus d'informations.&#x20;

La case "**prêt pour (date/heure)**" (obligatoire) : Ce champ indique au client quand sa commande sera prête pour l'enlèvement ou la livraison. Si votre cycle de commande est perpétuel et que vous exécutez les commandes au cas par cas plutôt qu'en vrac, vous devez indiquer quelque chose comme "Deux jours après réception de la commande". L'exemple ci-dessous montre comment un client peut basculer entre différents cycles de commande pour sélectionner la date qui lui convient le mieux.

![](<../../../.gitbook/assets/multipleoc3 (1).jpg>)

{% hint style="info" %}
Si vous opérez avec une vitrine ouverte en continu (c'est-à-dire que vous avez fixé la date de clôture de votre cycle de commande plus de 3 mois à l'avance), la case bleue "Prêt pour" sur votre vitrine indiquera "Les commandes sont actuellement ouvertes".
{% endhint %}

La note est également affichée à la caisse, lorsque le client sélectionne son mode d'expédition (voir ci-dessous) et est incluse dans l'e-mail de confirmation de la commande.

![](../../../.gitbook/assets/readyfor2.jpg)

Le message d'**instructions de collecte** sera inclus dans l'e-mail de confirmation de commande du client, sous le message correspondant au mode d'expédition choisi (voir ci-dessous). Cette note est conçue pour n'être visible que par les clients. Vous pouvez donc y inclure des informations plus sensibles, comme des adresses ou des numéros de téléphone, etc. Vous trouverez ci-dessous un exemple d'e-mail de confirmation de commande.

![collection details message](../../../.gitbook/assets/Collection-details.png)

**Ajouter des frais** : Là encore, des frais d'entreprise précédemment créés peuvent être attribués à ce distributeur. Pour les modèles simples (avec un distributeur central, qui est également le coordinateur du cycle de commande), l'ajout d'une commission à ce stade revient à ajouter une "commission de coordinateur" (elle s'appliquera à tous les produits). Pour les modèles complexes, le coordinateur peut souhaiter ajouter des frais différents pour tous les produits vendus par chaque distributeur. Le meilleur endroit pour implémenter cette fonctionnalité est ici.

### Ouvrir la vitrine

Cliquez sur **Enregistrer** pour programmer le cycle de commande. Si la date d'ouverture est déjà passée, votre boutique est instantanément ouverte ! Si vous n'êtes pas prêt à ouvrir tout de suite, saisissez des dates dans le futur, que vous pourrez modifier ultérieurement.&#x20;

Pour les cycles de commande périodiques et répétitifs, vous pouvez copier un cycle de commande existant et en modifier les dates, afin d'accélérer le processus. Voir ci-dessous.

![](../../../.gitbook/assets/occpy.jpg)

Les cycles de commande s'affichent en vert lorsqu'ils sont actifs, en jaune lorsqu'ils sont programmés pour une date ultérieure et en gris lorsqu'ils sont fermés. Lorsqu'un cycle de commande a été clôturé il y a plus d'un mois, il ne s'affiche plus dans cette liste. Pour afficher tous vos cycles de commande passés, cliquez sur "Afficher plus" en haut de la liste.

## Le Bouton 'Notifier les Producteurs'

En utilisant ce bouton en haut de la page, tous les producteurs liés au cycle de commande recevront un courriel contenant une liste des produits commandés jusqu'à présent pour ce cycle de commande particulier.

![](../../../.gitbook/assets/notifyproducers.jpg)

Lorsque le bouton " Notifier les producteurs " est sélectionné, une demande de confirmation apparaît. Une fois confirmé, un courriel sera automatiquement envoyé à tous les producteurs concernés. Cet e-mail comprendra les instructions de livraison (si ce champ est rempli dans la section des produits entrants) ainsi que les informations suivantes sur le produit :

* Numéros de produits (si applicable)&#x20;
* Nom du fournisseur&#x20;
* Nom du produit&#x20;
* Quantité commandée&#x20;
* Prix par unité&#x20;
* Sous-total par produit&#x20;
* Taxe incluse ( si applicable)\


## Rapports de Producteurs/Fournisseurs

Si votre cycle de commande comprend des produits provenant de producteurs/fournisseurs liés, ceux-ci pourront se connecter à leur compte OFN et consulter des rapports sur le cycle de commande. Par défaut, ils ne seront pas en mesure de voir les détails des clients dans ces rapports. Si vous souhaitez que vos fournisseurs aient accès aux noms des clients dans leurs rapports, vous pouvez ajuster ces paramètres dans les préférences de la boutique dans vos paramètres d'entreprise.
