---
description: >-
  This page explains how both producers can to import product details and
  distributors can set up their hub inventory in bulk.
---

# Importer des Produits dans l'Inventaire

L'outil d'importation de produits et de stocks vous permet de télécharger un fichier .csv pour ajouter et mettre à jour votre stock. Cela peut être beaucoup plus rapide et efficace que d'ajouter ou de mettre à jour les produits un par un. 

Pour les producteurs qui mettent déjà régulièrement à jour un catalogue de leurs produits dans une feuille de calcul Excel, cela peut faire gagner beaucoup de temps ! Vous trouverez l'**outil d'importation de produits et de stocks** en cliquant sur **Produits** dans le menu bleu horizontal, et sur Importation de produits dans le menu vert. 

Vous pouvez utiliser l'outil de quatre manières :

1. Importer de nouveaux produits 
2. Mettre à jour les détails des produits existants 
3. Importer des produits dans un nouvel inventaire de magasin ou de hub 
4. Mettre à jour les produits d'un inventaire de boutique ou de hub

{% hint style="info" %}
Si vous avez besoin de cette fonctionnalité, veuillez en informer votre OFN local. Vos commentaires sont les bienvenus.
{% endhint %}

Dans tous les cas, le processus consiste à télécharger un modèle csv, à remplir les champs et à télécharger à nouveau votre fichier csv dans OFN.

{% hint style="warning" %}
**Remarque importante sur les fichiers CSV** : Microsoft Excel n'ouvre pas directement les fichiers .csv. Si vous le pouvez, nous vous suggérons de télécharger la version gratuite de Libre Office [https://www.libreoffice.org/download/download/](https://www.libreoffice.org/download/download/). Avec Libre Office Calc, vous pourrez ouvrir et éditer des CSV très facilement et les enregistrer dans le bon format d'encodage UTF-8. 

