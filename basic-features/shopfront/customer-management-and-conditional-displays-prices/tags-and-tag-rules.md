# Affichages et prix conditionnels selon la catégorie d'acheteurs (tags)

## Règles de tags

Une fois les acheteurs regroupés par catégories, c'est à dire une fois qu'un tag leur a été associé, ([voir page précédente](https://guide.openfoodnetwork.org/v/fr/basic-features/shopfront/customer-management-and-conditional-displays-prices/customers)), vous allez pouvoir définir les règles d'affichage suivantes :&#x20;

* Rendre des cycles de vente visibles ou invisibles : par exemple, vous souhaitez créer des cycles de vente différents pour les acheteurs professionnels ou les CE d'entreprises, avec des marges différentes de celles appliquées aux particuliers, et souhaitez que ces cycles de ventes ne soient accessibles qu'à ces professionnels ; ou bien vous êtes un groupement d'achat et souhaitez réserver un cycle de vente aux membres de votre GA
* Rendre des méthodes de livraison visibles ou invisibles : cela peut-être utile si vous souhaitez par exemple réserver la livraison à domicile à des habitants de certains quartiers, ou à des membres "VIP" ;
* Rendre des méthodes de paiement visibles ou invisibles : par exemple, vous souhaitez réserver le paiement sur place aux membres de votre collectif ;
* Rendre certaines variantes visibles ou invisibles : cette règle permet de rendre une variante (déclinaison d'un produit) visible ou invisible dans la boutique pour certaines acheteurs.

## Comment paramétrer une règle de tag

Allez sur le menu **Entreprises** > **Paramètres** > **Règles de tag.**

Cliquez sur "**Ajouter une c par défaut**".

<figure><img src="../../../.gitbook/assets/Screen Shot 2022-11-24 at 13.28.31.png" alt=""><figcaption></figcaption></figure>

Choisir le type de règle et validez.

<figure><img src="../../../.gitbook/assets/Screen Shot 2022-11-24 at 13.27.39.png" alt=""><figcaption></figcaption></figure>

Entrez le tag pour lequel vous souhaitez rendre invisible la fonctionnalité. Par exemple ici, nous rendons invisible par défaut les cycles de vente tagués "ce-entreprise" :

<figure><img src="../../../.gitbook/assets/Screen Shot 2022-11-24 at 13.32.13.png" alt=""><figcaption></figcaption></figure>

Maintenant, cliquez sur le bouton rouge "**Ajouter une règle conditionnelle**", puis sur "**Ajouter une nouvelle règle**".&#x20;

<figure><img src="../../../.gitbook/assets/Screen Shot 2022-11-24 at 12.38.05.png" alt=""><figcaption></figcaption></figure>

Entrez les noms des tags désirés dans les champs disponibles. Par exemple, dans l'exemple ci-dessous, nous définissons que seuls les acheteurs ayant le tag "ce-entreprise", pourront voir les cycles de vente tagués "ce-entreprise". Ces cycles de vente seront invisibles pour tous les acheteurs ne disposant pas de ce tag.

<figure><img src="../../../.gitbook/assets/Screen Shot 2022-11-24 at 12.37.51.png" alt=""><figcaption></figcaption></figure>



Nous devons maintenant ajouter les tags au niveau des fonctionnalités à rendre visible ou invisible :&#x20;

#### Afficher ou masquer les cycles de vente de ma boutique

Dans l'onglet "Cycle de vente", modifiez votre cycle de vente et entrez le nom du tag dans le champ "tag".

<figure><img src="../../../.gitbook/assets/Screen Shot 2022-11-24 at 12.47.20.png" alt=""><figcaption></figcaption></figure>

Pour les boutiques multi-producteurs, le tag est à l'étape 3 du cycle de vente.

#### Afficher ou masquer des méthodes de livraison&#x20;

Pour cette règle, modifiez votre méthode de livraison dans l'onglet Entreprise > bouton Paramètres > onglet Méthodes de livraison.&#x20;

Dans l'exemple ci-dessous, la méthode de livraison "à domicile" est taggée "vip".

![](<../../../.gitbook/assets/image (53) (1) (1).png>)

#### Afficher ou masquer des méthodes de paiement&#x20;

Pour cette règle, modifiez votre méthode de livraison dans l'onglet Entreprise > bouton Paramètres > onglet Méthodes de paiement.  Dans l'exemple ci-dessous, un paiement sur facture sera une option proposée uniquement aux acheteurs professionnels.&#x20;

![](<../../../.gitbook/assets/image (83) (1) (1).png>)

#### Afficher ou masquer des variantes dans ma boutique

&#x20;Pour cette règle, le tag sur la variante est à associer au niveau du [catalogue boutique](https://guide.openfoodnetwork.org/v/fr/basic-features/products-1/inventory-tool) et pas dans le catalogue du producteur concerné.&#x20;





## Utiliser les tags pour gérer des tarifications différenciées selon la catégorie d'acheteur/ tarification sociale

Parfois, vous souhaitez appliquer des tarifications différentes selon le type d'acheteur : bénéficiaire d'un tarif social, membre d'un groupement d'achat ou non-membre, particuliers ou profesionnels, etc.&#x20;

Plusieurs possibilités de paramétrages utilisant les règles de tag sont à votre disposition  :

* Vous pouvez créer [deux cycles de vente](https://guide.openfoodnetwork.org/v/fr/basic-features/shopfront/order-cycle) : un cycle de vente pour les acheteurs tagués, un autre pour les non-tagués. Sur le cycle de vente dédié aux non-tagués, vous pouvez appliquer une commission supérieure.&#x20;
* Vous pouvez proposer une[ méthode de livraison](https://guide.openfoodnetwork.org/v/fr/basic-features/shopfront/shipping-methods) réservée aux acheteurs (exemple : "retrait au dépôt (membres)" vs "retrait au dépôt (non membres)", et associer des frais inférieurs, voir des frais négatifs (correspondant donc à une ristourne) pour la méthode concernant les membres. Quand le membre choisi cette méthode, le prix de sa commande est adapté (le montant total diminue si des frais négatifs sont associés). En revanche, cela implique de vérifier que l'acheteur ne triche pas lorsqu'il sélectionne la méthode correspondant à son profil, ou alors de taguer les membres "membres" et la méthode de paiement qui leur est réservée avec le même tag et paramétrer une règle de tag.
* Vous pouvez proposer une[ méthode de paiement](https://guide.openfoodnetwork.org/v/fr/basic-features/shopfront/payment-methods) avec des frais négatifs (ce qui correspondra à une ristourne donc) et réserver grâce aux tags cette méthode de paiement à des acheteurs professionnels par exemple.&#x20;

Exemple d'une initiative qui utilise la tarification sociale sur CoopCircuits :thumbsup:

> Le collectif en charge du point relais demande aux consommateurices de fournir un justificatif de quotient familial. Si ce dernier est inférieur à un certain niveau, les acheteurs peuvent bénéficier d'une tarification sociale (20% de réduction sur les achats).&#x20;
>
> Pour mettre cela en place dans CoopCircuits, le collectif a réalisé la configuration suivante&#x20;
>
> * dans l'onglet "Acheteurs", le collectif  attribue un tag "tarif réduit" aux emails correspondant aux bénéficiaires&#x20;
> * une méthode de paiement spécifique existe, tagguée "tarif réduit", et propose une réduction/marge négative de 20%&#x20;
> * une règle de tag définit que la méthode de paiement tagguée "tarif réduit" ne sera visible qu'aux mails taggués "tarif réduit"
>
> Ainsi,  les personnes bénéficiaires du tarif social peuvent, à la fin de la prise de commandes, choisir la méthode de paiement "tarif réduit" et bénéficier du tarif préférentiel sur l'ensemble de leur panier, soit 20% de remise.

{% hint style="info" %}
Au delà de l'usage des tags, il est possible d'utiliser la fonctionnalité "catalogue boutique" pour gérer des tarifications différenciées. Vous pouvez par exemple créé une boutique pour les acheteurs pro, dont vous ne communiquer l'url qu'à ces acheteurs. Cette boutique peut gérer un catalogue boutique et modifier les prix des produits qui s'afficheront dans la boutique. Cette solution peut être utile lorsque la ristourne appliquée aux professionnels ne suit aucune "règle" fixe, et que les prix sont définis produits par produits.
{% endhint %}

{% hint style="info" %}
**ATTENTION**: N'oubliez pas de définir vos [règles de tag](https://guide.openfoodnetwork.org/v/fr/basic-features/shopfront/customer-management-and-conditional-displays-prices/tags-and-tag-rules#regles-de-tags) afin que les tags fonctionnent !
{% endhint %}

&#x20;
