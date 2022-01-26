# Méthodes de livraison

{% hint style="warning" %}
La définition d'au moins une méthode de livraison est obligatoire avant l'ouverture d'une boutique !
{% endhint %}

## Définir une méthode de livraison

**1)** **Allez sur la page méthodes de livraison**

En tant qu'administrateur, allez sur le menu bleu **Entreprises** puis cliquez sur **paramètres** et enfin sur **méthodes de livraison** dans le menu vertical de gauche :

![](<../../.gitbook/assets/image (73) (1).png>)

**2)** Cliquez sur **créer une nouvelle méthode de livraison.** Vous serez redirigé sur cette page :&#x20;

![](<../../.gitbook/assets/image (51) (1) (1).png>)

**3)** Cochez la case correspondant à votre entreprise dans l'encart à droite intitulé "Hubs". Cela permettra à la méthode de bien s'appliquer à votre entreprise. **Vous pouvez sélectionner plusieurs entreprises**.

**4) Nom :** Choisissez un nom pour la méthode. Ce nom sera affiché au client durant son processus d'achat et sur les emails de confirmation de commande. Exemple :&#x20;

![](<../../.gitbook/assets/image (61) (1) (1).png>)

**5) Description :** Ici vous pouvez ajouter des détails supplémentaires, comme l'adress précise du lieu de retrait par exemple. Ces détails seront visibles pour les clients en gris à côté du nom (cf. capture ci-dessus).

**6) Catégorie :** Est-ce une livraison (à l'adresse de l'acheteur) ou un retrait (l'acheteur doit se déplacer pour aller retirer sa commande quelque part) ?

**7) Calculateur :** Sélectionnez comment les frais de livraisons vont s'appliquer sur la commande. Notez que ces frais peuvent être équivalent à zéro. Voir ci-dessous les [options du calculateur](broken-reference).

**8) Conditions de transport :** Quelles conditions spécifiques de transport sont associées à cette méthode de livraison ?

**9) Zone :** Sélectionnez la zone appropriée (généralement EU\_VAT).



## Le calculateur

![](<../../.gitbook/assets/image (55) (1) (1).png>)

**Poids (au kg)** – Cette marge/commission correspond à un montant fixe par kg commandé. Elle _s'applique uniquement à la somme des produits vendus par kg_. Elle ne s'appliquera donc pas aux produits vendus à la pièce par exemple.

**Pourcentage net** – Cette marge/commission correspond à un pourcentage pris sur le montant total de la commande.

**Montant fixe par commande** – La marge/commission correspond à un montant fixe pris pour l'ensemble de la commande, quelle que soit sa taille ou le nombre d'articles commandés.

**Montant variable selon nb article** – La marge/commission correspond à un montant donné par commande, mais qui varie selon le nombre d'articles commandés. Il peut s'agir par exemple d'une remise promotionnelle pour des achats en grosses quantités, "si l'acheteur commande plus de X articles les frais de gestion passent de Y à Z euros".

* ‘Coût du premier produit’ : Le montant de commission pris au premier article commandé
* ‘Coût des produits suivants’ : Le montant de commission pris pour les articles suivants
* 'Produits max’ : Le nombre maximum d'articles dans le panier sur lesquels la commission va s'appliquer. Aucune commission ne sera prise sur les articles suivants.

![](<../../.gitbook/assets/image (71) (1) (1).png>)

Exemple : Si la commission prise pour le premier article est de 2€, celle de l'article supplémentaire 1 € et le nombre maximum d'article est de 3. Si un client en commande 5, il paiera 2 € pour le premier, 1€ pour le 2ème et 3ème et aucune commission pour les articles 4 et 5.

**Montant fixe par article** – Cette commission est un montant fixe qui s'applique pour chaque article commandé, mais uniquement aux articles vendus à la pièce (et non ceux vendus au poids/volume).

**Montant variable selon total commande** – Cette marge/commission est utilisée pour appliquer une marge réduite à partir du moment où la commande atteint un certain montant.

* ‘Montant minimal’ : Si la commande est en-dessous de ce montant, l'acheteur devra payer le ‘Montant normal'.
* ‘Montant de la réduction’ : Si la commande est égale ou supérieure au montant minimal, le consommateur devra payer le ‘Montant de la réduction’.
* 'Devise' : La monnaie utilisée (généralement "EUR").
