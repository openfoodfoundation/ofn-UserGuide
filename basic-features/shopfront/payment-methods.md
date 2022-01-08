# Méthodes de paiement

{% hint style="danger" %}
La définition d'au moins une méthode de paiement est obligatoire avant l'ouverture d'une boutique !
{% endhint %}

## Définir une méthode de paiement

**1) Allez sur la page méthodes de paiement**

En tant qu'administrateur, allez sur le menu bleu **Entreprises** puis cliquez sur **paramètres** et enfin sur **méthodes de paiement** dans le menu vertical de gauche :&#x20;

![](<../../.gitbook/assets/image (50).png>)

**2)** Cliquez sur "**En créer une maintenant**".&#x20;

**3)** Sélectionnez votre entreprise dans la liste des hubs dans l'encart à droite. Cela signifie que la méthode de paiement sera créée pour cette entreprise. **Vous pouvez sélectionner plusieurs entreprises**.

![](<../../.gitbook/assets/image (74).png>)

**4)** **Nom :** Choisissez un nom pour cette méthode de paiement. (par exemple : "Payez par carte de crédit via Paypal"). Ce nom s'affichera au moment du paiement pour l'acheteur, ainsi que dans les emails de confirmation qui lui seront envoyés.

**5) Description :** ajoutez les détails associés la méthode de paiement. Par exemple, pour un virement, vous pouvez indiquez les détails du RIB. Cette description s'affichera au moment du paiement pour l'acheteur, ainsi que dans les emails de confirmation qui lui seront envoyés.

Un exemple de message au moment du choix de la méthode de paiement :&#x20;

![](<../../.gitbook/assets/image (52).png>)

&#x20;**6) Active :** Indiquez si vous souhaitez que cette méthode soit visible et utilisable.

**7) Tags :** Utilisez les tags si vous souhaitez rendre certaines méthodes de paiements accessibles ou non pour certains types d'acheteurs (voir le détail de la fonctionnalité [ici](broken-reference)).

**8)** **Fournisseurs** : Sélectionnez celui qui concerne la méthode que vous êtes en train de créer. Vous pouvez accepter les paiements de 5 "fournisseurs" de systèmes de paiement :

* Espèces / chèques / virements / autres (il s'agit de liquide ou chèque ou virement bancaires ou tout autre option ne nécessitant pas de passer par un portail de paiement en ligne et n'impliquant pas de validation automatique)
* PayPal Express
* Stripe

**9) Calculateur :** Sélectionnez comment les frais éventuels associés à la méthode de paiement vont s'appliquer sur la commande. Notez que ces frais peuvent être équivalent à zéro. Voir ci-dessous les [options du calculateur](https://ofn-user-guide.gitbook.io/guide-utilisateur-open-food-network/fonctionnalites-standards/mise-en-place-dune-boutique/frais-et-taxes#le-calculateur).

En cliquant sur **Créer**, la méthode de paiement sera créée et vous aurez de nouveaux champs pour définir les frais associés au calculateur choisi. Ces champs dépendent de la sélection effectuée dans le calculateur. Ainsi, si par la suite vous changez la sélection de calculateur, il faut d'abord sauvegarder votre modification (mettre à jour) et ensuite les champs associés apparaissent.&#x20;

## Prestataires de paiement intégrés

Voici les instructions pour configurer les modes de paiement tierces Paypal, Mastercard (MIGS) et Strip

{% tabs %}
{% tab title="Paypal" %}
Pour configurer un mode de paiement PayPal, vous avez besoin d'un compte professionnel ou marchand PayPal. Vous pouvez en créer un ici. Une fois que vous l'avez, vous pouvez configurer un "accès API" dans PayPal, ce qui permettra à OFN de connecter les clients directement à votre compte PayPal.

1. Connectez-vous à votre compte PayPal.
2. Sous le nom de votre compte, en haut à droite, se trouve un menu déroulant intitulé "Paramètres du compte".

![](../../.gitbook/assets/paypalmay1.jpg)

3\. Sélectionnez " Mettre à jour " dans Accès API

![](../../.gitbook/assets/paypalmay2.jpg)

4\. Sélectionnez "Gérer les informations d'identification de l'API" dans l'option de paiement personnalisé.

![](../../.gitbook/assets/paypalmay3.jpg)

De là, vous pourrez accéder à votre nom d'utilisateur, votre mot de passe et votre signature de l'API.

![](../../.gitbook/assets/paypalmay4.jpg)

Dans OFN, assurez-vous que vous êtes connecté en tant qu'utilisateur de l'entreprise. Allez dans une entreprise et créez une méthode de paiement. Sélectionnez PayPal et remplissez les détails à partir du site PayPal.&#x20;

**Serveur** : Remplacez le champ " serveur " par " en ligne " - ce champ est sensible à la casse.&#x20;

**Identifiant** : saisissez le nom d'utilisateur de l'API.&#x20;

**Mot de passe** : saisissez le mot de passe de l'API.&#x20;

**Signature** : saisissez la signature de l'API dans ce champ.

![](../../.gitbook/assets/paypal3.jpg)

