# Permissions inter-entreprises

Ces permissions doivent être octroyées pour qu'une entreprise deviennent fournisseur d'une autre ou inversement qu'une entreprise puisse distribuer les produits d'une autre. Un "droit" est accordé par une entreprise à une autre concernant l'accès / la modification des produits et du profil.

![](<../../.gitbook/assets/image (61) (1) (1) (1).png>)



Ensuite deux paragraphes vont plus loin en présentant les permissions depuis deux points de vue différents :

* ****[**Celui du hub**](https://ofn-user-guide.gitbook.io/guide-utilisateur-open-food-network/fonctionnalites-standards/votre-profil/e2e-permissions#point-de-vue-dun-hub)****
* **Celui du producteur**

## Les différentes permissions

Il existe 4 différentes permissions. Elles peuvent se combiner de différentes manières afin de donner aux entreprises plus ou moins de droits suivant leurs profils.&#x20;

![](<../../.gitbook/assets/image (40) (1) (1) (1).png>)

* **Permission de vendre les produits (= ajouter au cycle de vente) :** le fournisseur autorise le hub à ajouter ses produits à ses cycles de vente, donc à la vendre.
* **Permission d'ajouter les produits au catalogue boutique :** le fournisseur autorise le hub à ajouter ses produits au catalogue boutique du hub. Le hub pourra alors modifier les prix et stock des produits _uniquement pour sa boutique à lui_, cela n'affectera pas le catalogue du fournisseur.
* **Permission de modifier les produits :** le fournisseur autorise une entreprise (hub ou producteur) à créer, supprimer et modifier ses produits directement dans son catalogue fournisseur. Cela peut potentiellement impacter toutes les entreprises ayant accès au catalogue fournisseur car toute modification du catalogue du fournisseur se répercutera sur les distributions qui en sont faites.
* **Permission de modifier le profil :** une entreprise permet à une autre de modifier les détails de son profil (coordonnées, adresse, description, ...)

## Donner et gérer les permissions

Pour modifier, ajouter ou supprimer des permissions, rendez-vous sur l'interface d'administration puis dans le menu **Entreprises**, puis sous-menu **Permissions** (voir capture ci-dessous). Si vous avez besoin qu'une autre entreprise vous donne des permissions, vous devez les contacter par email ou téléphone. Il n'y a pas de fonctionnalité en ligne pour contacter une autre entreprise à ce sujet.

{% hint style="info" %}
**Attention** : vous ne pouvez pas gérer les permissions de votre entreprise si vous n'êtes pas gestionnaire de l'entreprise.
{% endhint %}

Pour accorder une permission, dans la première colonne, sélectionnez votre entreprise et dans la seconde l'entreprise à qui vous donnez des droits. Cliquez ensuite sur le type de permissions que vous souhaitez accorder. Vous pouvez sélectionner plusieurs permissions ou les sélectionner toutes en cliquant sur "TOUT". Puis cliquez sur "Créer". Notez que vous pouvez supprimer ou modifier ces permissions à tout moment.

![](<../../.gitbook/assets/image (49) (1) (1).png>)

## Les permissions gérées automatiquement

Lorsqu'un utilisateur est gestionnaire principal de plusieurs entreprises sur la plateforme, les 4v permissions sont créées automatiquement entre chaque entreprise. Ce n'est pas le cas entre des entreprises administrées par des utilisateurs différents.

## Pour les Hubs

Ces situations courantes illustrent quelles autorisations d'entreprise vous devrez configurer pour votre hub.

> **J'ai créé des profils de producteur pour chacun de mes fournisseurs. Quelles autorisations dois-je configurer avant de pouvoir stocker leurs produits sur la vitrine de mon Hub ?**

Le système est configuré de manière à ce que les hubs qui créent des profils de producteurs aient _les autorisations correctes installées par défaut_, afin qu'ils puissent commencer à ajouter des produits et à échanger avec ces profils de producteurs immédiatement.

> **Mon fournisseur a déjà une entreprise enregistrée auprès de l'OFN. Je voudrais ajouter leurs produits à la vitrine de mon hub.**

Vous devez contacter votre fournisseur en personne. Ses coordonnées (numéro de téléphone, adresse et adresse électronique) se trouvent dans son profil OFN.

Si vous avez uniquement l'intention de _**stocker leurs produits**_ et ne souhaitez pas les aider à gérer le reste de leur profil OFN, demandez au producteur de vous accorder la permission d'_**ajouter au cycle de commande**_ et la permission d'_**ajouter à l'inventaire**_.&#x20;

Si le fournisseur souhaite que vous, en tant que gestionnaire de Hub, l'aidiez à organiser son entreprise OFN, il peut vous accorder les quatre permissions. Dans ce cas, vous serez en mesure de modifier son profil et de gérer ses produits.

> **Mon Hub distribue par le biais de groupes d'achat. De quelles autorisations le groupe d'achat aura-t-il besoin avec mon hub et mes producteurs ?**

{% hint style="warning" %}
Ceci est un cas où le centre qui gère (coordonne) un cycle de commande diffère de l'entreprise auprès de laquelle les clients collectent leurs achats.&#x20;

_Si le centre A gère (coordonne) un cycle de commande pour un groupe d'acheteurs (centre B), alors le cycle de commande sera affiché sur la vitrine OFN du centre B._
{% endhint %}

Le groupe d'achat (Hub B ci-dessus) devra accorder au coordinateur du cycle de commande (Hub A ci-dessus) l'autorisation d'ajouter au cycle de commande (et de préférence l'autorisation d'ajouter à l'inventaire).

