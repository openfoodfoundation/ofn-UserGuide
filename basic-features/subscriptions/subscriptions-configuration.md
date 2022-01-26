# Configuration



## 1) Activez les commandes récurrentes <a href="#1-enable-subscriptions" id="1-enable-subscriptions"></a>

Activez le module en vous rendant sur les paramètres de votre profil > préférences boutique : \


![](<../../.gitbook/assets/image (52).png>)

**Abonnements (= commande récurrente) :** Pour activer, sélectionnez "Activée".

**Commandes des invités** : Nous vous recommandons de désactiver cette option afin de ne pas risquer des doublons de commandes une fois les commandes récurrentes rendues possibles.

**Modifier la commande** :&#x20;

* Si vous permettez à l'acheteur de modifier la commande il va pouvoir à chaque nouvelle commande automatiquement passée en son nom modifier les quantités achetées et retirer des produits. Pour en ajouter, il devra faire une nouvelle commande.
* Dans le cas contraire, ils devront vous contacter pour réaliser des modifications. Ils pourront cependant toujours réaliser une nouvelle commande.

## 2) Vérifiez les méthodes de paiement et de livraison <a href="#2-make-sure-you-have-shipping-and-payment-methods-setup" id="2-make-sure-you-have-shipping-and-payment-methods-setup"></a>

Lorsque vous créez une commande récurrente pour un acheteur, il faut que vous indiquiez les méthodes de paiement et de livraison choisies, qui s'appliqueront donc automatiquement à chaque commande passée en leur nom par le système.

#### **Méthodes de livraison** <a href="#shipping-methods" id="shipping-methods"></a>

Il n'y a pas de restriction sur les méthodes de livraison utilisées. Pour la configuration des méthodes de livraison consultez[ la page suivante](broken-reference).&#x20;

#### **Méthodes de paiement** <a href="#payment-methods" id="payment-methods"></a>

**Vous ne pouvez utiliser que deux méthodes de paiement pour les commandes récurrentes**. Consultez [cette page](broken-reference) pour la configuration générale des méthodes de paiement.

**1) Méthode manuelle** : Espèce, chèque ou virement bancaire (sans validation automatique sur la plateforme).

**2) Stripe :** Stripe est un portail de paiement par carte bancaire équivalent à Paypal (l'obligation de créer un compte pour l'acheteur en moins). Pour voir le détail de la configuration Stripe sur une boutique, [cliquez ici](broken-reference). A chaque commande, la carte bancaire va être débitée du montant de la commande, et reflètera toute modification apportée à la commande. Rien ne sera débité si la commande récurrente a été mise en pause ou annulée.

{% hint style="info" %}
Pour que l'acheteur soit correctement débité, il est nécessaire qu'il dispose d'un compte utilisateur sur la plateforme Open Food Network, qu'il ait enregistré une carte de crédit par défaut et donné l'autorisation à votre boutique de réaliser des prélèvements automatiques. Pour plus d'informations consultez la page [Pour l'acheteur](broken-reference).
{% endhint %}

Également, si vous utilisez Stripe, pensez à bien nommer cette méthode de paiement dans votre interface d'administration.

Par exemple, au lieu de l'appeler "Paiement par carte bancaire", vous pouvez l'appeler "paiement automatique pour commande récurrente". Une description possible à ajouter : "Votre carte de crédit par défaut sera utilisée pour chaque commande récurrente non mise en pause ou annulée". Ce nom et la description associée à la méthode de paiement seront affichés sur l'email de confirmation reçu par l'acheteur, donc il est important que le bon niveau de détail soit inscrit pour que tout soit clair et que l'acheteur soit rassuré sur l'utilisation de sa carte bancaire.&#x20;

![](<../../.gitbook/assets/image (89).png>)

## 3) Récupérer les informations auprès de vos acheteurs <a href="#3-gather-information-from-your-customers" id="3-gather-information-from-your-customers"></a>

Pour créer un abonnement pour vos acheteurs, vous allez avoir besoin de certaines informations :

**Nom**, **numéro de téléphone** et **adresse e-mail :** rappelons que tout acheteur souhaitant bénéficier de commandes récurrentes a l'obligation de se créer un compte sur la plateforme. Et comme précisé dans le paragraphe suivant, vous devez l'ajouter à votre [liste d'acheteurs](broken-reference).

**Adresse de facturation et de livraison :** vous aurez besoin de ces informations pour mettre en place la commande récurrente.

**Produits :** quels produits souhaitent-ils commander de manière récurrente et automatique ?

**Méthode de livraison** : vous devez associer une méthode de livraison à la commande récurrente.

**Méthode de paiement : vous devez associer une méthode de paiement à la commande récurrente (paiement en liquide ou chèque à réception, paiement par prélèvement automatique via Stripe).** Voir [point précédent](broken-reference) pour les paiements automatiques via Stripe.

**Dates** : la date de début et de fin de la commande récurrente. Pour rappel, pour qu'une commande récurrente soit passée pour un acheteur sur un cycle de vente donné, la date de début de la commande récurrente peut être située avant ou après la date de début du cycle de vente, en revanche la date de fin de la commande récurrente doit obligatoirement se situer après la date de fin du cycle de vente.

## 4) Ajoutez les nouveaux acheteurs à votre liste <a href="#4-add-your-subscribers-to-your-customer-list" id="4-add-your-subscribers-to-your-customer-list"></a>

Avant de mettre en place une commande récurrente pour un utilisateur, vous devez l'ajouter à votre [liste d'acheteurs](broken-reference).&#x20;

**Une fois ajouté à votre liste,** demandez-leur de se créer un compte sur la plateforme. Si vous planifier d'utiliser un prélèvement automatique via Stripe pour les commandes récurrentes, vous devrez aussi leur demander de sauvegarder une carte de paiement sur leur compte et de vous autoriser à prélever sur cette carte. Toutes les étapes à réaliser de leur côté sont disponibles à la page [Pour l'acheteur](broken-reference). &#x20;

