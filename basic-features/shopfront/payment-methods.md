# Modes de Paiement

{% hint style="danger" %}
Il vous faut créer **au moins un** mode de paiement avant de pouvoir ouvrir votre boutique.
{% endhint %}

Avant de poursuivre votre lecture, nous vous proposons une démonstration rapide de la manière de configurer votre premier mode de paiement :

![](../../.gitbook/assets/paymentmethod.gif)

## Configurer un Mode de Paiement

* Accédez à la page des modes de paiement en cliquant sur **Entreprises** dans le menu horizontal bleu, puis cliquez sur **Paramètres** à côté de votre entreprise. La page des modes de paiement se trouve dans le menu de gauche. 
* Cliquez sur **Créer un nouveau mode de paiement +** . Vous serez dirigé vers une page comme celle-ci :

![](../../.gitbook/assets/paymentmethods2.jpg)

* Cochez votre entreprise, dans la case située à droite de la page intitulée "Hubs". Cela indique à quelle entreprise s'appliquera le mode de paiement que vous êtes sur le point de créer. Vous pouvez sélectionner plusieurs entreprises. 
* **Nom** : Choisissez un nom pour ce mode de paiement. \(par exemple, "Payer par carte de crédit"\). Ce nom sera affiché à la caisse et sur les e-mails de confirmation de commande des clients.

![](../../.gitbook/assets/paymentmethod2.jpg)

* **Description** : fournissez des détails supplémentaires sur le mode de paiement. Par exemple, pour un virement bancaire, vous indiquerez dans ce champ les coordonnées du compte bancaire sur lequel vous souhaitez que le client effectue le paiement BACS. Cette description est affichée à la caisse et dans les e-mails de confirmation de commande. 
* **Affichage** : Choisissez entre "visible par l'administration uniquement" et "visible par l'acheteur sur la boutique".

{% hint style="info" %}
Si vous souhaitez désactiver un mode de paiement pendant un certain temps, mais que vous souhaitez le proposer à nouveau à l'avenir \(peut-être en raison d'une épidémie de COVID, vous devez temporairement cesser de proposer des encaissements\), changez-le en "visible par l'administration uniquement".
{% endhint %}

{% hint style="warning" %}
Si vous changez tous les modes de paiement de votre entreprise en "visible par l'administration uniquement", vous obtiendrez une vitrine à affichage unique pour les cycles de commande actifs.
{% endhint %}

* **Actif** : Indiquez si ce mode de paiement est actuellement visible et disponible, ou non. 
* **Étiquettes** : Utilisez des étiquettes si vous souhaitez rendre certains modes de paiement disponibles ou non pour des clients spécifiques \(par exemple, vous pouvez autoriser uniquement les clients en gros à payer par BACS mais "obliger" les clients nationaux à payer par carte de crédit ou PayPal\). Pour plus d'informations, lisez ici. 
* **Fournisseurs de paiement** : Sélectionnez l'option correspondant au mode de paiement que vous créez. Il existe cinq options :
* * MasterCard Internet Gateway Service \(MIGS\) 
  * PayPal Express 
  * Stripe SCA
  * Espèces, chèques ou virements bancaires. Ces paiements ne passent pas par un portail de paiement en ligne et n'impliquent pas de validation automatique.

![](../../.gitbook/assets/payment-methods1.jpg)

{% hint style="warning" %}
N'oubliez pas ! Si votre entreprise a activé l'option "_**Les clients peuvent modifier ou annuler des commandes pendant qu'un cycle de commande est ouvert**_" \(dans Entreprises -&gt; Paramètres -&gt; Préférences de la boutique\), le seul fournisseur de paiement recommandé compatible avec cette fonctionnalité est "Espèces, TEF, ...".\)
{% endhint %}

* **Calculatrice** : Sélectionnez comment vous souhaitez que les frais associés au mode de paiement s'appliquent à une commande. Notez que les frais liés au mode de paiement peuvent être fixés à zéro. Voir ci-dessous pour plus d'informations sur les frais de mode de paiement.

En cliquant sur **Créer**, le mode de paiement sera créé et vous disposerez de nouveaux champs pour définir les frais du mode de paiement. Ces champs visibles dépendent de la "calculatrice" que vous avez sélectionnée.

{% hint style="info" %}
Si vous modifiez le champ "Calculatrice" du mode de paiement, vous devez d'abord enregistrer vos modifications \(Mettre à jour\) pour que les nouveaux champs associés deviennent visibles.
{% endhint %}

## Prestataires de paiement intégrés

Voici les instructions pour configurer les modes de paiement tierces Paypal, Mastercard \(MIGS\) et Strip

{% tabs %}
{% tab title="Paypal" %}
Pour configurer un mode de paiement PayPal, vous avez besoin d'un compte professionnel ou marchand PayPal. Vous pouvez en créer un ici. Une fois que vous l'avez, vous pouvez configurer un "accès API" dans PayPal, ce qui permettra à OFN de connecter les clients directement à votre compte PayPal.

