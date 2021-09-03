# Fixation des Prix de Viande et autres produits " entiers " de poids inconnu

Nous qualifions d'**irréguliers** les produits qui sont vendus en fonction de leur poids/volume, mais dont la quantité exacte n'est connue qu'au moment de la récolte/distribution. Par exemple, des morceaux de viande, des tranches de fromage, des gros légumes. 

Il existe un certain nombre d'outils différents disponibles sur la plateforme OFN pour aider à gérer et organiser ces ventes.

## Première option : fixer un poids/prix moyen et rembourser

Vous pouvez facturer le prix moyen du produit, puis rembourser ou facturer le client en supplément, si le poids réel s'écarte de la moyenne. 

Lorsque vous connaissez le poids réel des produits \(c'est-à-dire lorsque vous préparez les commandes pour la collecte par les clients\), connectez-vous à " Gestion des commandes groupées " \(Commandes -&gt; Gestion des commandes groupées\) et ajoutez la colonne Poids / Volume au tableau.

![](../../.gitbook/assets/bom1.jpg)

Vous pouvez alors modifier le poids affiché pour chaque acheteur pour une commande donnée et un produit donné. Le prix sera recalculé automatiquement en fonction de la quantité saisie.

{% hint style="info" %}
N'oubliez pas de renvoyer un e-mail de confirmation de commande au client pour l'informer de la différence de prix et de toute somme à payer en plus par la suite.
{% endhint %}

## Deuxième option : Afficher les fourchettes de prix

Même logique que l'option 1, mais au lieu d'afficher initialement un prix moyen, indiquez une fourchette de prix. Cette solution présente l'avantage d'indiquer clairement à l'acheteur que le prix final est susceptible de changer. 

Les variantes peuvent également être utilisées pour créer différentes fourchettes.

> **Exemple 1** \(un seul produit et une seule variante\) : 
>
> Produit = Poulet \(entre 8 et 12 kg avec prix selon le poids, 10 £ / kg\) 
>
> **Exemple 2** \(deux variantes pour un seul produit\) : 
>
> Produit = Poulet \(10 £ / kg\) 
>
> Variante 1 = Petit poulet \(entre 8 et 12 kg, prix en fonction du poids réel\) 
>
> Variante 2 = Gros poulet \(entre 13 et 20 kg, prix en fonction du poids réel\) ...

## Troisième option : Créer des variantes à prix fixe 

Une version un peu plus simple de la deuxième option consiste à créer des variantes pour vos produits sur la base de fourchettes de poids, mais à facturer un **prix fixe** pour tous les articles qui entrent dans la fourchette. Par exemple, si la courge butternut coûte 1 €/kg, vous pouvez lister les variantes avec les prix fixes suivants :

* Petite \(0.7 - 0.9 kg\) 0,80€. 
* Moyenne \(0.9 - 1.1 kg\) 1,00€. 
* Grande \(1,1 - 1,3 kg\) 1,20€ 
* Extra grande \(1.3 - 1.5 kg\) 1,40€

## Quatrième option : Créer des variantes avec des poids définis

Si vous connaissez à l'avance le poids de tous vos steaks, par exemple, vous pouvez utiliser la fonctionnalité de variante pour afficher directement le prix précis de chaque article. Par exemple :

![](../../.gitbook/assets/knownweight.jpg)

## Modifier des commandes

Il peut être difficile pour les producteurs de viande de connaître à l'avance la disponibilité des produits ou de préparer leurs emballages en conséquence. \(Jusqu'à l'abattage, le poids d'un poulet ou d'un gigot d'agneau peut être inconnu\). 

Ce n'est pas un problème puisque les commandes peuvent être modifiées \(en ajoutant, modifiant ou supprimant des produits\) si nécessaire. Pour plus d'informations, voir Commandes.

## Rembourser ou réclamer aux clients la différence : Comment ça fonctionne ?

Si un client **paie ses marchandises à la collecte ou à la livraison**, le gestionnaire du hub aura pu modifier la commande avant le paiement en fonction du poids réel et des produits livrés. Dans ce cas, il ne sera donc pas nécessaire de rembourser ou de facturer à nouveau le client. 

Si une commande **est payée en ligne avant la livraison**, alors vous devez rembourser ou facturer la différence entre la somme déjà reçue et celle due pour les produits précis à livrer. Cliquez ici pour voir comment procéder.

{% hint style="danger" %}
Une alternative consiste à utiliser un système de paiement en ligne pour stocker temporairement le montant "en attente" jusqu'à ce que la commande ait été validée. 

_Cette fonctionnalité n'est pas encore implémentée dans Open Food Network. Nous travaillons également sur l'implémentation automatisée de "crédits" permettant à un hub de rembourser sous la forme d'une note de crédit qui pourrait être utilisée par le client comme paiement partiel pour sa prochaine commande._
{% endhint %}

## Informez l'acheteur de votre système de prix 

Vous pouvez informer vos clients de vos politiques de tarification pour les articles à poids variable \(tels que la viande\) dans la boîte de message affichée en haut de la façade de votre boutique. Cette option se trouve dans les paramètres d'entreprise -&gt; Préférences de la boutique. 

Il peut être utile d'ajouter un rappel de ces politiques de prix dans le champ de description des modes de paiement. Par exemple, vous pouvez ajouter : "N'oubliez pas que le prix final peut varier de 10 % en fonction du poids si vous avez acheté des articles non divisibles tels que de la viande ou de gros légumes".

