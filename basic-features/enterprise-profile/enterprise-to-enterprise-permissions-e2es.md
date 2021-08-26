# Autorisations d'entreprise

## Autorisations d'entreprise

Dans le cadre des autorisations d'entreprise de l'OFN se trouvent des règles qui régissent les relations commerciales entre les entreprises : fournisseurs et distributeurs. Ces règles doivent être mises en place avant qu'une entreprise \(Profil de producteur ou Boutique de producteur\) puisse devenir le fournisseur d'une autre \(Hub\). Une permission \(ou "droit"\) est accordée par une entreprise à une autre concernant l'accès / la modification des produits et du profil. Cette page détaille les différentes permissions et la manière de les attribuer. 

Pour accéder aux autorisations de votre entreprise :

![](../../.gitbook/assets/permissions.gif)

Nous allons aborder ce sujet des points de vue suivants:

* [un Hub](enterprise-to-enterprise-permissions-e2es.md#hub-perspective) \(le distributeur\)
* un profil de producteur ou une boutique \(le fournisseur\)

## Les quatre autorisations 

Il existe 4 types différents d'autorisations d'entreprise. On peut les configurer de différentes manières pour donner aux entreprises plus ou moins de droits en fonction de leurs profils.

![](../../.gitbook/assets/e2emenu2.jpg)

**Autorisation d'ajouter au cycle de commande** : le fournisseur \(producteur\) autorise le distributeur \(un hub OFN\) à ajouter des produits aux cycles de commande de ce dernier. Ainsi, les produits du fournisseur peuvent apparaître sur la vitrine du hub. 

**Autorisation de gérer des produits** : le fournisseur autorise une autre entreprise enregistrée auprès d'OFN \(généralement un hub\) à créer, supprimer et modifier des produits directement dans son catalogue fournisseur.

{% hint style="danger" %}
Cela peut potentiellement avoir un impact sur tous les hubs que le producteur fournit via OFN.
{% endhint %}

> _Par exemple, si l'agriculteur Jo fournit des pommes de terre aux plateformes A et B mais qu'il autorise la plateforme A à gérer ses produits, si la plateforme A modifie le prix des pommes de terre, ce changement de prix \(dans le cadre des paramètres standard\) sera répercuté sur les devantures des deux plateformes A et B._

**Autorisation de modifier le profil** : une entreprise autorise une autre à modifier les détails de son profil d'entreprise \(coordonnées, adresse, description, ...\). 

**Autorisation d'ajouter des produits à l'inventaire** : le fournisseur \(producteur\) autorise le distributeur \(hub\) à ajouter ses produits au catalogue \(ou 'Inventaire'\) du hub.

{% hint style="info" %}
Si un producteur approvisionne plus d'un hub en marchandises, alors pour permettre à chacun de ces hubs de gérer les prix et les niveaux de stock de leurs produits de manière indépendante, nous recommandons d'ajouter cette permission entre les deux entreprises et aux hubs de modifier leurs paramètres d'inventaire.
{% endhint %}

## Accorder et Gérer les Autorisations

Pour modifier, ajouter ou supprimer des autorisations, rendez-vous dans le tableau de bord de l'administrateur, puis sélectionnez "Entreprises" dans le menu bleu et "Autorisations" dans le sous-menu vert.

![](../../.gitbook/assets/e2emenu.jpg)

Pour donner une autorisation :

* Sélectionnez votre entreprise dans le menu déroulant de la première colonne \(vous êtes un producteur qui fournit d'autres personnes\). 
* Sélectionnez le nom de l'entreprise \(hub\) que vous souhaitez approvisionner dans la deuxième colonne. 
* Cochez les autorisations que vous souhaitez accorder au distributeur de vos marchandises \(hub\) ou, pour accorder plusieurs autorisations, sélectionnez "tout". 
* Cliquez sur "Créer".

Notez que vous pouvez supprimer ou modifier ces autorisations à tout moment.

{% hint style="warning" %}
Seuls les utilisateurs qui sont gestionnaires de l'entreprise peuvent modifier ses permissions.
{% endhint %}



Si vous avez besoin qu'une autre entreprise vous accorde des autorisations, vous devez la contacter par courriel ou par téléphone. Il n'existe pas de fonction en ligne pour ce faire.

## Les Autorisations Gérées Automatiquement

Lorsqu'un utilisateur est le gestionnaire principal \(propriétaire\) de plusieurs entreprises sur la plateforme, les autorisations sont créées automatiquement entre chaque entreprise. Ce n'est pas le cas lorsque les entreprises sont gérées par des utilisateurs différents.

## Pour les Hubs

Ces situations courantes illustrent quelles autorisations d'entreprise vous devrez configurer pour votre hub.

> **J'ai créé des profils de producteur pour chacun de mes fournisseurs. Quelles autorisations dois-je configurer avant de pouvoir stocker leurs produits sur la vitrine de mon Hub ?**

Le système est configuré de manière à ce que les hubs qui créent des profils de producteurs aient _les autorisations correctes installées par défaut_, afin qu'ils puissent commencer à ajouter des produits et à échanger avec ces profils de producteurs immédiatement.

> **Mon fournisseur a déjà une entreprise enregistrée auprès de l'OFN. Je voudrais ajouter leurs produits à la vitrine de mon hub.**

Vous devez contacter votre fournisseur en personne. Ses coordonnées \(numéro de téléphone, adresse et adresse électronique\) se trouvent dans son profil OFN.

Si vous avez uniquement l'intention de _**stocker leurs produits**_ et ne souhaitez pas les aider à gérer le reste de leur profil OFN, demandez au producteur de vous accorder la permission d'_**ajouter au cycle de commande**_ et la permission d'_**ajouter à l'inventaire**_. 

Si le fournisseur souhaite que vous, en tant que gestionnaire de Hub, l'aidiez à organiser son entreprise OFN, il peut vous accorder les quatre permissions. Dans ce cas, vous serez en mesure de modifier son profil et de gérer ses produits.

> **Mon Hub distribue par le biais de groupes d'achat. De quelles autorisations le groupe d'achat aura-t-il besoin avec mon hub et mes producteurs ?**

{% hint style="warning" %}
Ceci est un cas où le centre qui gère \(coordonne\) un cycle de commande diffère de l'entreprise auprès de laquelle les clients collectent leurs achats. 

_Si le centre A gère \(coordonne\) un cycle de commande pour un groupe d'acheteurs \(centre B\), alors le cycle de commande sera affiché sur la vitrine OFN du centre B._
{% endhint %}

Le groupe d'achat \(Hub B ci-dessus\) devra accorder au coordinateur du cycle de commande \(Hub A ci-dessus\) l'autorisation d'ajouter au cycle de commande \(et de préférence l'autorisation d'ajouter à l'inventaire\).

Les producteurs qui fournissent au hub A des produits qui seront également vendus par le groupe d'achat \(hub B\) doivent accorder aux deux hub A et B l'autorisation d'ajouter au cycle de commande \(et de préférence l'autorisation d'ajouter à l'inventaire\).

