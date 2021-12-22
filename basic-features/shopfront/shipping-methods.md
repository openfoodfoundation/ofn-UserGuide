# Méthodes d'Expédition

{% hint style="warning" %}
Il vous faut créer **au moins une** méthode d'expédition avant de pouvoir ouvrir votre boutique.
{% endhint %}

Avant de poursuivre votre lecture, nous vous proposons une démonstration rapide de la manière de configurer votre première méthode d'expédition :

![](../../.gitbook/assets/shippingmethod.gif)

## Configurer une méthode d'expédition

* Accédez à la page Méthodes d'expédition en cliquant sur **Entreprises** dans le menu horizontal bleu, puis cliquez sur **Paramètres** à côté de votre entreprise. La page **Méthodes d'expédition** se trouve dans le menu sur le côté gauche.&#x20;
* Cliquez sur **Créer une nouvelle méthode d'expédition +** . Vous serez dirigé vers une page comme celle-ci :

![](../../.gitbook/assets/shippingmethods.jpg)

* Cochez la case située à côté de votre entreprise sur le côté droit de la page, sous "Hubs". Cela indique que la méthode d'expédition que vous êtes sur le point de créer s'appliquera à cette entreprise. Vous pouvez sélectionner plusieurs entreprises, si vous le souhaitez.&#x20;
* **Nom** : Choisissez un nom pour la méthode. Ce nom sera affiché au client pendant le processus d'achat et dans les courriers électroniques de confirmation de la commande. Exemple :

![](<../../.gitbook/assets/shippinginfo (1).jpg>)

* **Description** : Ajoutez des détails supplémentaires, tels que l'adresse précise du point de collecte. Ces détails seront visibles par les clients en gris à côté du nom (voir la capture d'écran ci-dessus) et dans leur e-mail de confirmation de commande.&#x20;
* **Affichage** : Choisissez entre "visible par l'administration uniquement" et "visible par l'acheteur sur la boutique".

{% hint style="info" %}
Si vous souhaitez désactiver une méthode d'expédition pendant un certain temps, mais que vous souhaitez la proposer à nouveau à l'avenir (peut-être un point de collecte réservé à l'été et que vous ne souhaitez pas mettre à la disposition des clients en hiver), changez-la en "visible par l'administration uniquement".
{% endhint %}

* **Catégorie de méthode** : Cette méthode est-elle une livraison ou un point de retrait ?&#x20;
* **Étiquettes** : entrez des étiquettes ici si vous souhaitez différencier les clients. Les étiquettes peuvent être utiles si vous souhaitez offrir la livraison gratuite à une catégorie de clients ou offrir la livraison uniquement à ceux qui ont une adresse enregistrée à proximité. Plus d'informations ici.&#x20;
* **Calculateur** : Sélectionnez la manière dont les frais d'expédition seront ajoutés à cette méthode d'expédition. Notez que les frais d'expédition peuvent être nuls. Voir ci-dessous pour plus de détails.&#x20;
* **Catégorie de taxe** : Cette option vous permet de définir la taxe associée à votre méthode d'expédition/frais de collecte indépendamment de celle affectée aux produits taxables détenus par votre entreprise. Les options sont les suivantes : aucune, taux plein, taux zéro, taux réduit ou frais d'expédition.&#x20;
* **Catégories de transport** : Les conditions de transport (réfrigération, congélation, par défaut) associées à cette méthode d'expédition.

{% hint style="danger" %}
Cochez toutes les cases qui s'appliquent à votre entreprise alimentaire. Par exemple, si vous vendez des produits dont la catégorie d'expédition est "congelé", pour que le client puisse régler ses achats, la catégorie "congelé" devra être cochée dans le mode d'expédition souhaité.
{% endhint %}

* **Zones** : Sélectionnez la zone appropriée (pour permettre un calcul correct des taxes).

En cliquant sur **Créer**, la méthode d'expédition sera créée, et de nouveaux champs vous seront proposés pour ajouter des détails sur les frais de la méthode d'expédition. Les champs présentés dépendent du calculateur de frais d'expédition que vous avez sélectionné.

{% hint style="info" %}
Si vous modifiez le type de calculateur pour une méthode d'expédition, vous devez d'abord **enregistrer** avant de pouvoir modifier les paramètres du calculateur.
{% endhint %}

## Calculateurs de Frais

![](../../.gitbook/assets/shippingcalc.jpg)

**Pourcentage net** - Ces frais sont facturés en pourcentage du montant total de la commande.

{% hint style="danger" %}
Tous les **frais en pourcentage** sont calculés sur un pourcentage du **coût des produits** uniquement.
{% endhint %}

{% hint style="warning" %}
Si votre entreprise ajoute un pourcentage fixe de frais d'entreprise à tous les produits, alors pour obtenir le **montant** du "pourcentage net", le pourcentage souhaité du panier d'un client est le suivant :&#x20;

&#x20;$$= (100 + Frais)*Pourcentage/100$$&#x20;

Par exemple, pour une entreprise dont les frais d'entreprise sont de 20 % et qui souhaite facturer des frais d'expédition correspondant à 5 % du panier total d'un client, le montant à saisir dans le pourcentage fixe de ce mode d'expédition est le suivant :

$$= (100 + 20) *5/100 = 6$$&#x20;
{% endhint %}

**Poids (par kg)** - ces frais sont appliqués aux produits sur une base par kg. _Ces frais ne seront appliqués qu'aux produits dont le prix est calculé par kg_, et non aux produits répertoriés comme articles (par exemple, un produit répertorié comme "1 botte de persil" ne contribuera pas au montant total des frais d'expédition facturés au client).&#x20;

