# Importer un tableau de produits



Cet outil vous permet de téléverser un fichier csv pour ajouter en une seule manipulation une liste de produits au catalogue d'un producteur ou dans un catalogue boutique, ou mettre à jour des informations en masse comme les stocks. Cela évite les ajouts ou mise à jour sur chaque produit un par un. Pour un producteur qui met à jour son catalogue dans un tableur type Excel régulièrement, cela peut lui faire gagner beaucoup de temps !

Pour accéder à la fonctionnalité, cliquez sur le menu principal **Produits** puis le sous-menu **import produits**.&#x20;

<figure><img src="../../.gitbook/assets/Import produits cadré.jpg" alt=""><figcaption></figcaption></figure>



Les 4 possibilités principales offertes par cette fonctionnalité sont :

1. Importer de nouveaux [produits](https://guide.openfoodnetwork.org/v/fr/basic-features/products-1) dans les catalogues producteurs
2. Mettre à jour les caractéristiques de produits existants dans les catalogues producteurs
3. Importer des produits dans le [catalogue boutique](https://guide.openfoodnetwork.org/v/fr/basic-features/products-1/inventory-tool?q=catalogue+bout)
4. Mettre à jour les caractéristiques de produits existants dans le catalogue boutique

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

<table data-header-hidden data-full-width="true"><thead><tr><th>Titre de colonne</th><th>Obligatoire?</th><th>Description</th><th>Exemple</th></tr></thead><tbody><tr><td>Titre de colonne</td><td>Obligatoire?</td><td>Description</td><td>Exemple</td></tr><tr><td>producer</td><td>Oui</td><td>Le nom du producteur des produits que vous souhaitez importer</td><td>La belle ferme</td></tr><tr><td>sku</td><td>Non</td><td>La référence produit</td><td>AD001265</td></tr><tr><td>name</td><td>Oui</td><td>Le nom du produit</td><td>Carotte</td></tr><tr><td>display name</td><td>Non</td><td>Ce champ s'applique uniquement si vous importez des variantes (voir plus bas). Dans le cas contraire vous pouvez le laisser vide.</td><td>Carotte rouge</td></tr><tr><td>category</td><td>Oui</td><td>Les catégories disponibles sont listées sur la page d'import produit. Veuillez indiquer ici la catégorie du produit</td><td>Fruits &#x26; Légumes</td></tr><tr><td>units</td><td>Oui</td><td>Le poids, le volume ou la quantité</td><td>500</td></tr><tr><td>unit_type</td><td>Non</td><td>Sous quelle unité de mesure est vendu le produit ? (grammes, litres,... ?) S'il est vendu à la pièce, laissez vide</td><td>g</td></tr><tr><td>variant_unit_name</td><td>?</td><td>Si le produit est vendu à la pièce, indiquez le nom de la pièce ici</td><td>Botte</td></tr><tr><td>price</td><td>Oui</td><td>Le prix du produit TTC</td><td>3.70</td></tr><tr><td>on_hand</td><td>Non</td><td>Si le stock du produit est limité, indiquez la limite ici, sinon laissez vide et renseignez la colonne on_demand</td><td>40</td></tr><tr><td>available_on</td><td>Non</td><td>Laissez vide</td><td>​</td></tr><tr><td>on_demand</td><td>Non</td><td>Si vous avez un stock infini du produit, indiquez 1 et si vous utilisez la colonne on_hand laissez vide</td><td>1</td></tr><tr><td>shipping_category</td><td>Oui</td><td>Les conditions de transport disponibles sont listées sur la page d'import produit. Veuillez indiquer ici les conditions de transport du produit (réfrigéré, ...)</td><td>​Produits réfrigérés</td></tr><tr><td>tax_category</td><td>Non</td><td>Si le prix de votre produit inclus de la TVA, indiquez TVA plus pourcentage sinon laissez vide</td><td>TVA 5,5%</td></tr><tr><td>description</td><td>Non</td><td>Vous pouvez créer une description mais pas la mettre à jour pour l'instant.</td><td>Ces carottes sont lavées par nos soins avant la livraison</td></tr></tbody></table>

### Les variantes

[Les variantes](https://guide.openfoodnetwork.org/v/fr/basic-features/products-1/product-variants) peuvent être distinguées par les unités (par exemple un produit vendu par 500 g ou 1 kg) ainsi que le champ display\_name (exemple : Yaourt à la myrtille, fraise...). Chaque variante est regroupée sous le même nom produit. Exemple :

<table data-header-hidden><thead><tr><th width="150">name</th><th>display_name</th><th>price</th><th>units</th><th>unit_type</th></tr></thead><tbody><tr><td>name</td><td>display_name</td><td>price</td><td>units</td><td>unit_type</td></tr><tr><td>Farine de sarrasin</td><td>​</td><td>3.50</td><td>500</td><td>g</td></tr><tr><td>Farine de sarrasin</td><td>​</td><td>5.50</td><td>750</td><td>g</td></tr><tr><td>Yaourt</td><td>Fraise</td><td>4</td><td>200</td><td>g</td></tr><tr><td>Yaourt</td><td>Myrtille</td><td>4</td><td>200</td><td>g</td></tr></tbody></table>

Pour rappel exemple d'affichage pour l'acheteur d'un produit avec 3 variantes :

![](<../../.gitbook/assets/image (57) (1).png>)

### Exemple d'unités <a href="#variants-1" id="variants-1"></a>

Un exemple d'import avec des unités différentes :&#x20;

<table data-header-hidden><thead><tr><th width="150">producer</th><th>name</th><th>display_name</th><th>price</th><th>units</th><th>unit_type</th><th>variant_unit_name</th></tr></thead><tbody><tr><td>producer</td><td><strong>name</strong></td><td><strong>display_name</strong></td><td><strong>price</strong></td><td><strong>units</strong></td><td><strong>unit_type</strong></td><td><strong>variant_unit_name</strong></td></tr><tr><td>Producteur A</td><td>Patate douce</td><td>Légumineuses</td><td>3.50</td><td>500</td><td>g</td><td></td></tr><tr><td>Producteur B</td><td>Bar</td><td>Poisson</td><td>3.50</td><td>300</td><td>ml</td><td></td></tr><tr><td>Producteur C</td><td>Pommes</td><td>Fruits &#x26; légumes</td><td>9.50</td><td>5</td><td>kg</td><td></td></tr><tr><td>Producteur D</td><td>Persil</td><td>Herbes &#x26; épices</td><td>3.00</td><td>1</td><td></td><td>botte</td></tr></tbody></table>

### Importer le fichier CSV

Une fois votre fichier csv prêt, vous pouvez le téléverser sur Open Food Network.

Allez sur **Produits** > **Import produit**\
Sélectionnez **"catalogue produits des producteurs"**\
Sélectionnez votre fichier\
Cliquez sur **Téléverser**

Avant que l'import ne se lance, vous verrez un récapitulatif. C'est le moment de vérifier si une erreur ne s'est pas glissée dans votre fichier !

## Mettre à jour les caractéristiques de produits existants dans des catalogues producteurs <a href="#update-existing-product-details" id="update-existing-product-details"></a>

Comment mettre à jour des produits existants ?

Le processus est similaire à la création de produit.  6 champs sont obligatoires pour que l'import fonctionne et seul 5 champs sont modifiables via l'import :

<table data-header-hidden><thead><tr><th>Champs obligatoires (non modifiables)</th><th width="278.3333333333333">Champs modifiables</th><th>Champs non modifiables et non obligatoires</th></tr></thead><tbody><tr><td>Champs obligatoires (non modifiables)</td><td>Champs modifiables</td><td>Champs non modifiables et non obligatoires</td></tr><tr><td>producer</td><td>sku</td><td>variant_unit_name</td></tr><tr><td>name</td><td>price</td><td>tax_category</td></tr><tr><td>category</td><td>on_hand</td><td>shipping_category</td></tr><tr><td>units</td><td>on_demand</td><td>​description</td></tr><tr><td>unit_type (si applicable)</td><td></td><td>​</td></tr><tr><td>variant_unit_name (si applicable)</td><td>​</td><td>​</td></tr><tr><td>display_name</td><td></td><td></td></tr></tbody></table>

## Importer ou mettre à jour des produits dans le [catalogue boutiques](https://guide.openfoodnetwork.org/v/fr/basic-features/products-1/inventory-tool) <a href="#import-new-inventory" id="import-new-inventory"></a>

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
Sélectionnez **"catalogues boutiques des hubs distributeurs"**\
Sélectionnez votre fichier\
Cliquez sur **Téléverser**

Avant que l'import ne se lance, vous verrez un récapitulatif. C'est le moment de vérifier si une erreur ne s'est pas glissée dans votre fichier !