Si vous ne pouvez pas utiliser Libre Office, alors pour ouvrir un fichier CSV dans Microsoft Excel, vous devez suivre les étapes suivantes : [https://support.office.com/en-gb/article/import-or-export-text-txt-or-csv-files-5250ac4c-663c-47ce-937b-339e391393ba](https://support.office.com/en-gb/article/import-or-export-text-txt-or-csv-files-5250ac4c-663c-47ce-937b-339e391393ba)  
{% endhint %}

{% hint style="danger" %}
Tous les champs ne peuvent pas être capturés et téléchargés/mises à jour à l'aide de cet outil. Actuellement, les images, les propriétés et les paramètres d'achat groupé doivent être téléchargés manuellement pour chaque produit.

Nous espérons les inclure dans les développements futurs.
{% endhint %}

## Importer de Nouveaux Produits

Utilisez ces instructions si vous souhaitez ajouter de nouveaux produits au profil d'un producteur.

{% hint style="success" %}
Vous pouvez simultanément télécharger de nouveaux produits et mettre à jour des produits existants avec un seul téléchargement CSV. Les instructions de ce guide sont séparées pour plus de clarté, mais vous pouvez combiner les nouveaux produits et les mises à jour dans la même feuille de calcul.
{% endhint %}

### Préparer le fichier CSV à être importé

Tout d'abord, téléchargez le **fichier CSV modèle de liste de produits** depuis la page d'**importation de produits** et ouvrez-le avec Libre Office \(Excel ou équivalent\). 

Vous verrez que le modèle donne tous les intitulés de colonne nécessaires pour réussir l'importation d'un produit. Chaque ligne correspond à un nouveau produit ou à une nouvelle variante. Vous trouverez ci-dessous une description de la manière de remplir chaque colonne.

{% hint style="danger" %}
Notez que tous les champs sont sensibles à la casse. Par exemple, vous devez utiliser mL et non ml, ou Légumes et non légumes.
{% endhint %}

| Colonne | Requis? | Description | Exemple |
| :--- | :--- | :--- | :--- |
| producteur | Oui | Le nom du profil du producteur auquel ce produit sera attribué. | Ferme de la Montagne |
| N° de produit | Non | Le numéro associé à ce produit. | AD001265 |
| nom | Oui | Le nom du produit. | Yaourt |
| nom d'affichage | Non | Ce champ s'applique si vous créez des variantes \(voir les instructions ci-dessous\). Si vous ne créez pas de variante, laissez ce champ vide. | Yaourt aux Framboises |
| catégorie | Oui | Dans quelle catégorie se trouve ce produit ? Les catégories disponibles sont énumérées sur la page d'importation des produits. | Produits Laitiers |
| unités | Oui | la valeur du poids / la quantité / le nombre d'unité. | 500 |
| type d'unité | Peut-être | Dans quelle unité le produit est-il vendu? | g |
| unité de variante | Peut-être | Si le produit se vend par article, indiquez le nom de l'article ici. | Pot |
| prix | Oui | Le prix du produit. Si le produit est soumis à des taxes, indiquez le prix incluant celles-ci. | 3.70 |
| niveau de stock | Peut-être | Si votre stock pour ce produit est limité, indiquez celu-ci ici. Sinon, utilisez le champs " illimité ". | 40 |
| en stock | Non | Laissez ce champs libre |  |
| illimité | Oui | Si vous avez du stock illimité pour ce produit, indiquez 1. | 1 |
| catégorie d'expédition | Oui | Dans quelle catégorie d'expédition se trouve ce produit ? Les catégories d'expédition disponibles sont répertoriées sur la page Importation de produit. |  |
| catégorie de taxe | Non | Si le prix de votre produit inclut la taxe, tapez GST, sinon laissez le champ vide. | GST |
| description | Non | Vous pouvez créer une description, mais vous ne pouvez pas la mettre à jour. Veuillez vous assurer que le texte que vous avez écrit correspond à la description actuelle en cas de mise à jour. | Ce yaourt contient des framboises de la région |

#### Importer des Variantes de Produits

Dans le processus d'importation, les variantes se distinguent par les unités \(comme la salade vendue en sacs de 500 g et 750 g\) ou le champ nom \(comme un yaourt vendu en plusieurs saveurs\). Tant que le nom du produit est le même, les lignes seront importées en tant que variantes. L'exemple ci-dessous montre une salade qui existe en variantes de 500 g et 750 g, et un yaourt qui existe en plusieurs saveurs.

| nom | nom d'affichage | prix | unités | type d'unité |
| :--- | :--- | :--- | :--- | :--- |
| Framboises |  | 3.60 | 200 | g |
| Framboises |  | 4.80 | 300 | g |
| Pommes | Golden Delicious | 3.60 | 500 | g |
| Pommes | Pink Lady | 4.80 | 500 | g |

L'image ci-dessous montre comment ces produits seront affichés dans la boutique. Notez que le champ "name" devient le titre principal et que le champ "nom d'affichage" devient le titre secondaire.

![](../../.gitbook/assets/samedisplayname%20%281%29.jpg)

![](../../.gitbook/assets/differentdisplaynames.jpg)

#### Exemples de types d'unité

Vous trouverez ci-dessous quelques exemples montrant comment présenter des produits avec différentes unités \(g, ml, kg et articles\).

| producteur | **nom** | **catégorie** | **prix** | **unités** | type d'unité | **nom de variante** |
| :--- | :--- | :--- | :--- | :--- | :---: | :---: |
| Les salades de Suzanne | Salade | Légumes | 3.50 | 500 | g |  |
| Le Verger d'Henri | Jus de fruits | Boissons | 3.50 | 300 | ml |  |
| Bélanger Primeurs | Pommes de terre | Légumes | 9.50 | 5 | kg |  |
| la Boulangerie de Tom | Pain complet | Boulangerie | 3.00 | 1 |  | miche |

### Importer le fichier CSV

Une fois que vous avez rempli le modèle de **liste de produits CSV**, vous êtes prêt à le télécharger dans OFN.

1. Allez dans **Produits** &gt; **Importation de produits**. 
2. Sélectionnez le type d'importation : Sélectionnez **Liste de produits** 
3. Sélectionnez une feuille de calcul à télécharger : Trouvez le fichier csv que vous souhaitez télécharger. Comme vous téléchargez de nouveaux produits, vous pouvez ne pas cocher la case "Remettre le stock à zéro pour tous les produits existants non présents dans le fichier". 
4. Cliquez sur **Télécharger**.

Vous verrez un résumé de votre téléchargement, y compris les éventuelles erreurs. Vous serez également informé du nombre de produits que vous créez et de ceux que vous mettez à jour. Si vous êtes satisfait des résultats du téléchargement, cliquez sur **Enregistrer**.

{% hint style="success" %}
C'est une bonne habitude de vérifier que les produits ont été téléchargés/mises à jour comme vous le souhaitiez.
{% endhint %}

Vous pouvez ensuite télécharger une autre feuille de calcul ou aller à la page des produits pour voir vos nouveaux produits.

## Mettre à jour les Détails d'un Produit Existant

Les instructions ci-dessous concernent la mise à jour des détails d'un produit existant. Cet outil est conçu comme un moyen rapide de mettre à jour les prix et les niveaux de stock des produits.

{% hint style="info" %}
Vous pouvez simultanément télécharger de nouveaux produits et mettre à jour des produits existants avec un seul téléchargement CSV. Les instructions de ce guide sont séparées pour plus de clarté, mais vous pouvez combiner les nouveaux produits et les mises à jour dans la même feuille de calcul.
{% endhint %}

### Préparer le fichier CSV à être importé

Le processus de mise à jour des détails d'un produit est similaire à celui du téléchargement de nouveaux produits. La première étape consiste à télécharger le **modèle de liste de produits** et à remplir les noms des produits et des fournisseurs. Si vous disposez de cette feuille de calcul provenant d'un précédent téléchargement, c'est encore mieux. 

Le système requiert sept champs pour identifier correctement le produit que vous souhaitez mettre à jour. Quatre champs peuvent être mis à jour et quatre ne le peuvent pas à l'aide de cet outil.

| Champs requis \(non modifiables\) | Champs modifiables | Champs non requis et non modifiables |
| :--- | :--- | :--- |
| \*producteur | N° de produit | ^nom d'unité des variantes |
| \*nom | prix | ^catégorie de taxe |
| ^catégorie | en stock | ^catégorie d'expédition |
| \*unités | illimité | ^description |
| ^type d'unité \(si applicable\) |  |  |
| ^nom d'unité de variantes \(si applicable\) |  |  |
| \*nom d'affichage |  |  |

_^ si vous essayez de mettre à jour ces champs, vous verrez un message d'erreur_

_\*Si vous essayez de mettre à jour ces champs, vous allez créer de nouveaux produits ou de nouvelles variantes, plutôt que de mettre à jour un produit existant._

Une fois terminé, le fichier .csv peut être importé de la même manière que pour les nouveaux produits.

{% hint style="info" %}
**Mettre le stock à zéro pour tous les produits existants non présents dans le fichier** : Si vous cochez cette case, le système mettra la valeur "En stock" à zéro pour tous les produits déjà dans votre liste de produits. Si un produit était "illimité", il restera "illimité". Les produits de cette importation conserveront le niveau de stock défini dans le fichier .csv.
{% endhint %}

## Importer ou Mettre à Jour les Produits de votre Inventaire

Voici les instructions pour ajouter ou mettre à jour des produits dans 

### Préparer le fichier CSV à être importé

Tout d'abord, téléchargez le **modèle d'inventaire en fichier CSV** à partir de la page d'**importation de produits**. 

Vous verrez que le modèle donne tous les en-têtes de colonne nécessaires pour réussir à importer un produit. Chaque ligne correspond à un nouveau produit ou à une nouvelle variante. Vous trouverez ci-dessous une description de la manière de remplir chaque colonne.

{% hint style="danger" %}
Notez que tous les champs sont sensibles à la casse. Par exemple, vous devez utiliser mL et non ml, ou Légumes et non légumes.
{% endhint %}

| Colonne | Requis? | Description | Exemple |
| :--- | :--- | :--- | :--- |
| producteur | Oui | Le nom du profil du producteur auquel sera attribué ce produit. | Ferme du Moulin |
| distributeur | Oui | Le nom du hub auquel ce produit est assigné. | Compagnie Exemple |
| nom | Oui | Le nom du produit. | Yaourt |
| nom d'affichage | Non | Ce champs est util pour distinguer les variantes. Si le produit n'a pas de variantes, laissez ce champs libre. | Yaourt aux Framboises |
| nom d'unité de variante | Oui | Si le produit se vend en tant qu'article défini, indiquez le ici. | grappe |
| unités | Oui | Le poids, le volume, la quantité. | 500 |
| type d'unité | Oui | Dans quelle unité le produit est-il vendu? Si le produit se vend en tant qu'article défini, laissez ce champs libre. | g |
| prix | Oui | Le prix du produit. Si le produit est soumis à des taxes, indiquez le prix incluant celles-ci. | 3.70 |
| en stock | Oui | Si vous avez du stock limité, indiquez 1 s'il vous reste du stock et 0 s'il ne vous en reste pas. |  |
| illimité | Oui | Si vous avez du stock illimité pour ce produit, indiquez 1 et laissez le champs " en stock " libre. | 1 |
| N° de produit | Non | Le numéro associé à ce produit. | AD001265 |

### Importer le fichier CSV <a id="import-the-csv"></a>

Une fois complété, vous pouvez importer le **fichier CSV d'inventaire** à la plateforme OFN.

1. Allez dans **Produits** &gt; **Importation de produits**. 
2. Sélectionnez le **type d'importation** : Sélectionnez Inventaires 
3. Sélectionnez une **feuille de calcul à télécharger** 
4. Cliquez sur **Télécharger**.

Vous verrez un résumé de votre téléchargement, y compris les éventuelles erreurs. Vous serez également informé du nombre de produits que vous créez et de ceux que vous mettez à jour. Si vous êtes satisfait des résultats du téléchargement, cliquez sur **Enregistrer**.

{% hint style="success" %}
C'est une bonne habitude de vérifier que les produits ont été téléchargés / mis à jour comme vous l'aviez prévu.
{% endhint %}