## Pour les Producteurs

Lorsqu'un producteur souhaite commencer à vendre ses produits par l'intermédiaire d'autres entreprises \(hubs ou groupes d'achat\), il doit établir les autorisations appropriées d'entreprise à entreprise. Il existe différents niveaux d'autorisation qu'un producteur peut accorder, en fonction du pouvoir qu'il souhaite donner au hub pour gérer ses produits et son profil \(voir le haut de page\). 

Ces exemples explorent quelques scénarios courants.

> **Je suis un producteur et j'aimerais qu'un hub OFN local stocke et vende mes produits.**

**Essentiel** : Pour que le hub puisse ajouter vos produits à sa vitrine, vous devez lui accorder la "permission d'ajouter au cycle de commande". 

**Facultatif** : vous pouvez également donner au hub l'autorisation de gérer vos produits, de modifier votre profil ou d'ajouter à l'inventaire.

> **Un hub que je fournis distribue par le biais de groupes d'achat.**

Pour que vos produits puissent être distribués par les groupes d'achat, vous devez ajouter au minimum l'autorisation "d'ajouter au cycle de commande" pour l'entreprise du groupe d'achat ainsi que pour le hub que vous fournissez directement.

> **Je suis une boutique de producteurs qui approvisionne un Hub local tout en gérant ma propre vitrine. Le hub aimerait gérer les niveaux de stock et les prix de mes produits. J'aimerais également gérer les niveaux de stock et les prix de mes produits.**

Ce scénario peut être résolu en accordant au hub l'autorisation d'ajouter à l'inventaire ainsi que l'autorisation d'ajouter au cycle de commande. 

Cela permet au hub de stocker vos produits dans sa boutique, mais de fixer ses propres prix et niveaux de stock. Lorsque vous stockerez vos produits dans votre propre boutique, ils continueront à refléter les prix et les niveaux de stock que vous avez définis.