**Solution** : Solution détermine si un utilisateur a besoin ou non d'un compte PayPal pour passer à la caisse.&#x20;

Tapez "Marque" si vous voulez que les utilisateurs aient un compte Paypal, ou " Sole " s'ils peuvent passer à la caisse sans compte Paypal (avec une carte de crédit).&#x20;

**Page d'atterrissage** : Vous pouvez sélectionner la page à afficher aux clients une fois qu'ils sont redirigés vers PayPal.&#x20;

Tapez "Connexion" pour diriger le client vers le formulaire de connexion à PayPal (si vous avez sélectionné "Marque" ci-dessus). Ou tapez "Facturation" pour afficher aux clients un formulaire où ils peuvent saisir les données de leur carte de crédit et éventuellement ouvrir un compte PayPal (si vous avez sélectionné "Sole" ci-dessus).
{% endtab %}

{% tab title="MIGS" %}
&#x20;MasterCard Internet Gateway Service (MIGS)

La configuration de ce service doit être effectuée par votre banque.
{% endtab %}

{% tab title="Stripe" %}
Stripe est une plateforme de paiement en ligne similaire à Paypal. Elle vous permettra d'accepter les paiements par carte de crédit de vos clients. Stripe est une plateforme mondiale, mais n'est disponible que sur certaines instances OFN. Contactez votre équipe OFN locale pour savoir si elle est disponible sur votre OFN.

**Pourquoi utiliser Stripe ?**&#x20;

Stripe est simple à configurer pour les propriétaires de boutiques et son prix est raisonnable. Les frais facturés par Stripe varient selon les pays.&#x20;

Stripe est également facile à utiliser pour les clients. Contrairement à Paypal, lorsque le client passe à la caisse, il n'a pas besoin de se connecter à Paypal pour passer sa commande, il lui suffit d'entrer les détails de sa carte et de terminer sa commande.&#x20;

Stripe est la méthode de paiement recommandée pour les boutiques qui souhaitent utiliser les abonnements sur OFN, car Stripe permet aux clients d'autoriser une boutique à facturer automatiquement leur carte de crédit pour les commandes d'abonnement. Cette possibilité n'est pas offerte par les plateformes de paiement Paypal, Pin ou MIGS.

#### Configuration

**Connexion avec Stripe**&#x20;

Avant de pouvoir configurer un mode de paiement utilisant Stripe, vous devez vous connecter à Stripe. Pour ce faire, cliquez sur le bouton "Connecter avec Stripe".

![](../../.gitbook/assets/Connect-with-Stripe.png)

Vous serez dirigé vers un formulaire pour remplir vos coordonnées. Si vous avez déjà un compte Stripe, vous pouvez vous connecter, sinon, remplissez le formulaire pour créer un compte Stripe.&#x20;

Les informations qui vous seront demandées sont les suivantes : le pays, une description de votre activité, l'adresse et le numéro d'immatriculation de votre entreprise, vos coordonnées personnelles et votre compte bancaire (où les paiements reçus seront déposés).

**Créer un nouveau mode de paiement**&#x20;

Une fois que vous vous êtes connecté à Stripe, vous pouvez créer un mode de paiement qui fonctionnera avec votre compte connecté.&#x20;

Remplissez les champs **Nom**, **Description**, **Actif** et **Balises** comme vous le feriez avec n'importe quel mode de paiement.&#x20;

**Opérateur** : Sélectionnez Stripe.&#x20;

Une fois que vous avez sélectionné Stripe, "Paramètres du fournisseur" s'affiche.&#x20;

**Propriétaire du compte Stripe** : Sélectionnez l'entreprise qui a un compte Stripe connecté.&#x20;

Si vous sélectionnez une entreprise qui n'est pas connectée à Stripe (voir ci-dessus), vous obtiendrez l'erreur suivante. Cliquez sur "Connectez-vous" ou retournez à l'onglet Méthodes de paiement pour vous connecter à Stripe. Voir les instructions ci-dessus.

![](../../.gitbook/assets/Stripe-connect.png)

**Paiements Stripe pour les clients**&#x20;

