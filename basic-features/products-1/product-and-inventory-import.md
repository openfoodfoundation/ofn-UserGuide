---
description: >-
  This page explains how both producers can to import product details and
  distributors can set up their hub inventory in bulk.
---

# Importer des produits



{% hint style="info" %}
Cette fonctionnalité est encore en version béta. Contactez-nous pour toute question !
{% endhint %}

Cet outil vous permet de téléverser un fichier csv pour ajouter en une seule manipulation une liste de produits au catalogue d'un producteur ou dans un catalogue boutique, ou mettre à jour des informations en masse comme les stocks. Cela évite les ajouts ou mise à jour sur chaque produit un par un. Pour un producteur qui met à jour son catalogue dans un tableur type Excel régulièrement, cela peut lui faire gagner beaucoup de temps !

Pour accéder à la fonctionnalité, cliquez sur le menu principal **Produits** puis le sous-menu **import produits**.&#x20;

Les 4 possibilités principales offertes par cette fonctionnalité sont :

1. Importer de nouveaux produits dans des catalogues producteurs
2. Mettre à jour les caractéristiques de produits existants dans des catalogues producteurs
3. Importer des produits dans des catalogues boutiques
4. Mettre à jour les caractéristiques de produits existants dans des catalogues boutiques

Dans chacun des cas, il vous faudra télécharger le modèle de fichier csv sur la plateforme, le remplir et le téléverser ensuite sur la plateforme.

{% hint style="info" %}
**Important** : Microsoft Excel ne permet pas l'ouverture "directe" d'un tableur en csv. Si vous le pouvez, nous vous conseillons d'utiliser les tableurs libres de **LibreOffice** [https://www.libreoffice.org/download/download/](https://www.libreoffice.org/download/download/) Avec Libre Office Calc, vous pourrez ouvrir directement le fichier au format csv et l'enregistrer au bon format d'encodage **UTF-8**. Si vous préférez tout de même utiliser Microsoft Excel, veuillez suivre la procédure suivante pour ouvrir un fichier csv : [https://support.office.com/fr-fr/article/Importer-ou-exporter-des-fichiers-texte-txt-ou-csv-5250ac4c-663c-47ce-937b-339e391393ba](https://support.office.com/fr-fr/article/Importer-ou-exporter-des-fichiers-texte-txt-ou-csv-5250ac4c-663c-47ce-937b-339e391393ba)

**Notre conseil :** Téléchargez Libre Office, enregistrer au format .csv et au format d'encodage UTF 8
{% endhint %}

## Importer de nouveaux produits dans un catalogue producteur <a href="#import-new-products" id="import-new-products"></a>

Tout d'abord, téléchargez le modèle sur la page d'import et ouvrez-le avec Libre Office (ou Excel ou équivalent).

Le modèle indique les colonnes à remplir pour réussir l'import. Consultez les informations ci-dessous pour bien remplir le fichier.

{% hint style="info" %}
**Attention à la casse** :&#x20;

* Il faut utiliser par exemple mL et non ml !&#x20;
* Il ne faut pas d'espace à la suite d'une champ, par exemple pas d'espace après TVA 5.5%
* Le profil producteur doit être crée avant d'importer
{% endhint %}

Par ailleurs, certains champs ne sont pas encore disponibles via l'import produit (les images, les labels...).

| Titre de colonne    | Obligatoire? | Description                                                                                                                                                      | Exemple                                                   |
| ------------------- | ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------- |
| producer            | Oui          | Le nom du producteur des produits que vous souhaitez importer                                                                                                    | La belle ferme                                            |
| sku                 | Non          | La référence produit                                                                                                                                             | AD001265                                                  |
| name                | Oui          | Le nom du produit                                                                                                                                                | Carotte                                                   |
| display name        | Non          | Ce champ s'applique uniquement si vous importez des variantes (voir plus bas). Dans le cas contraire vous pouvez le laisser vide.                                | Carotte rouge                                             |
| category            | Oui          | Les catégories disponibles sont listées sur la page d'import produit. Veuillez indiquer ici la catégorie du produit                                              | Fruits & Légumes                                          |
| units               | Oui          | Le poids, le volume ou la quantité                                                                                                                               | 500                                                       |
| unit\_type          | Non          | Sous quelle unité de mesure est vendu le produit ? (grammes, litres,... ?) S'il est vendu à la pièce, laissez vide                                               | g                                                         |
| variant\_unit\_name | ?            | Si le produit est vendu à la pièce, indiquez le nom de la pièce ici                                                                                              | Botte                                                     |
| price               | Oui          | Le prix du produit TTC                                                                                                                                           | 3.70                                                      |
| on\_hand            | Non          | Si le stock du produit est limité, indiquez la limite ici, sinon laissez vide et renseignez la colonne on\_demand                                                | 40                                                        |
| available\_on       | Non          | Laissez vide                                                                                                                                                     | ​                                                         |
| on\_demand          | Non          | Si vous avez un stock infini du produit, indiquez 1 et si vous utilisez la colonne on\_hand laissez vide                                                         | 1                                                         |
| shipping\_category  | Oui          | Les conditions de transport disponibles sont listées sur la page d'import produit. Veuillez indiquer ici les conditions de transport du produit (réfrigéré, ...) | ​Produits réfrigérés                                      |
| tax\_category       | Non          | Si le prix de votre produit inclus de la TVA, indiquez TVA plus pourcentage sinon laissez vide                                                                   | TVA 5.5%                                                  |
| description         | Non          | Vous pouvez créer une description mais pas la mettre à jour pour l'instant.                                                                                      | Ces carottes sont lavées par nos soins avant la livraison |

### Les variantes

