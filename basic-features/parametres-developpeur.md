# Paramètres développeur

Sur demande, votre instance peut vous activer l'accès à un onglet "Paramètres développeur", qui vous permet de :&#x20;

:thumbsup: **accéder à votre clé API**&#x20;

:thumbsup: **configurer des "webhook"**

Après activation, cet onglet apparaît dans votre compte utilisateur :

<figure><img src="../.gitbook/assets/Screen Shot 2023-03-29 at 23.59.20.png" alt=""><figcaption></figcaption></figure>

## La clé API

Elle vous permet de faire des intégrations avec d'autres logiciels. Par exemple, votre instance peut vous proposer d'importer automatiquement votre liste d'acheteurs dans un outil de newsletter, tel que Sendinblue ou MailChimp. Dans ce cas, le logiciel de newsletter aura besoin de votre clé API CoopCircuits.

## Les webhooks

Un _webhook_ c'est une fonction qui envoie un message d'un logiciel à un autre lors d'un évènement spécifique. Elle permet ainsi de faire le lien entre plusieurs logiciels. Lorsque l'événement concerné se produit, un message est envoyé avec une charge utile contenant des données sur l'événement.

Le message est envoyé sous forme de requête HTTP à une adresse URL (ou point de terminaison). C'est l'adresse de l'autre logiciel, qui de son côté déclenchera une action spécifique en recevant le message.&#x20;

{% hint style="info" %}
Un exemple concret : pour les utilisateurs qui disposent de l'intégration avec un outil de newsletter, cela permettra de déclencher automatiquement l'envoi de la newsletter à chaque début de cycle de vente ! Le webhook pour la fin du cycle de vente arrive bientôt ;)
{% endhint %}

### Configuration du webhook

Allez dans votre compte, dans l'onglet "Paramètres développeur", sous la section "Webhook"&#x20;

<figure><img src="../.gitbook/assets/Screen Shot 2023-03-30 at 00.17.24.png" alt=""><figcaption></figcaption></figure>

Au niveau de l'événement pour lequel vous souhaitez créer un webhook, entrez l'URL de point de terminaison unique fournie par l'autre logiciel. Cliquez sur créer.&#x20;

Désormais, chaque fois que l'événement se produit, l'autre système recevra une requête avec une charge utile contenant les informations pertinentes.
