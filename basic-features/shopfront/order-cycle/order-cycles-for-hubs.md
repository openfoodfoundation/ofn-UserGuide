# Cycle de vente géré par un hub

_\*Vous êtes un producteur  et avez choisi un type de profil "Boutique producteur" ? Rendez-vous sur_ [_Cycle de vente pour les fournisseurs_](broken-reference)_._

En créant un cycle de vente, vous définissez les périodes d'ouverture de votre boutique, les produits pouvant être achetés ainsi que les marges et commissions ajoutées sur les prix de base des produits pour couvrir les frais liés à la distribution.

**Pourquoi gérer par cycle de vente ?** Certaines entreprises préfèrent avoir une ouverture en continu et répondre à chaque commande au fil de l'eau. D'autres fonctionnent par périodes de commande correspondant à un jour de livraison donné. Par exemple, les ventes seront ouvertes pendant deux semaines (un cycle de vente de deux semaines) : à la fin de ces deux semaines, toutes les commandes seront emballées et livrées en même temps le mercredi suivant. Une fois que ce lot de commandes a été livré, un nouveau cycle de vente redémarre. Cela permet d'optimiser la préparation des commande et le transport, réduisant aussi les frais associés grâce à une logique de massification.

## Créer un nouveau cycle de vente

Connecté en administrateur, rendez-vous sur le menu Cycle de vente ou depuis votre tableau de bord, cliquer sur le bouton suivant :&#x20;

![](<../../../.gitbook/assets/image (78).png>)

Puis cliquez sur "Nouveau cycle de vente" :&#x20;

![](<../../../.gitbook/assets/image (91).png>)

{% hint style="info" %}
**Attention !** Vos cycles de vente seront inactifs tant que vous n'aurez pas créé au moins une [méthode de livraison ](broken-reference)et une[ méthode de paiement](broken-reference)
{% endhint %}

La première chose à faire est de sélectionner un coordinateur pour votre cycle de vente. Cette entreprise aura toutes les permissions pour modifier et gérer le cycle de vente. Les autres entreprises impliquées dans le cycle de vente (les fournisseurs ou les autres hubs) auront des accès restreints. Pour plus d'informations sur les gestions des droits entre entreprises dans le contexte des cycles de vente, cliquez [ici](broken-reference).

Une fois le coordinateur choisi vous êtes redirigé vers un écran en 3 étapes :

### 1. Informations générales

![](<../../../.gitbook/assets/image (56).png>)

**Nom :** Choisissez un nom pour le cycle de vente. Il sera visible uniquement de vous, donc indiquez quelque chose qui vous permettra de le retrouver facilement ensuite. Par exemple vous pouvez choisir une dénomination type _Semaine26\_2018._

**Commandes à partir de :** La date à laquelle votre boutique commencera à accepter des commandes pour ce cycle de vente.

**Commandes jusqu'au :** La date à laquelle votre boutique arrêtera d'accepter des commandes pour ce cycle de vente. Si vous souhaitez laisser votre boutique ouverte en continue, indiquer une date dans un futur très lointain.

**Ajouter commission coordinateur :** Si vous souhaitez appliquer une marge ou commission sur tous les produits et tous les distributeurs figurant dans ce cycle de vente, vous pouvez choisir ici la marge souhaitée parmi les marges et commission prédéfinies (voir page [Marges et commissions](broken-reference)).

### 2. Produits entrants

Cette section vous permet de sélectionner les produits qui seront vendus durant le cycle de vente, parmi les produits proposés par les producteurs. Les producteurs visibles dans la liste déroulante sont uniquement les producteurs vous [ayant autorisé à vendre leurs produits](broken-reference). Cliquez bien sur "ajouter un fournisseur" pour voir les produits associés à ce fournisseur. Cochez les produits que vous souhaitez ajouter (vous pouvez aussi les sélectionner tous).&#x20;

{% hint style="info" %}
**Attention** : les produits qui sont en rupture de stock s'afficheront également dans la liste. Faites bien attention au stock disponible en les ajoutant.
{% endhint %}

Les **détails de livraison produits** sont facultatifs, et sont affichés dans l'email automatiquement envoyé aux producteurs à la fin du cycle de vente. Il s'agit donc de précisions que le hub adresse au producteur concernant les conditions de livraison.

