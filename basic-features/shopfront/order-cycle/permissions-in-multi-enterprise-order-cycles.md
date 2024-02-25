# Permissions dans les cycles de vente multi-acteurs



_\*Cette page explique les droits qu'a chaque acteur (producteur-fournisseur, distributeur, coordinateur) dans le contexte d'un cycle de vente impliquant plusieurs entreprises, de type "_[cycle de vente géré par un hub](https://guide.openfoodnetwork.org/v/fr/basic-features/shopfront/order-cycle/order-cycles-for-hubs)"_. Si vous souhaitez des informations sur les cycles de vente géré par un producteur,_[ _cliquez ici._](https://guide.openfoodnetwork.org/v/fr/basic-features/shopfront/order-cycle/order-cycles-for-producers)

Le coordinateur du cycle de vente est l'acteur qui a le plus de contrôle sur le cycle de vente. Les autres acteurs (fournisseurs / distributeurs) peuvent voir les commandes les concernant, et éditer les paramètres du cycle de vente qui les impliquent directement, mais ne peuvent pas modifier le cycle de vente au-delà.&#x20;

## Le coordinateur

Si le coordinateur du cycle de vente n'est pas de type "hub" (donc s'il est de type producteur non hub), l'interface complète du cycle de vente ne sera pas chargée, vous ne verrez que l'interface correspondant au [cycle de vente géré par un producteur.](https://guide.openfoodnetwork.org/v/fr/basic-features/shopfront/order-cycle/order-cycles-for-producers) Pour voir l'interface complète, assurez-vous que le coordinateur est de nature "hub". Un profil simple ne peut pas créé/géré de cycle de vente.

{% hint style="info" %}
Une fois qu'un cycle de vente est créé, son coordinateur ne peut plus être changé
{% endhint %}

Le coordinateur peut :

* Créer le cycle de vente
* Lui donner un nom et des dates de début et de fin de période de commande
* Appliquer des commissions sur l'ensemble des produits (commission coordinateur) ou sur les produits distribués par un distributeur donné (partie produits sortants) ou sur les produits d'un fournisseur donné (partie produits entrants)

### Produits entrants

* Le coordinateur peut "sourcer" son cycle de vente en appelant des fournisseurs pour lesquels il a le droit de vendre les produits. Le fournisseur en question doit donc bien avoir [créé les permissions ](https://guide.openfoodnetwork.org/v/fr/basic-features/enterprise-profile/enterprise-to-enterprise-permissions-e2es)nécessaires au coordinateur d'ajouter leurs produits dans son cycle de vente avant la création du cycle.
* Il peut sélectionner, au sein des catalogues de ces fournisseurs, les produits qu'il souhaite vendre dans ce cycle de vente.
* Il peut appliquer des commissions différenciées par fournisseur. Cela peut être utile par exemple si un fournisseur vend un type de produits pour lequel le coordinateur veut prendre une marge plus élevée. Ou si le coordinateur intègre dans son coût les frais de transport, et que pour un fournisseur donné les produits viennent de plus loin et coûtent plus cher à acheminer.

### Produits sortants

* Le coordinateur peut choisir les distributeurs via lesquels seront vendus les produits de ce cycle de vente (il peut se sélectionner lui-même). Chaque distributeur doit être de nature "hub" (hub producteur ou boutique producteur), doit avoir donné [la permission](https://guide.openfoodnetwork.org/v/fr/basic-features/enterprise-profile/enterprise-to-enterprise-permissions-e2es) au coordinateur d'ajouter des produits dans son cycle de vente, et doit bien avoir paramétré au moins une [méthode de paiement](https://guide.openfoodnetwork.org/v/fr/basic-features/shopfront/payment-methods) et une [méthode de livraison](https://guide.openfoodnetwork.org/v/fr/basic-features/shopfront/shipping-methods).

{% hint style="info" %}
Si le hub a omis de paramétrer une méthode de paiement ou une méthode de livraison, il apparaîtra dans la liste des distributeurs potentiels, mais ne pourra pas être sélectionné par le coordinateur pour être ajouté au cycle de vente.
{% endhint %}

* Il peut sélectionner, au sein de l'ensemble des produits précédemment sélectionnés dans la catégorie "produits entrants", les produits qui seront distribués dans la boutique du distributeur en question. Pour qu'un distributeur puisse voir apparaitre dans la liste des produits disponibles les produits d'un fournisseur donné, ce dernier doit avoir donné [la permission](https://guide.openfoodnetwork.org/v/fr/basic-features/enterprise-profile/enterprise-to-enterprise-permissions-e2es) à ce distributeur de vendre ses produits.
* Il peut appliquer des commissions différenciées par distributeur. Par exemple, il se peut qu'il applique une marge supérieur pour un distributeur plus éloigné pour couvrir de couts de transport supérieurs.

## Le fournisseur du cycle de vente (ajouté dans la section "produits entrants")

Le fournisseur d'un cycle de vente va voir dans le menu "cycles de vente" les cycles de vente pour lesquels il est impliqués, même s'il ne les a pas créé lui-même. En cliquant sur un de ces cycles de vente, il verra les détails de ce cycle de vente _le concernant_. Il ne verra donc pas les autres fournisseurs impliqués dans le cycle de vente par exemple. Il peut modifier les éléments le concernant, comme décocher un produit par exemple pour lequel il n'a plus suffisamment de disponibilités. Il ne peut pas modifier le nom ni les dates de période de commande du cycle de vente.

Aussi, dans le menu "rapports", le fournisseur pourra là aussi voir les commandes qu'il a reçu pour ce cycle de vente.

Le gestionnaire du cycle de vente peut choisir de laisser le fournisseur du cycle de vente visualiser le nom des **acheteurs**. Ce choix se fait dans les préférences Boutiques.\


<figure><img src="../../../.gitbook/assets/image (86).png" alt=""><figcaption><p>Option "Affichage du nom des acheteurs"</p></figcaption></figure>

### Produits entrants

* Le fournisseur peut voir, ajouter, retirer des produits de la partie "produits entrants" du cycle de vente.
* Le fournisseur peut ajouter / supprimer ses marges et commissions sur ses produits. Par exemple, si le fournisseur paie des frais de transport non inclus dans son pris de vente au hub, il peut ajouter une commission pour frais de transport qui s'appliquera au prix de ses produits, indépendamment des marges prises par le distributeur.

### Produits sortants

Les droits qu'a un fournisseur sur la gestion de ses produits dans la partie "produits sortants" dépendent de la[ permission](https://guide.openfoodnetwork.org/v/fr/basic-features/enterprise-profile/enterprise-to-enterprise-permissions-e2es) que lui a accordé le distributeur en question.&#x20;

* Si le distributeur l'a autorisé à ajouter des produits aux cycles de ventes, le fournisseur va pouvoir voir, ajouter, retirer des produits de la liste des produits sortants du distributeur.
* Si le distributeur n'a pas donné cette autorisation, le fournisseur va pouvoir voir ses produits dans la liste des produits sortants du distributeur mais ne pourra ni en ajouter ni en retirer.
* Dans tous les cas, le fournisseur ne peut pas modifier les dates de livraison/retrait ni les précisions sur les modalités de livraison/retrait, et ne peut pas non plus modifier les marges et commissions appliquées par le distributeur.

## Le distributeur du cycle de vente (ajouté dans la section "produits sortants")

Le distributeur d'un cycle de vente va voir dans le menu "cycles de vente" les cycles de vente pour lesquels il est impliqués, même s'il ne les a pas créé lui-même. En cliquant sur un de ces cycles de vente, il verra les détails de ce cycle de vente _le concernant_. Il ne verra donc pas les autres distributeurs impliqués dans le cycle de vente par exemple. Il peut modifier les éléments le concernant, comme les dates et informations de livraison / retrait et les marges et commissions. Il ne peut pas modifier le nom ni les dates de période de commande du cycle de vente.

Aussi, dans le menu "rapports", le distributeur pourra voir les commandes qu'il a reçu pour ce cycle de vente, avec les noms des acheteurs, qui apparaitront dans sa liste d'acheteurs.

### Produits entrants

Le distributeur peut voir les produits entrants des producteurs qui lui ont donné l'autorisation de vendre leurs produits, mais ne peuvent pas modifier leur disponibilité, ni ajouter de marges et commissions sur un fournisseur donné (seul le coordinateur peut faire ça, ou le fournisseur concerné).&#x20;

{% hint style="info" %}
Pour l'instant, seul le coordinateur du cycle de vente peut ajouter des fournisseurs au cycle de vente. Le distributeur n'en a pas le pouvoir.
{% endhint %}

### Produits sortants

Les droits qu'a un distributeur sur la gestion des produits dans la partie "produits sortants" dépendent de la [permission](https://guide.openfoodnetwork.org/v/fr/basic-features/enterprise-profile/enterprise-to-enterprise-permissions-e2es) que lui a accordé le fournisseur.&#x20;

* Le distributeur peut voir, ajouter, retirer des produits de sa liste de produits sortants uniquement pour les fournisseurs qui lui ont [donné l'autorisation](broken-reference) de vendre leurs produits.
* Il peut modifier les dates de livraison/retrait et les précisions sur les modalités de livraison/retrait
* Il peut modifier les marges et commissions appliquées