[Les variantes](broken-reference) peuvent être distinguées par les unités (par exemple un produit vendu par 500 g ou 1 kg) ainsi que le champ display\_name (exemple : Yaourt à la myrtille, fraise...). Chaque variante est regroupée sous le même nom produit. Exemple :

| name               | display\_name | price | units | unit\_type |
| ------------------ | ------------- | ----- | ----- | ---------- |
| Farine de sarrasin | ​             | 3.50  | 500   | g          |
| Farine de sarrasin | ​             | 5.50  | 750   | g          |
| Yaourt             | Fraise        | 4     | 200   | g          |
| Yaourt             | Myrtille      | 4     | 200   | g          |

Pour rappel exemple d'affichage pour l'acheteur d'un produit avec 3 variantes :

![](<../../.gitbook/assets/image (57) (1).png>)

### Exemple d'unités <a href="#variants-1" id="variants-1"></a>

Un exemple d'import avec des unités différentes :&#x20;

| producer     | **name**     | **display\_name** | **price** | **units** | **unit\_type** | **variant\_unit\_name** |
| ------------ | ------------ | ----------------- | --------- | --------- | -------------- | ----------------------- |
| Producteur A | Patate douce | Légumineuses      | 3.50      | 500       | g              |                         |
| Producteur B | Bar          | Poisson           | 3.50      | 300       | ml             |                         |
| Producteur C | Pommes       | Fruits & légumes  | 9.50      | 5         | kg             |                         |
| Producteur D | Persil       | Herbes & épices   | 3.00      | 1         |                | botte                   |

### Importer le fichier CSV

Une fois votre fichier csv prêt, vous pouvez le téléverser sur Open Food Network.

Allez sur **Produits** > **Import produit**\
****Sélectionnez **"catalogue produits des producteurs"**\
****Sélectionnez votre fichier\
****Cliquez sur **Téléverser**

Avant que l'import ne se lance, vous verrez un récapitulatif. C'est le moment de vérifier si une erreur ne s'est pas glissée dans votre fichier !

## Mettre à jour les caractéristiques de produits existants dans des catalogues producteurs <a href="#update-existing-product-details" id="update-existing-product-details"></a>

Comment mettre à jour des produits existants ?

Le processus est similaire à la création de produit.  6 champs sont obligatoires pour que l'import fonctionne et seul 5 champs sont modifiables via l'import :

| Champs obligatoires (non modifiables) | Champs modifiables | Champs non modifiables et non obligatoires |
| ------------------------------------- | ------------------ | ------------------------------------------ |
| producer                              | sku                | variant\_unit\_name                        |
| name                                  | price              | tax\_category                              |
| category                              | on\_hand           | shipping\_category                         |
| units                                 | on\_demand         | ​description                               |
| unit\_type (si applicable)            |                    | ​                                          |
| variant\_unit\_name (si applicable)   | ​                  | ​                                          |
| display\_name                         |                    |                                            |

## Importer ou mettre à jour des produits dans des catalogues boutiques <a href="#import-new-inventory" id="import-new-inventory"></a>

Tout d'abord, téléchargez le modèle sur la page d'import et ouvrez-le avec Libre Office (ou Excel ou équivalent).

Le modèle indique les colonnes à remplir pour réussir l'import. Consultez les informations ci-dessous pour bien remplir le fichier.

{% hint style="info" %}
**Attention à la casse** : il faut utiliser par exemple mL et non ml !
{% endhint %}

Par ailleurs, certains champs ne sont pas encore disponibles via l'import produit (les images, les labels...).

| Titre de colonne    | Obligatoire? | Description                                                                                                                       | Exemple        |
| ------------------- | ------------ | --------------------------------------------------------------------------------------------------------------------------------- | -------------- |
| producer            | Oui          | Le nom du producteur des produits que vous souhaitez importer                                                                     | La belle ferme |
| distributor         | Oui          | Le nom du hub qui va vendre le produit                                                                                            | Hub demo       |
| sku                 | Non          | La référence produit                                                                                                              | AD001265       |
| name                | Oui          | Le nom du produit                                                                                                                 | Carotte        |
| display name        | Non          | Ce champ s'applique uniquement si vous importez des variantes (voir plus bas). Dans le cas contraire vous pouvez le laisser vide. | Carotte rouge  |
| category            | Oui          | Les catégories disponibles sont listées sur la page d'import produit. Veuillez indiquer ici la catégorie du produit               | Poisson        |
| units               | Oui          | Le poids, le volume ou la quantité                                                                                                | 500            |
| unit\_type          | Oui          | Sous quelle unité est vendu le produit ? (grammes, litres,... ?) S'il est vendu à la pièce, laissez vide                          | g              |
| variant\_unit\_name | Oui          | Si le produit est vendu à la pièce, indiquez le nom de la pièce ici                                                               | Botte          |
| price               | Oui          | Le prix du produit TTC                                                                                                            | 3.70           |
| on\_hand            | Non          | Si le stock du produit est limité, indiquez la limite ici, sinon laissez vide et renseingez la colonne on\_demand                 | 40             |
| available\_on       | Non          | Laissez vide                                                                                                                      | ​              |
| on\_demand          | Non          | Si vous avez un stock infini du produit, indiquez 1 et si vous utilisez la colonne on\_hand laissez vide                          | 1              |

### Importer le fichier CSV <a href="#import-the-csv" id="import-the-csv"></a>

Une fois votre fichier csv prêt, vous pouvez le téléverser sur Open Food Network.

Allez sur **Produits** > **Import produit**\
****Sélectionnez **"catalogues boutiques des hubs distributeurs"**\
****Sélectionnez votre fichier\
****Cliquez sur **Téléverser**

Avant que l'import ne se lance, vous verrez un récapitulatif. C'est le moment de vérifier si une erreur ne s'est pas glissée dans votre fichier !
