# Remboursements et ajustements de paiements

Au cours de vos ventes, vous allez sans doute être amené à procéder à des ajustements de commande

Les scénarios les plus courants sont les suivants :

1\. Un **produit au poids variable** a été commandé, et au moment de la livraison, vous allez renseigner le poids exact pour ajuster le prix réel à régler\
2\. Un produit **n'a pas été livré** par le producteur\
3\. L'acheteur a souhaité sur place **ajouter des produits** dans la commande d'origine\
4\. il y a un soucis sur la commande et vous voulez **accorder une ristourne sur cette commande**\


Deux cas de figure principaux se présentent :\
\
**A. La commande n'a pas été payée d'avance** et sera réglée sur place au moment du retrait. Dans ce cas, les ajustements sont passés avant le règlement, et ce qui sera réglé sera donc le montant final exact.

**B. La commande a été payée au moment de la commande, par Stripe ou Paypal par exemple, ou virement bancaire.** Dans ce cas, 3 situations possibles :\
\- le solde est créditeur, vous devez de l'argent à l'acheteur et souhaitez le rembourser\
\- le solde est créditeur, vous devez de l'argent à l'acheteur et souhaitez qu'il puisse utiliser ce solde pour payer en partie sa prochaine facture\
\- le solde est débiteur, il vous doit de l'argent

## A- Comment rembourser un trop perçu sur une commande ?

### a- Paiement via Stripe

Si le paiement a été effectué via votre compte marchand Stripe, le remboursement peut être géré directement via Open Food Network.

La commande que vous souhaitez ajuster est notée comme "payée" :&#x20;

<figure><img src="../../.gitbook/assets/Commande_payé_edit.jpg" alt=""><figcaption></figcaption></figure>

Vous allez vouloir soit saisir l'ajustement en édition de cette commande, c'est à dire modifier le poids du produit réel dans "**gestion des commandes par lot**, par exemple". Ici nous prenons le cas d'une modification de poids livré réellement à un acheteur : \
\
**Avant ajustement**&#x20;

<figure><img src="../../.gitbook/assets/Gestion C_poids_edit.jpg" alt=""><figcaption></figcaption></figure>

**Après ajustement** \


<figure><img src="../../.gitbook/assets/Gestion C_poids2_edit.jpg" alt=""><figcaption></figcaption></figure>

Vous constatez ensuite la commande modifiée avec le crédit sur la commande, et vous pouvez alors cliquer sur le symbole "Créditer" ici encadré sur l'image pour lancer le remboursement par Stripe sur le compte du client du crédit dû :&#x20;

![](<../../.gitbook/assets/image (39).png>)

Vous constatez bien sur votre compte Stripe le remboursement partiel :&#x20;

![](<../../.gitbook/assets/image (88) (1).png>)

{% hint style="info" %}
Le remboursement va mettre 5 à 10 jours pour apparaître sur le compte de votre acheteur.
{% endhint %}

{% hint style="info" %}
Les frais prélevés par Stripe (1,4% + 0,25 cts par transaction - voir les montants à jour sur le site de Stripe [ici](https://stripe.com/fr/pricing)) ne sont pas remboursés bien entendu, et reste prélevés sur la base du montant payé à l'origine. Il peut être parfois plus avantageux de capturer un ajustement sur la commande suivante de l'acheteur, ou lui proposer d'utiliser ses crédits pour payer une future commande (fonctionnalité qui sera développée dans les mois à venir).
{% endhint %}

Si une commande a été annulée et que vous voulez intégralement rembourser la commande, vous également pouvez le faire directement depuis l'interface Open Food Network :&#x20;

<figure><img src="../../.gitbook/assets/Commande annulée_edit.jpg" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Commande annulée2.jpg" alt=""><figcaption></figcaption></figure>

### b- Paiement via Paypal

Les remboursements partiels ou totaux de commandes réglés par Paypal ne fonctionne pas bien pour le moment sur Open Food Network. Pour l'instant aucun organisateur de circuit court n'utilise cette méthode de paiement, Stripe étant bien plus économique. Si vous souhaitez néanmoins utiliser Paypal, contactez-nous pour que nous puissions prioriser la gestion des remboursements par Paypal dans notre feuille de route.

### c- Paiement via virement bancaire

Si le paiement a été réalisé via un mode de paiement non automatique (hors Stripe et Paypal donc), mais déjà capturé comme payé, comme par exemple, via virement bancaire, vous pouvez saisir un ajustement sur la commande, et capturer un paiement négatif.

## B- Comment permettre à  un acheteur de régler partiellement sa prochaine facture avec ses crédits ?

Il vous est aussi possible de ne pas rembourser une commande, mais simplement de déduire le montant dû de la prochaine commande via un ajustement manuel sur cette prochaine commande.

{% hint style="info" %}
Nous avons le projet de permettre à un acheteur qui a des crédits disponible de les utiliser en priorité pour régler sa prochaine commande. Cette fonctionnalité n'a pas encore été développée mais [a été priorisée dans notre feuille de route](https://community.openfoodnetwork.org/t/enable-customers-to-pay-partially-or-fully-with-their-credits/1211). Si cette fonctionnalité répond aussi à votre besoin, n'hésitez pas à nous contacter pour que nous prenions en compte votre situation dans le design de la fonctionnalité.
{% endhint %}

## C- Comment prélever le montant complémentaire ?

Si vous avez ajouté à une commande déjà réglée (quel que soit le moyen de paiement) un nouvel article par exemple, vous avez la possibilité de capturer un paiement complémentaire. Ce paiement doit être capturé manuellement, et ne peut pas être prélevé via Stripe ou Paypal.&#x20;

{% hint style="info" %}
Tant que les prélèvements complémentaires sur des paiement en ligne via Stripe ou Paypal ne peuvent pas être gérés de manière satisfaisante, il peut être judicieux d'être vigilant à la façon de saisir les produits, pour éviter les ajustements positifs, et inviter à passer une commande complémentaire si un produit a été oublié, cette nouvelle commande pouvant donc être réglée via Stripe ou Paypal.
{% endhint %}