Vous pouvez aussi les ajouter à votre liste une fois leur compte créé. Dans tous les cas, il est nécessaire pour l'acheteur de disposer d'un compte valide sur la plateforme, donc il doit bien avoir confirmé son adresse email. Par ailleurs, si vous utilisez Stripe en tant que méthode de paiement, il est nécessaire de les ajouter à votre liste d'acheteurs **AVANT qu'ils autorisent votre boutique à réaliser des prélèvements**.

Ainsi, nous recommandons le processus suivant :\
1- Contactez l'acheteur pour obtenir les informations listées ci-dessus\
2- Ajoutez le à votre liste d'acheteur\
3- Ecrivez-lui en lui demandant de se créer un compte sur la plateforme (et si vous utilisez le prélèvement automatique par Stripe d'enregistrer une carte et vous autoriser à prélever dessus)\
4- [Créer ensuite seulement leur commande récurrente](broken-reference)&#x20;

## 5) Les rythmes d'abonnement <a href="#5-schedules" id="5-schedules"></a>

{% hint style="info" %}
S'il s'agit de votre première utilisation d'Open Food Network, nous vous conseillons de vous familiariser tout d'abord avec le concept de [cycle de vente](broken-reference).
{% endhint %}

### A propos <a href="#about-schedules" id="about-schedules"></a>

Une commande récurrente consiste à la passation automatique par la plateforme d'une commande prédéfinie pour un acheteur donné à chaque nouveau cycle de vente d'un distributeur donné, selon une régularité convenue entre l'acheteur et le distributeur (dite "rythme d'abonnement"). La fonctionnalité offre beaucoup de flexibilité, permettant au distributeur de proposer des "abonnements" hebdomadaires, ou bimensuels par exemple pour proposer des offres correspondant au mieux aux besoins de leurs acheteurs. Ainsi si vous disposez de plusieurs [cycles de ventes simultanés](broken-reference), un pour les particuliers et un pour les pro, peut-être n'activerez-vous pas la possibilité de commandes récurrentes pour les professionnels. Ou alors, si vous avez des cycles de ventes hebdomadaires mais permettez la commande d'un "panier produits laitiers" hebdomadaire ou bimensuel, vous pourrez définir les semaines sur lesquels seront livrées les commandes récurrentes du rythme bimensuel (cycles des semaines paires, ou cycles des semaines impaires, par exemple).

{% hint style="success" %}
Lorsqu'un rythme d'abonnement a été créé et associé à des commandes récurrentes, ces commandes ne seront lancées que pour les nouveaux cycles de vente reliés à ce rythme d'abonnement.
{% endhint %}

### Créer un rythme d'abonnement <a href="#create-a-schedule" id="create-a-schedule"></a>

Une fois les premières étapes réalisées, vous allez voir apparaître le bouton "rythme d'abonnement" dans le menu Cycle de vente. Cliquez dessus pour créer un nouveau rythme d'abonnement :&#x20;

![](<../../.gitbook/assets/image (77).png>)

{% hint style="info" %}
Attention, vous devez au moins avoir un cycle de vente ouvert ou à venir pour pouvoir configurer un rythme d'abonnement.
{% endhint %}

![](<../../.gitbook/assets/image (83) (1).png>)

**Nom :** Pensez à donner un nom logique au rythme d'abonnement. Par exemple : "hebdomadaire", "mensuel", "un jeudi sur deux"... Ce nom n'est pas visible pour les acheteurs.

{% hint style="info" %}
Attention, si vous êtes manager sur plusieurs boutiques et que vous souhaitez utiliser la fonctionnalité de commande récurrente sur plusieurs boutiques, vous devrez créé un ou plusieurs rythme(s) d'abonnement pour chaque boutique. Pensez dans ce cas à mettre des noms clairs, car tous les rythmes vous serons proposés de façon mélangés lorsque vous mettrez en place une commande récurrente. Par exemple : hebdo-quartierZ, hebdo-quartierY, etc.
{% endhint %}

Vous pouvez déplacer les cycles de ventes en utilisant les < et > boutons.

Cliquez sur "Créer" lorsque vous avez terminé.

### Modifier ou supprimer un rythme d'abonnement <a href="#edit-or-delete-a-schedule" id="edit-or-delete-a-schedule"></a>

Pour modifier ou supprimer un rythme, cliquez sur son nom dans la colonne correspondante du tableau des cycles de vente. Cette colonne peut être être rendue visible grâce à ce menu sur la page Cycle de vente : ****&#x20;

![](<../../.gitbook/assets/image (51).png>)

{% hint style="info" %}
Vous ne pouvez pas supprimer un rythme d'abonnement si des commandes récurrentes y sont associées.
{% endhint %}

### Ajouter ou supprimer un cycle de vente d'un rythme d'abonnement <a href="#adding-or-removing-order-cycles-from-schedules" id="adding-or-removing-order-cycles-from-schedules"></a>

Soit vous utilisez la fonctionnalité de modification d'un rythme décrite ci-dessus, soit vous pouvez utiliser la fonction présente dans la modification d'un cycle de vente, en ajoutant ou supprimant un rythme d'abonnement : ****&#x20;

![](<../../.gitbook/assets/image (53).png>)

{% hint style="info" %}
Un même cycle de vente peut se retrouver dans plusieurs rythmes d'abonnement !
{% endhint %}