1. Connectez-vous à votre compte PayPal.
2. Sous le nom de votre compte, en haut à droite, se trouve un menu déroulant intitulé "Paramètres du compte".

![](../../.gitbook/assets/paypalmay1.jpg)

3. Sélectionnez " Mettre à jour " dans Accès API

![](../../.gitbook/assets/paypalmay2.jpg)

4. Sélectionnez "Gérer les informations d'identification de l'API" dans l'option de paiement personnalisé.

![](../../.gitbook/assets/paypalmay3.jpg)

De là, vous pourrez accéder à votre nom d'utilisateur, votre mot de passe et votre signature de l'API.

![](../../.gitbook/assets/paypalmay4.jpg)

Dans OFN, assurez-vous que vous êtes connecté en tant qu'utilisateur de l'entreprise. Allez dans une entreprise et créez une méthode de paiement. Sélectionnez PayPal et remplissez les détails à partir du site PayPal. 

**Serveur** : Remplacez le champ " serveur " par " en ligne " - ce champ est sensible à la casse. 

**Identifiant** : saisissez le nom d'utilisateur de l'API. 

**Mot de passe** : saisissez le mot de passe de l'API. 

**Signature** : saisissez la signature de l'API dans ce champ.

![](../../.gitbook/assets/paypal3.jpg)

**Solution:** Solution determines whether or not a user needs a PayPal account to check out.

Type “Mark” if you do want users to have a paypal account, or “Sole” if they can checkout without a Paypal account \(with credit card\).

**Landing Page:** You can select which page to show customers once they’re redirected to PayPal.

Type “Login” to direct customer to the login form for PayPal \(if you selected “Mark” above\). Or type “Billing” to show show customers a form where they can enter their credit card data and possibly sign up for a PayPal account \(if you selected “Sole” above\).
{% endtab %}

{% tab title="MIGS" %}
 MasterCard Internet Gateway Service \(MIGS\)

Set up of this service needs to be done through your bank. So far it has been tested with Bendigo Bank.
{% endtab %}

