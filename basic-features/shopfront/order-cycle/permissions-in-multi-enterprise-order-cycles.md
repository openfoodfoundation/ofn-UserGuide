# Les cycles de commande multi-entreprise

Cette page explique les différents droits dont dispose chaque entreprise dans le cadre de cycles de commande complexes impliquant plusieurs entreprises. Soit :

* le producteur \(profil ou boutique\) qui fournit uniquement le cycle de commande
* un hub qui distribue les marchandises uniquement
* un hub qui coordonne le cycle de commande \(et peut ou non également fournir ou distribuer des biens\)

Pour plus de détails sur les cycles de commande simples impliquant un seul producteur vendant uniquement son propre stock \(boutique de producteur\), voir ici.

_**Le coordinateur a le plus haut degré de contrôle sur un cycle de commande. Les autres entreprises peuvent visualiser les cycles de commande dans lesquels elles sont impliquées, mais uniquement modifier les paramètres qui les concernent.**_

## Le Coordinateur

{% hint style="info" %}
La **fonctionnalité complète du cycle de commande** ne peut être obtenue que si une entreprise est enregistrée en tant que Hub. Pour changer votre type d'entreprise, voir ici.
{% endhint %}

{% hint style="warning" %}
Une fois qu'un cycle de commande a été créé, il n'est pas possible de modifier le coordinateur.
{% endhint %}

Le  coordinateur d'un cycle de commande peut

* Créer les cycles de commande. 
* Définir et modifier le nom du cycle de commande ainsi que les dates d'ouverture et de fermeture. 
* Appliquer les taxes d'entreprise à tous les produits \(taxe de coordination\), aux produits fournis par les producteurs \(dans la section entrante\), et/ou aux produits distribués par les hubs \(dans la section sortante\).

### **Approvisionnement**

* Le coordinateur peut ajouter des entreprises en tant que fournisseurs. Toutefois, pour ce faire, l'entreprise fournisseur \(enregistrée comme producteur auprès de l'OFN\) doit avoir accordé au centre de coordination l'autorisation d'ajouter ses produits à un cycle de commande. 
* Le coordinateur peut sélectionner tous les produits ou un sous-ensemble de produits de ses fournisseurs qu'il souhaite inclure dans le cycle de commande. 
* Le coordinateur peut appliquer des frais d'entreprise différentiels à chaque fournisseur. Par exemple, il peut souhaiter facturer un boucher fournisseur à un tarif plus élevé \(pour couvrir le coût supplémentaire du transport réfrigéré\) qu'un boulanger.

### **Distribution**

Le coordinateur peut choisir les entreprises par lesquelles les produits listés dans un cycle de commande sont distribués \(y compris sa propre entreprise\). 

Pour ce faire, chaque distributeur potentiel doit :

1. Être enregistré en tant que hub. 
2. Avoir accordé au hub coordinateur la permission d'ajouter des produits à un cycle de commande. 
3. Avoir au moins une méthode d'expédition et de paiement active.

{% hint style="info" %}
Si une entreprise de distribution potentielle apparaît parmi les options possibles dans la partie sortante du cycle de commande mais ne peut être sélectionnée, elle n'a probablement pas encore configuré les méthodes d'expédition et/ou de paiement.
{% endhint %}

Le coordinateur peut choisir parmi la liste complète des produits entrants, qui sera affichée sur la vitrine de chaque plateforme de distribution. _**Le fournisseur \(profil de producteur ou magasin\) doit avoir mis en place une autorisation d'entreprise de "cycle d'ajout à la commande" entre lui et le centre de distribution spécifique \(ainsi que le coordinateur\).**_

Le coordinateur peut, s'il le souhaite, appliquer des frais d'entreprise différentiels à chaque centre de distribution. Cela peut être avantageux si un concentrateur est plus éloigné du coordinateur qu'un autre, et donc si les frais de transport qui lui sont associés sont plus élevés.

## Entreprises de fournisseurs 

Le fournisseur \(producteur\) peut voir tous les cycles de commande auxquels il participe en visitant la page de résumé du cycle de commande \(à partir du menu bleu horizontal supérieur\), même s'il n'a pas créé les cycles de commande lui-même. En cliquant sur le cycle de commande, un producteur entrant ne peut voir que ses détails, et non les produits ou les détails des autres personnes impliquées dans le cycle de commande. Il peut modifier les éléments qui le concernent : par exemple, il peut supprimer un produit en rupture de stock d'un cycle de commande. Une entreprise de fournisseur ne peut pas modifier le nom ni les dates d'un cycle de commande. 