Lorsque les clients passent à la caisse dans une boutique et paient avec un mode de paiement Stripe, ils ont la possibilité de cocher une case autorisant le stockage des détails de leur carte de crédit dans leur compte (s'ils sont connectés).&#x20;

Le client peut également enregistrer une carte de crédit dans son compte, ou supprimer celles qui ont été enregistrées.

![](../../.gitbook/assets/Add-card.png)

Lors de son prochain achat dans une boutique OFN proposant Stripe comme méthode de paiement, le client pourra choisir parmi ses cartes de crédit enregistrées.

**Consulter et encaisser vos paiements via Stripe**&#x20;

Lorsqu'un client paie sa commande avec Stripe, les fonds (moins les frais de Stripe) sont versés sur votre compte Stripe. En fonction de vos paramètres dans Stripe, les fonds seront transférés automatiquement et périodiquement sur le compte bancaire de votre choix.

**Accepter un paiement supplémentaire**&#x20;

Si vous devez demander un paiement supplémentaire à un client parce qu'il a un solde à payer, vous pouvez créer une facture dans Stripe. Le client recevra un e-mail lui demandant de payer par carte de crédit/débit. Ceci ne sera pas communiqué à OFN, vous devrez donc marquer le paiement manuellement.

![](<../../.gitbook/assets/image (17).png>)
{% endtab %}
{% endtabs %}

## Les Frais des Modes de Paiement

![](../../.gitbook/assets/Fee-calculators.png)

Vous pouvez associer des frais aux méthodes de paiement. Le plus souvent, cela sert à répercuter les frais d'un portail de paiement sur le client. Par exemple, vous pouvez faire payer le client pour le service de paiement par PayPal afin de couvrir les frais facturés par PayPal.

{% hint style="danger" %}
Les frais du mode de paiement ne comprennent pas la taxe (TVA).
{% endhint %}

### Calculateur de frais

**Pourcentage net** : Ces frais sont facturés en pourcentage du montant total de la commande.

{% hint style="danger" %}
Tous les **frais en pourcentage** sont calculés sur un pourcentage du **coût des produits** uniquement.
{% endhint %}

{% hint style="warning" %}
Si votre entreprise ajoute un pourcentage net de frais d'entreprise à tous les produits, alors pour obtenir le **montant** du "pourcentage net", le pourcentage souhaité du panier d'un client est le suivant:

&#x20;$$= (100 + Frais)*Pourcentage/100$$&#x20;

Par exemple, pour une entreprise dont les frais d'entreprise sont de 20 % et qui souhaite facturer des frais de 5 % du panier total d'un client pour le paiement, le montant à saisir dans le pourcentage fixe de ce mode de paiement est le suivant :

$$= (100 + 20) *5/100 = 6$$&#x20;
{% endhint %}

**frais fixe :** Ces frais sont appliqués comme un montant standard à toutes les commandes, quelle que soit la taille de la commande.

**frais flexible** – Ce calculateur de frais est particulièrement utile si vous souhaitez encourager les clients à passer des commandes importantes : le coût du paiement peut être réduit ou nul lorsque le nombre seuil d'articles a été atteint.

* Coût du premier article : Les frais facturés pour le premier article de la commande.&#x20;
* Coût de l'article supplémentaire : Les frais facturés pour les articles au-delà du premier article.&#x20;
* Maximum d'articles : Le nombre maximum d'articles sur lesquels les frais seront appliqués. Les articles achetés au-delà de ce nombre ne seront pas facturés.

![](../../.gitbook/assets/paymentflex.jpg)

> Par exemple : si le "Coût du premier article" est fixé à 0,20 €, le "Coût de l'article supplémentaire" à 0,10 € et le " Maximum d'articles " à 3, un client qui achète 5 articles se verra facturer 0,40 € de frais de paiement (0,20 € pour le premier article, 0,10 € pour les articles deux et trois, et 0,00 € pour les articles quatre et cinq).

**Frais fixe (par article)** : un frais constant, appliqué aux produits listés comme "articles". (Il ne s'applique pas aux produits vendus au poids ou au volume. Par conséquent, aucun frais de mode de paiement associé ne sera facturé à un client qui, par exemple, achète du riz au kilo).&#x20;

**Montant variable selon total commande** : Il s'agit d'un mode de paiement flexible facturé en fonction du montant total de la vente, plutôt que du nombre d'articles achetés (tarif flexible ci-dessus).

* Montant minimum : Valeur monétaire du seuil entre les frais du mode de paiement normal et les frais du mode de paiement réduit.&#x20;
* Montant normal : Frais de mode de paiement appliqués aux ventes inférieures au seuil indiqué dans "Montant minimum".&#x20;
* Montant de la remise : Frais de mode de paiement appliqués aux ventes supérieures au seuil indiqué dans "Montant minimum".

{% hint style="danger" %}
Le **montant minimum** correspond au _coût total des produits_ contenus dans le panier d'un client et ne comprend pas les frais d'entreprise.
{% endhint %}

{% hint style="warning" %}
Par exemple, si une entreprise ajoute des frais d'entreprise de 20 % à tous ses produits et qu'elle souhaite définir le seuil entre l'absence de frais de paiement (Montant de la remise = 0) et, par exemple, des frais de 0,50 € (= Montant normal) pour un panier de 30 €, le Montant minimum est le suivant

$$= 30 * 100 /(100+20) = 25€$$&#x20;
{% endhint %}

![](../../.gitbook/assets/paymentpc.jpg)

{% hint style="info" %}
Les portails de paiement facturent souvent aux entreprises un montant fixe par transaction plus un petit % du coût total. Ainsi, les frais encourus par un Hub ou une boutique pour les clients qui achètent le même montant total en plusieurs petites ventes seront plus élevés que si le client faisait tous ses achats en une seule fois.&#x20;

Les calculateurs de taux flexible et de sac de prix, appliqués aux frais de méthode de paiement, peuvent s'avérer utiles pour compenser cela.
{% endhint %}

## Remboursements

L'émission et la gestion des remboursements dépendent de la manière dont le client a payé sa commande à l'origine. Vous trouverez plus de détails ici.