{% tab title="Stripe" %}
[Stripe](https://stripe.com/au) is an online payment platform similar to Paypal. It will allow you to accept credit card payments from your customers. Stripe is a global platform, but is only available on certain OFN instances. Contact your [local OFN team](https://openfoodnetwork.org/ofn-local/) to see whether it’s available on your OFN.

#### Why use Stripe?

Stripe is simple to setup for shop owners and is reasonably priced. The fees charged by Stripe vary in each country; [Australia](https://stripe.com/au/pricing), [Canada](https://stripe.com/ca/pricing), [France](https://stripe.com/fr/pricing), [UK](https://stripe.com/gb/pricing), [USA](https://stripe.com/us/pricing).

Stripe is also easy for customers to use. Unlike Paypal, when the customer checks out, they don’t need to login with Paypal to place their order, rather they just need to enter their card details and then complete their order.

Stripe is the recommended payment method for shops who wish to use [**subscriptions** ](../subscriptions/)on OFN, as Stripe allows customers to give permission to a shop to automatically bill their credit card for subscription orders. This isn’t offered by Paypal, Pin or MIGS payment platforms.

#### Setup

**Connect with Stripe**

Before you can setup a payment method that uses Stripe, you’ll need to Connect with Stripe. To do this, click on the ‘Connect with Stripe’ button.

![](../../.gitbook/assets/connect-with-stripe.png)

You’ll be taken to a form to fill in your details. If you already have an account with Stripe, you can login, if not, fill in the form to create a Stripe account.

The information you’ll be asked for includes: country, a description of your business, your Business address and ABN, your personal details and your bank account \(where received payments will be deposited\).

**Create a New Payment Method**

Once you’ve connected with Stripe, you can then create a payment method which will work with your connected account.

Treat the **Name**, **Description**, **Active** and **Tags** fields as you would with any payment method.

**Provider:** Select Stripe.

Once you select Stripe, ‘Provider Settings’ will be shown.

**Stripe Account Owner:**

Select the enterprise that has a Stripe account connected.

If you select an enterprise that is not Connected to Stripe \(see above\) , you will get the error shown below. Either click ‘Connect One’ or return to your Payment Methods tab to Connect with Stripe. See instructions above.

![](../../.gitbook/assets/stripe-connect.png)

#### Stripe Payments for Customers

When customers checkout in a shop and pay with a Stripe payment method, they’ll have the options of selecting a tickbox allowing their credit card details to be stored against their account \(if they are logged in\).

Customer can also save a credit card in their Account, or delete saved ones.

![](../../.gitbook/assets/add-card.png)

When the customer next shops with an OFN shop offering Stripe as a payment method, they’ll be able to select from their saved credit cards.

**Viewing and redeeming your payments via Stripe**

When a customer pays for their order with Stripe, the funds \(minus Stripe's fees\) will go to your stripe account. Depending on your setting in Stripe the funds will be automatically transferred to your chosen bank account periodically.

**Taking further payment**

If you need to take additional payment from a customer because they have further balance due,  you can create an invoice in Stripe. The customer will get sent an email asking for them to pay with Credit/Debit card. This won't be communicated to OFN, so you'll need to mark the payment off manually.

![](../../.gitbook/assets/image%20%2831%29.png)
{% endtab %}
{% endtabs %}

## Les Frais des Modes de Paiement

![](../../.gitbook/assets/fee-calculators.png)

Vous pouvez associer des frais aux méthodes de paiement. Le plus souvent, cela sert à répercuter les frais d'un portail de paiement sur le client. Par exemple, vous pouvez faire payer le client pour le service de paiement par PayPal afin de couvrir les frais facturés par PayPal.

{% hint style="danger" %}
Les frais du mode de paiement ne comprennent pas la taxe \(TVA\).
{% endhint %}

### Calculateur de frais

**Pourcentage net** : Ces frais sont facturés en pourcentage du montant total de la commande.

{% hint style="danger" %}
Tous les **frais en pourcentage** sont calculés sur un pourcentage du **coût des produits** uniquement.
{% endhint %}

{% hint style="warning" %}
Si votre entreprise ajoute un pourcentage net de frais d'entreprise à tous les produits, alors pour obtenir le **montant** du "pourcentage net", le pourcentage souhaité du panier d'un client est le suivant:

 $$= (100 + Frais)*Pourcentage/100$$ 

Par exemple, pour une entreprise dont les frais d'entreprise sont de 20 % et qui souhaite facturer des frais de 5 % du panier total d'un client pour le paiement, le montant à saisir dans le pourcentage fixe de ce mode de paiement est le suivant :

$$= (100 + 20) *5/100 = 6$$ 
{% endhint %}

**frais fixe :** Ces frais sont appliqués comme un montant standard à toutes les commandes, quelle que soit la taille de la commande.

**frais flexible** – Ce calculateur de frais est particulièrement utile si vous souhaitez encourager les clients à passer des commandes importantes : le coût du paiement peut être réduit ou nul lorsque le nombre seuil d'articles a été atteint.

* Coût du premier article : Les frais facturés pour le premier article de la commande. 
* Coût de l'article supplémentaire : Les frais facturés pour les articles au-delà du premier article. 
* Maximum d'articles : Le nombre maximum d'articles sur lesquels les frais seront appliqués. Les articles achetés au-delà de ce nombre ne seront pas facturés.

![](../../.gitbook/assets/paymentflex.jpg)

> Par exemple : si le "Coût du premier article" est fixé à 0,20 €, le "Coût de l'article supplémentaire" à 0,10 € et le " Maximum d'articles " à 3, un client qui achète 5 articles se verra facturer 0,40 € de frais de paiement \(0,20 € pour le premier article, 0,10 € pour les articles deux et trois, et 0,00 € pour les articles quatre et cinq\).

**Frais fixe \(par article\)** : un frais constant, appliqué aux produits listés comme "articles". \(Il ne s'applique pas aux produits vendus au poids ou au volume. Par conséquent, aucun frais de mode de paiement associé ne sera facturé à un client qui, par exemple, achète du riz au kilo\). 

**Montant variable selon total commande** : Il s'agit d'un mode de paiement flexible facturé en fonction du montant total de la vente, plutôt que du nombre d'articles achetés \(tarif flexible ci-dessus\).

* Montant minimum : Valeur monétaire du seuil entre les frais du mode de paiement normal et les frais du mode de paiement réduit. 
* Montant normal : Frais de mode de paiement appliqués aux ventes inférieures au seuil indiqué dans "Montant minimum". 
* Montant de la remise : Frais de mode de paiement appliqués aux ventes supérieures au seuil indiqué dans "Montant minimum".

{% hint style="danger" %}
Le **montant minimum** correspond au _coût total des produits_ contenus dans le panier d'un client et ne comprend pas les frais d'entreprise.
{% endhint %}

{% hint style="warning" %}
Par exemple, si une entreprise ajoute des frais d'entreprise de 20 % à tous ses produits et qu'elle souhaite définir le seuil entre l'absence de frais de paiement \(Montant de la remise = 0\) et, par exemple, des frais de 0,50 € \(= Montant normal\) pour un panier de 30 €, le Montant minimum est le suivant

$$= 30 * 100 /(100+20) = 25€$$ 
{% endhint %}

![](../../.gitbook/assets/paymentpc.jpg)

{% hint style="info" %}
Les portails de paiement facturent souvent aux entreprises un montant fixe par transaction plus un petit % du coût total. Ainsi, les frais encourus par un Hub ou une boutique pour les clients qui achètent le même montant total en plusieurs petites ventes seront plus élevés que si le client faisait tous ses achats en une seule fois. 

Les calculateurs de taux flexible et de sac de prix, appliqués aux frais de méthode de paiement, peuvent s'avérer utiles pour compenser cela.
{% endhint %}

## Remboursements

L'émission et la gestion des remboursements dépendent de la manière dont le client a payé sa commande à l'origine. Vous trouverez plus de détails ici.