Dans la section Rapports \(menu bleu horizontal supérieur\), un producteur fournisseur entrant peut visualiser les commandes qu'il a reçues pour le cycle de commande.

{% hint style="warning" %}
Une entreprise de fournisseur ne voit pas automatiquement les noms des clients qui ont acheté ses produits si elle n'est pas également le coordinateur du cycle de commande. Ce paramètre peut être modifié par le coordinateur du cycle de commande \(entreprise qui gère le cycle de commande\). Si vous avez besoin de voir les noms des clients pour faciliter l'emballage et l'exécution des commandes, vous pouvez contacter votre coordinateur du cycle de commande et lui demander de cocher la case Noms des clients dans les rapports dans les paramètres de l'entreprise sous Préférences de la boutique.
{% endhint %}

### **Approvisionnement**

* Un fournisseur peut visualiser, ajouter et supprimer **ses** produits dans la section "Produits entrants" d'un cycle de commande. 
* Un fournisseur peut ajouter/supprimer les frais d'entreprise qui sont appliqués à **ses** produits dans la section "Produits entrants" du cycle de commande. Cela peut être utile pour les producteurs qui fournissent plusieurs hubs, dont certains sont beaucoup plus éloignés d'eux que d'autres. Ils peuvent souhaiter ajouter un prélèvement supplémentaire aux hubs plus éloignés pour couvrir les coûts de transport.

### **Distribution**

Le degré d'influence d'un fournisseur sur ses produits dans la section "Produits sortants" d'un cycle de commande dépend des autorisations d'entreprise spécifiques qu'il a accordées au centre de distribution et vice versa.

* Si le hub de distribution a accordé au producteur fournisseur \(profil, magasin ou hub\) le droit d'"ajouter au cycle de commande \[du hub\]", le fournisseur peut visualiser, ajouter et supprimer des produits de la liste dans la section "Produits sortants" du cycle de commande. 
* Si le hub de distribution n'a pas accordé au producteur fournisseur \(profil, magasin ou hub\) le droit d'"ajouter au cycle de commande \[du hub\]", alors le fournisseur peut voir mais PAS ajouter et supprimer des produits de la liste dans la section "Produits sortants" du cycle de commande. 
* Un fournisseur n'est jamais en mesure de modifier les détails de l'enlèvement et de la livraison, ni les frais d'entreprise appliqués au distributeur.

## Entreprises de distributeurs

Un distributeur peut voir les cycles de commande auxquels il participe dans sa page de résumé des cycles de commande, même s'il ne les a pas créés lui-même \(c'est-à-dire s'il n'est pas le coordinateur du cycle de commande\). En cliquant sur un cycle de commande, l'entreprise distributrice sortante peut voir les détails d'un cycle de commande qui ne concernent qu'elle. \(Par exemple, si elle n'est pas l'unique distributeur du cycle de commande, elle ne pourra pas voir qui sont les autres entreprises distributrices ni les produits qu'elles proposeront sur leur façade de magasin\). Le centre de distribution sortant peut voir et modifier les détails de sa distribution - dates et méthodes de livraison, et frais d'entreprise pour la distribution - mais pas le nom ni la période du cycle de commande lui-même. 

Dans le menu "Rapports", un distributeur de cycle de commande peut voir les commandes qui ont été passées \(avec les noms des clients\) pour faciliter la livraison/l'expédition des marchandises.

### **Approvisionnement** 

Un distributeur peut _**voir**_ les produits entrants des fournisseurs qui lui ont accordé l'autorisation d'entreprise "ajouter au cycle de commande" mais il ne peut pas modifier les niveaux de stock/disponibilité ni appliquer/supprimer les frais d'entreprise spécifiques aux producteurs.

{% hint style="warning" %}
Actuellement, seul le coordinateur d'un cycle de commande peut y ajouter des fournisseurs \(producteurs\) supplémentaires.
{% endhint %}

### **Distribution**

Le degré d'influence du centre de distribution sur les produits de la section "produits sortants" d'un cycle de commande dépend des permissions d'entreprise entre lui et le producteur fournisseur.

Le centre de distribution peut

* Ajouter/supprimer des produits de son échange sortant. Cela s'applique uniquement aux produits des producteurs qui ont été ajoutés au cycle de commande par le coordinateur et qui ont accordé au distributeur l'autorisation d'entreprise "ajouter au cycle de commande". 
* Modifier les détails de l'enlèvement et de la livraison 
* Ajouter/supprimer leurs frais d'entreprise

