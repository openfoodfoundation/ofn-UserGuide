# Boutique vitrine sans possibilité d’achat

Il arrive qu'un gestionnaire de boutique souhaite afficher les produits qu'il vend sur une logique de "vitrine", pour faire savoir ce qu'il propose à la vente, mais sans autoriser les achats. Par exemple, pour montrer les produits qui seront bientôt en vente dans le prochain cycle de vente.

Pour paramétrer votre boutique en mode "vitrine sans achat possible", il faut ouvrir un [cycle de vente](https://guide.openfoodnetwork.org/v/fr/basic-features/shopfront/order-cycle) incluant les produits que vous souhaitez afficher, et pour la période souhaitée. Puis allez dans **Entreprises > Gérer > Méthode de paiements** et basculer toutes les méthodes de paiement en "visible pour l'administration uniquement", comme dans l'image ci-dessous.&#x20;

{% hint style="danger" %}
Si vous utilisez la même méthode de paiement pour plusieurs boutiques, ce paramètre s'appliquera pour toutes les boutiques. Il vaut mieux dans ce cas créer une nouvelle méthode de paiement en mode "visible pour l'administration uniquement", qui ne s'appliquera qu'à votre boutique vitrine.
{% endhint %}



<figure><img src="../../.gitbook/assets/Screen Shot 2022-09-21 at 14.42.50.png" alt=""><figcaption></figcaption></figure>

Et le tour est joué ! Vos produits s'affichent sur votre boutique, mais la boutique est bien affichée comme fermée à la commande. Exemple ci-dessous :&#x20;

<figure><img src="../../.gitbook/assets/Screen Shot 2022-09-21 at 14.45.05.png" alt=""><figcaption></figcaption></figure>
