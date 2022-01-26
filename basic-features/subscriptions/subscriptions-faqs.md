# FAQ commandes récurrentes

### **Si je supprime l'association d'un rythme d'abonnement à un cycle de vente déjà ouvert, que se passe-t-il pour les commandes automatiques déjà lancées à l'ouverture du cycle ? Sont-elles supprimées ?** &#x20;

Les commandes resteront ouvertes et seront traitées de façon normale, donc à la fermeture du cycle de vente, l'acheteur recevra une confirmation que la commande a bien été passée. Si vous souhaitez supprimer toutes les commandes automatiques associées au cycle de vente en question, vous devrez [annuler chaque commande individuellement](broken-reference).&#x20;

### **Si j'ajoute une commande récurrente associée à un rythme d'abonnement correspondant à un cycle de vente en cours, est-ce qu'une commande sera automatiquement passée pour l'acheteur pour le cycle de vente en cours ?**&#x20;

Oui ! Le cas échéant une commande va être passée automatiquement dans les minutes qui suivront la création de la commande récurrente. Si vous ne souhaitez pas que la commande récurrente démarre dès le cycle de vente en cours, pensez à mettre une date de début pour la commande récurrente postérieure à la fermeture du cycle de vente.&#x20;

### **Que se passe-t-il si le stock d'un produit donné permet de répondre à certaines commandes récurrentes, mais pas à toutes ? Quels acheteurs se verront attribuer le stock disponible ?**&#x20;

Dans ce cas, le stock ne sera pas répartis entre tous les acheteurs avec commandes automatiques pour ce produit, mais sera alloué à chaque commande automatique une par une jusqu'à ce que le stock s'épuise, et les commandes automatiques suivantes apparaîtront comme non complètement satisfaites (le produit sera manquant).&#x20;

### **Que se passe-t-il si je modifie le paramétrage d'une commande récurrente alors qu'une commande automatique a déjà été déclenchée sur un cycle de vente en cours ?**

ASi vous modifiez le paramétrage de la commande récurrente alors qu'un cycle de vente sur le rythme d'abonnement correspondant est ouvert, la commande automatique déjà passée pour ce cycle de vente sera modifiée et prendra en compte les nouveaux paramètres saisis (ex: suppression d'un produit). L'email de confirmation qui sera envoyé à la fermeture du cycle de vente reflètera bien la nouvelle situation, prenant en compte les changements effectués. Si vous ne voulez pas que les changements s'appliquent à la commande automatique déjà en cours, attendez la fin du cycle de vente pour modifier le paramétrage de la commande récurrente.&#x20;

### **Que se passe-t-il si le stock d'un produit ne permet pas de satisfaire toutes les commandes récurrente pour un cycle de vente donnée, et qu'un acheteur qui s'est vu alloué le stock demandé pour ce produit annule sa commande. Est-ce que ce stock sera réalloué à une autre commande automatique qui n'avait pas pu être satisfaite ?**&#x20;

Non. Si l'acheteur annule la commande ou retire le dit produit de sa commande, le stock du produit sera augmenté de la quantité correspondante, mais ne sera pas automatiquement réalloué à une autre commande automatique déjà passée. Vous pouvez cependant le faire manuellement en éditant une commande automatique spécifique [selon le process décrit ici](broken-reference).
