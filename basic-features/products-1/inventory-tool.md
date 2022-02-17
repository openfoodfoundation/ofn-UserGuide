# Catalogue boutique

{% hint style="warning" %}
L’usage du catalogue boutique complexifie considérablement votre usage du logiciel Open Food Network, nous vous conseillons de vous assurer de votre besoin avant de vous engager dans son utilisation. Si vous avez un doute, ou souhaitez confirmer la pertinence de son utilisation, [contactez-nous](https://ofn-user-guide.gitbook.io/guide-utilisateur-open-food-network/#dautres-questions-des-ameliorations)
{% endhint %}

## Introduction

La fonctionnalité catalogue boutique permet à un hub-distributeur A de modifier uniquement pour sa boutique les informations de prix et stock des produits pour lesquels il a la [permission](https://guide.openfoodnetwork.org/v/fr/basic-features/enterprise-profile/enterprise-to-enterprise-permissions-e2es) adéquate, et de faire sa sous-sélection de produits en masquant les produits qu'il ne souhaite pas distribuer, sans que cela n'affecte le catalogue d'origine du producteur. Ainsi, si un autre hub-distributeur B offre dans sa boutique les mêmes produits du même producteur, il ne sera pas affecté par les changements effectués par A dans son catalogue boutique.

## Paramètres du profil concernant le catalogue boutique

Pour y accéder, rendez-vous sur **Entreprises**, puis "**paramètres**" et enfin "c**atalogue boutique**" dans le menu vertical de gauche :

![](<../../.gitbook/assets/image (42) (1) (1).png>)

Vous avez deux options :&#x20;

1. Les nouveaux produits ajoutés par vos fournisseurs doivent être préalablement ajoutés à votre catalogue boutique avant de pouvoir être ajoutés à vos cycle de vente. Quand vous créerez un cycle de vente, vous ne verrez dans les produits "entrants" que les produits préalablement ajoutés à votre catalogue boutique.&#x20;
2. Les produits ajoutés par vos fournisseurs peuvent être ajoutés à votre boutique en ligne sans que vous n'ayez à les ajouter au préalable dans votre catalogue boutique. Quand vous créerez un cycle de vente, vous verrez dans les produits "entrants" l'ensemble des produits des producteurs sélectionnés. Bien sûr, si vous avez modifié dans votre catalogue boutiques les prix ou stock de certains de ces produits, ce sont bien ces informations là qui seront affichées dans votre boutique. Si vous ne pensez pas utiliser le catalogue, sélectionnez cette option recommandée.&#x20;

## Accéder au catalogue boutique

Cliquez sur le menu **Produits** dans l'interface d'administration, puis sur **Catalogue** **boutique** dans le sous menu vert. Si vous gérez plusieurs boutiques, il vous sera demandé d'en sélectionner une car chaque catalogue est géré indépendamment.&#x20;

![](<../../.gitbook/assets/image (65) (1) (1) (1).png>)

Lors de chaque visite de ce catalogue boutique, si de nouveaux produits ont été ajoutés par vos fournisseurs, un message vous alertera sur le fait que vous avez de nouveaux produits disponibles pouvant être ajoutés à votre catalogue. Tant que ce ne sera pas fait, ils resteront dans la catégorie "**Nouveaux produits**".

![](<../../.gitbook/assets/image (55) (1) (1) (1).png>)

En cliquant sur "**vérifier maintenant**" vous serez redirigé vers la liste des **nouveaux produits**.

## Nouveaux produits

![](<../../.gitbook/assets/image (48) (1) (1).png>)

Les nouveaux produits peuvent être soit **ajoutés** à votre catalogue, soit **masqués**. Si vous souhaitez modifier pour votre boutique les caractéristiques prix/stock d'un produit de la liste, vous devez l'ajouter à votre catalogue boutique. S'il s'agit d'un produit que vous ne voudrez jamais vendre dans votre boutique ou en tout cas pas à court terme, vous pouvez choisir de le masquer.

Pour rappel, si l'option choisie dans les [paramètres](https://guide.openfoodnetwork.org/v/fr/basic-features/enterprise-profile/enterprise-settings#catalogue-boutique) est que les produits doivent être ajoutés à votre catalogue pour pouvoir être ajoutés dans un cycle de vente et donc mis en vente dans votre boutique en ligne, tous les produits que vous laissez dans la liste "nouveaux produits" seront par défaut masqués, c'est-à-dire qu'ils ne pourront pas être sélectionnés dans vos cycles de vente. Si l'autre option a été choisie, ils pourront être ajoutés dans vos cycles de vente.&#x20;

## Produits du Catalogue Boutique

![](<../../.gitbook/assets/image (37) (1) (1).png>)

Via le bouton colonnes à droite, vous pouvez choisir les éléments de paramétrage que vous souhaitez pouvoir voir et modifier lorsque cela est permis.&#x20;

![](<../../.gitbook/assets/image (71) (1) (1) (1).png>)

### Modifier pour votre boutique les prix, stocks et références produits

Toutes les modifications que vous ferez ici seront visibles sur votre boutique. Vous pouvez modifier les champs suivants (mais pas les autres, c'est-à-dire le nom du produit, le conditionnement, ou encore la description ou l'image) :

* **Référence produit :** vous pouvez ici indiquer une autre référence produit que celle du producteur
* **Prix :** le prix est modifiable mais n'oubliez pas que les quantités unitaires associées ne le sont pas
* **En stock :** si votre stock disponible pour ce produit diffère du stock disponible proposé par le producteurs, vous pouvez indiquer votre stock. Vos produits ne seront plus visibles dans la boutique une fois que cette valeur atteint zéro.
* **A volonté :** vous pouvez sélectionner si le produit est vendu à la demande ou suivant un stock défini, ou si vous souhaitez garder le même paramètre que celui figurant au catalogue producteur.

### Réinitialiser les niveaux de stock par défaut

Cette colonne permet de revenir à un stock par défaut, par exemple au début de chaque nouveau cycle de vente, selon votre stratégie de réassort. Si vous souhaitez utiliser cette fonctionnalité, cochez la case et renseignez le stock par défaut dans la case avoisinante pour les produits concernés. Pour réinitialiser le stock par défaut pour ces produits, cliquez sur **Action** puis **Réinitialiser les niveaux de stock par défaut.** Seuls les produits avec une case cochée seront affectés par cette action.

C'est utile par exemple pour les hubs-distributeurs qui savent que chaque mois ils auront de nouveaux arrivages définis pour certains produits pour remettre leur stock défini à niveau avant la prochaine vente.

### Hériter ?

Si vous n'avez rien modifié sur un produit, la case à cocher "hériter?" est sélectionnée par défaut. Cela signifie que les informations entrées par le producteur et visibles en gris seront reprises et publiées sur la boutique. En modifiant tous les champs ou juste certains, cette case à cocher se dé-sélectionnera automatiquement.

Pour revenir aux informations producteurs, vous pouvez à tout moment re-sélectionner cette case.

### Masquer des produits

En cliquant sur le bouton masquer, les produits en question disparaîtront de la liste des nouveaux produits ou du catalogue boutique et seront basculés vers la liste des produits masqués. Ils ne font plus partie de votre catalogue boutique, et ne pourront donc pas être ajoutés à vos cycles de vente si vous avez choisi l'option vous obligeant à ajouter les produits à votre catalogue avant de pouvoir les vendre dans votre boutique.

{% hint style="warning" %}
N'oubliez pas de sauvegarder vos modifications !
{% endhint %}

## Produits masqués

La liste des produits que vous avez décidé de masquer se trouve ici :&#x20;

![](<../../.gitbook/assets/image (45) (1) (1) (1) (1).png>)

Sur cette page, vous pouvez décider d'ajouter à votre catalogue boutique certains produits préalablement masqués en cliquant sur le bouton "Ajouter" :

![](<../../.gitbook/assets/image (47) (1) (1).png>)

## Catalogue boutique et cycle de vente

Dans le menu Cycle de vente > Modifier un cycle de vente, si vous cliquez sur "paramètres avancés" vous disposez d'une option pour choisir si - sur ce cycle en particulier - les informations viennent de votre catalogue ou directement des fournisseurs :

![](<../../.gitbook/assets/image (46) (1) (1).png>)
