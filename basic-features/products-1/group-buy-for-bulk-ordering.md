# Achat Groupé - pour les commandes en gros

La fonction d'**achat groupé** est conçue pour les entreprises qui achètent une partie de leur stock entrant en grandes quantités et le revendent en plus petites unités \(par exemple, l'achat d'un sac de riz de 25 kg et la vente au détail aux clients par kg\). 

L'achat en gros est une pratique courante pour les **groupes d'achat** qui, en achetant de gros volumes, peuvent bénéficier de prix de gros au même titre que les distributeurs classiques. Ce faisant, les membres peuvent accéder à des denrées alimentaires beaucoup moins chères que celles qu'ils pourraient obtenir auprès de commerces traditionnels. 

Pour ces entreprises, la décision de commander un certain produit dépend du fait que les clients ont collectivement commandé suffisamment pour justifier un achat en gros. Cela peut être dû à des remises sur le volume ou à des frais de livraison. La fonction d'achat groupé permet au hub de réaliser plus facilement des économies sur les achats en gros. 

Lorsqu'un produit est affecté à l'achat groupé, il s'affiche avec l'étiquette "Achat groupé" sur la photo de la façade de votre magasin. Lorsqu'un client choisit d'ajouter le produit à son panier, un écran contextuel l'invite à saisir les quantités minimale et maximale, comme indiqué ci-dessous :

![](../../.gitbook/assets/bulkbuy.gif)

Les clients devront renseigner:

* Leur quantité minimale - la quantité de produit qu'ils souhaitent idéalement obtenir. 
* Leur quantité maximale - la quantité maximale qu'ils seraient prêts à acheter.

{% hint style="info" %}
Il s'agit essentiellement d'un moyen pour le client de dire "vous avez ma permission d'augmenter ma commande jusqu'à ce point, si cela signifie qu'en tant que groupe, nous pouvons atteindre la quantité de commande en gros".
{% endhint %}

Dans Gestion des Commandes Groupées, vous pouvez visualiser le total des quantités minimales et maximales commandées pour le produit, par tous vos clients. Ensuite, vous pouvez soit augmenter les commandes des clients, dans les limites de leur fourchette acceptable, pour atteindre la quantité en vrac, soit, si la quantité maximale de commande est insuffisante, supprimer toutes les commandes pour ce produit.

{% hint style="danger" %}
La fonction d'achat groupé ne peut **pas** être appliquée aux produits listés avec unités = **articles**.
{% endhint %}

## Activer l'Achat Groupé pour un produit

Sur le tableau de bord d'administration, allez à "**Produits**" dans le menu horizontal bleu. Choisissez de **modifier** un produit en cliquant sur l'icône en forme de crayon et de papier à droite du produit en question :

![](../../.gitbook/assets/productedit.jpg)

Sélectionnez ensuite **Options d'Achat Groupé** dans le menu de droite.

![](../../.gitbook/assets/groupbuy.jpg)

Sélectionnez **Oui** sous **Achat groupé ?** pour activer cette fonction pour le produit. 

La **taille de l'unité en vrac** est le montant que la commande collective du groupe doit atteindre.

{% hint style="warning" %}
Les **unités** pour la quantité de taille unitaire en vrac dépendent des unités sélectionnées pour la vente au détail du produit aux clients.

Si le produit est vendu par :

* **Poids** : les unités sont en g \(donc si le total collectif doit être égal à 5 kg, entrez "5000" dans ce champ\). 
* **Volume** : les unités sont en litres \(donc si le total collectif doit être de 10 l, entrez "10" dans ce champ\). 
* **Articles** : par exemple, si vous vendez des bouquets de fleurs mais que vous devez acheter 100 bouquets au total, entrez "100" dans ce champ.
{% endhint %}

## Ajuster les Commandes pour Compléter les lots

Sous Commandes-&gt; Gestion des commandes groupées, vous pouvez visualiser et modifier les commandes des clients pour les produits achetés en gros afin que la commande combinée de tous les clients atteigne le seuil requis.

1. Sélectionnez le cycle de commande ou la plage de dates qui vous intéresse. 
2. Recherchez le produit \(Poisson dans l'exemple ci-dessous\). 
3. Assurez-vous que la colonne "Max" est affichée afin que vous puissiez voir la limite supérieure que chaque client est prêt à acheter. 
4. Ensuite, cliquez sur la valeur \('test fish : Fish One' dans l'exemple ci-dessous\) dans la colonne **Produit : Unité**, pour afficher la case du total des commandes \(en bleu\) pour le produit en question. 
5. En utilisant les informations de la colonne **Maximum**, vous pouvez augmenter les quantités commandées pour atteindre le seuil d'un lot complet. 
6. Cliquez sur mettre à jour pour enregistrer les modifications apportées aux commandes des clients.

![](../../.gitbook/assets/bulkorder2.jpg)

Le **nombre actuel d'unités complétées** divise votre quantité totale commandée par la taille de l'unité d'achat groupé. Si ce chiffre est supérieur à 1, cela signifie que les commandes des clients existants satisfont ou dépassent la taille d'unité d'achat groupé requise. Si ce chiffre est inférieur à 1, les commandes clients existantes n'atteignent pas ce seuil. Ce chiffre augmentera au fur et à mesure que vous augmenterez la quantité de commandes clients. 

**Nombre maximal d'unités complétées** : il s'agit de la somme de toutes les quantités de commande MAX du client, divisée par la taille de l'unité d'achat groupé. Si le chiffre est supérieur à 1, vous savez que le total de vos commandes MAX dépasse la quantité requise pour l'achat groupé. S'il est inférieur à zéro, cela signifie que même les quantités de commande MAX n'atteindront pas le seuil.