Les producteurs qui fournissent au hub A des produits qui seront également vendus par le groupe d'achat (hub B) doivent accorder aux deux hub A et B l'autorisation d'ajouter au cycle de commande (et de préférence l'autorisation d'ajouter à l'inventaire).

## Pour les Producteurs

Lorsqu'un producteur souhaite commencer à vendre ses produits par l'intermédiaire d'autres entreprises (hubs ou groupes d'achat), il doit établir les autorisations appropriées d'entreprise à entreprise. Il existe différents niveaux d'autorisation qu'un producteur peut accorder, en fonction du pouvoir qu'il souhaite donner au hub pour gérer ses produits et son profil (voir le haut de page).&#x20;

Ces exemples explorent quelques scénarios courants.

> **Je suis un producteur et j'aimerais qu'un hub OFN local stocke et vende mes produits.**

**Essentiel** : Pour que le hub puisse ajouter vos produits à sa vitrine, vous devez lui accorder la "permission d'ajouter au cycle de commande".&#x20;

**Facultatif** : vous pouvez également donner au hub l'autorisation de gérer vos produits, de modifier votre profil ou d'ajouter à l'inventaire.

> **Un hub que je fournis distribue par le biais de groupes d'achat.**

Pour que vos produits puissent être distribués par les groupes d'achat, vous devez ajouter au minimum l'autorisation "d'ajouter au cycle de commande" pour l'entreprise du groupe d'achat ainsi que pour le hub que vous fournissez directement.

> **Je suis une boutique de producteurs qui approvisionne un Hub local tout en gérant ma propre vitrine. Le hub aimerait gérer les niveaux de stock et les prix de mes produits. J'aimerais également gérer les niveaux de stock et les prix de mes produits.**

Ce scénario peut être résolu en accordant au hub l'autorisation d'ajouter à l'inventaire ainsi que l'autorisation d'ajouter au cycle de commande.&#x20;

Cela permet au hub de stocker vos produits dans sa boutique, mais de fixer ses propres prix et niveaux de stock. Lorsque vous stockerez vos produits dans votre propre boutique, ils continueront à refléter les prix et les niveaux de stock que vous avez définis.