**Montant fixe par commande** - Ce tarif est appliqué comme tarif standard à toutes les commandes, quelle que soit leur taille.&#x20;

**Montant fixe par article** - Ces frais sont constants et s'appliquent aux produits répertoriés comme "articles". (Il ne s'applique pas aux produits vendus au poids ou au volume. Par conséquent, aucun frais d'expédition ne sera facturé à un client qui, par exemple, achète du riz au kilo).&#x20;

**Montant variable selon le nombre d'articles** - Ce calculateur de frais est particulièrement utile si vous souhaitez encourager les clients à passer des commandes importantes : le coût de l'expédition peut être réduit ou nul lorsque le seuil du nombre d'articles a été atteint.

* Coût du premier article : Les frais facturés pour le premier article de la commande.&#x20;
* Coût d'article supplémentaire : Les frais facturés pour les articles au-delà du premier article.&#x20;
* Articles maximum : Le nombre maximum d'articles sur lesquels les frais seront appliqués. Les articles achetés au-delà de ce nombre ne seront pas facturés.

![](../../.gitbook/assets/shippingfeeflex.jpg)

> Par exemple : Si les frais d'expédition pour le "Coût du premier article" sont de 2 €, le "Coût de l'article supplémentaire" = 1 € et le "Nombre maximal d'articles" = 3: Un client qui achète 5 articles se verra facturer 4 € de frais de port (2 € pour le premier article, 1 € pour les articles deux et trois, et 0 € pour les articles quatre et cinq).

**Montant variable selon la commande** - Il s'agit d'une méthode de frais d'expédition flexible facturée en fonction du montant total de la vente, plutôt que du nombre d'articles achetés (tarif flexible ci-dessus).

* Montant minimum : Valeur monétaire du seuil entre les frais d'expédition normaux et les frais d'expédition réduits.&#x20;
* Montant normal : Frais d'expédition appliqués aux ventes inférieures au seuil indiqué dans "Montant minimum".&#x20;
* Frais réduit : Frais de port appliqués aux ventes supérieures au seuil indiqué dans 'Montant minimum'.

{% hint style="danger" %}
Le **montant minimum** correspond au _**coût total des produits**_ contenus dans le panier d'un client et ne comprend pas les frais d'entreprise.
{% endhint %}

{% hint style="warning" %}
Par exemple, si une entreprise ajoute des frais d'entreprise de 20 % à tous les produits et qu'elle souhaite fixer le seuil entre la livraison gratuite (montant de la remise = 0) et, par exemple, la livraison à 5 € (= montant normal) à un panier de 30 €, le montant minimum est le suivant

$$= 30 * 100 /(100+20) = 25 €$$&#x20;
{% endhint %}

![](../../.gitbook/assets/shippingfeepc.jpg)