Le bouton marge et commission dans cette section, au niveau de chaque ligne producteurs, vous permet d'appliquer une marge différenciée selon le producteur. Par exemple, le producteur de farine achemine ses produits d'assez loin et les coûts de transport sont particulièrement élevés sur ces produits. Le hub souhaite refléter ce coût de manière transparente sur les produits de ce producteur : il va pouvoir ajouter une marge spécifique pour ce producteur, qui s’additionnera aux autres marges figurant au niveau du coordinateur ou des distributeurs (produits sortants). Sélectionnez le nom de l'entreprise, puis le nom de la marge comme dans l'exemple ci-dessous :

Cette marge s'appliquera à tous les produits du fournisseur. La marge sera calculée en fonction du calculateur sélectionné au moment de sa création (voir page [marges et commissions](broken-reference)).

### 3. Produits vendus (sortants)

Vous pouvez ici sélectionner un ou plusieurs hubs-distributeurs, pour lesquels donc leurs boutiques respectives seront ouvertes à la commande pour ce cycle de vente. Dans un modèle simple, il n'y a qu'un seul hub--distributeur. Il suffit de le sélectionner puis de sélectionner tous les produits associés. Dans un modèle plus complexe avec plusieurs hubs-distributeurs dans la partie produits sortants, vous avez ainsi la possibilité de sélectionner des produits différents pour chaque hub et de paramétrer des dates de livraison différentes.

![](<../../../.gitbook/assets/image (50).png>)

Les **tags** vous permettent de taguer le cycle de vente pour qu'il ne soit visible que de certains acheteurs (voir page [Affichages relatifs aux catégories d'acheteurs (tags)](broken-reference)).

**Prêt pour :** La date à laquelle cette commande sera disponible (ou livrée) pour les acheteurs. Vous pouvez indiquer ici un texte libre qui sera utilisé pour nommer ce cycle de vente, par exemple _Vendredi prochain_. Certains hubs "hackent" un peu ce fonctionnement et saisissent ici la nature de la commande concernée par ce cycle de vente, par exemple (Commande viande pour 23 juillet).

**Modalités de retrait/livraison :** Les indications précisées ici seront incluses dans l'email de confirmation de commande envoyé au client, juste en-dessous de la méthode de livraison. Ils seront les seuls à obtenir cette information donc vous pouvez y inclure des informations comme des adresses ou numéros de téléphone.

**Ajouter une commission** **:** A nouveau une marge ou commission peut être spécifiée. Elle s'appliquera sur tous les produits proposés à la vente par ce distributeur.

### 4. Ouvrir la boutique

Cliquez sur "créer" pour créer le cycle de vente. Si la date d'ouverture est déjà passée, votre boutique est instantanément ouverte ! Si vous n'êtes pas prêt à ouvrir tout de suite, indiquez des dates dans le passé ou le futur, que vous pourrez changer ensuite.

Si votre cycle de vente se répète de manière périodique et régulière, vous pouvez dupliquer un cycle de vente passé afin d'aller plus vite (bouton orange sur la capture, attention il n'est pas orange sur la plateforme) :

![](<../../../.gitbook/assets/image (37).png>)

Les cycles de vente sont présentés en vert lorsqu'ils sont actifs, jaune lorsqu'ils sont en attente d'ouverture (date de début pas encore passée) et gris lorsqu'ils sont fermés. Un mois après sa fermeture le cycle de vente n’apparaîtra plus dans cette liste, il faudra cliquer sur "voir plus" pour voir tous vos cycles de vente.

## Notifier les producteurs

Depuis un cycle de vente, il vous est possible de notifier à tout moment les producteurs des commandes en cours. \
Cliquez sur le bouton "modifier" du cycle de vente de votre choix depuis la liste des cycles de vente puis sélectionnez "Notifier les producteurs"

![](<../../../.gitbook/assets/image (93).png>)

En utilisant ce bouton, tous les producteurs liés à ce cycle de vente recevront un email contenant une liste des produits commandés pour ce cycle de vente avec les instructions éventuelles de livraison si elles ont été renseignées dans le cycle de vente (produits entrants).
