---
title: Gestion de la boîte de réception et les services EWS d’Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3dfa0fc9-64bb-4d18-bff7-bf6b3bed4a0d
description: Découvrez comment vous pouvez gérer votre boîte de réception dans vos applications EWS ou votre API managées à l’aide de règles de boîte de réception et la liste des expéditeurs bloqués.
ms.openlocfilehash: fe06c5ee87e2679506ca7247c5fc2c96912dee86
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754961"
---
# <a name="inbox-management-and-ews-in-exchange"></a>Gestion de la boîte de réception et les services EWS d’Exchange

Découvrez comment vous pouvez gérer votre boîte de réception dans vos applications EWS ou votre API managées à l’aide de règles de boîte de réception et la liste des expéditeurs bloqués.
  
Boîtes aux lettres Exchange sont équipés de fonctionnalités pour aider les utilisateurs à organiser leur courrier entrant automatiquement. Ces fonctions de tous les fonctionnent sur le serveur sans intervention de l’utilisateur, mais ils sont différents besoins. Les API managées EWS fournir un accès à ces fonctionnalités, permettant à vos utilisateurs à gérer leurs boîtes aux lettres.
  
**Le tableau 1. Fonctionnalités de gestion de boîte de réception**

|**Si vous souhaitez...**|**Utilisez...**|
|:-----|:-----|
|Agir sur les messages entrants (comme les déplacer vers un autre dossier ou de les supprimer) en fonction des critères spécifiques (tels que l’expéditeur, l’objet ou les pièces jointes)  <br/> |Règles de boîte de réception  <br/> |
|Supprimer tous les messages entrants provenant d’un expéditeur particulier  <br/> |Liste des expéditeurs bloqués  <br/> |
   
## <a name="inbox-rules"></a>Règles de boîte de réception
<a name="bk_InboxRules"> </a>

Nous allons en face : pas de chaque message électronique est égales. Pour chaque e-mail qu'obtient d’un utilisateur à partir de son responsable, est un à partir d’une liste de distribution vidéo cat Internet qu’il rejoint ans et jamais compris autour pour quitter. Vidéos de Chat Internet sont divertissement, la quantité de trafic Obtient de liste de distribution peut obtenir inutilisable et les messages importants permettre facilement être perdue dans la mer du courrier de liste de distribution dans une boîte de réception. Nombre d’utilisateurs activer les règles de boîte de réception pour aider à réduire ces messages et passer d’un endroit bien mieux à leur boîte de réception. Exchange Web Services (EWS), votre application peut alliance de la puissance des règles de prendre en charge.
  
L’API managée EWS fournit les méthodes [ExchangeService.GetInboxRules](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getinboxrules%28v=exchg.80%29.aspx) et [ExchangeService.UpdateInboxRules](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.updateinboxrules%28v=exchg.80%29.aspx) pour l’utilisation de règles. EWS fournit les opérations [GetInboxRules](http://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx) et [UpdateInboxRules](http://msdn.microsoft.com/library/f982a237-471e-45c5-a2b5-468cfc53150b%28Office.15%29.aspx) pour l’utilisation de règles. Toutefois, notez que les API managées EWS présentent les limitations suivantes lorsque vous travaillez avec des règles de boîte de réception : 
  
- EWS ne peut pas accéder ou créer des règles « client seulement » ou les règles qui sont définies dans Outlook pour exécuter « sur cet ordinateur uniquement ».
    
- Pour modifier l’ensemble de règles à l’aide de EWS, vous devez supprimer les règles Outlook BLOB, s’il est présent. Cela signifie que pour modifier des règles à l’aide de EWS supprime toutes les règles qui ont été précédemment activés (désactivé) à l’aide d’Outlook. 
    
### <a name="how-do-rules-work"></a>Fonctionnement des règles
<a name="bk_HowRulesWork"> </a>

Le moteur de règles joue un opérateur pour la boîte aux lettres d’un utilisateur. Lorsqu’un message arrive dans la boîte aux lettres de l’utilisateur, mais avant que le message s’affiche dans la boîte de réception, ce message est évalué par rapport à une liste ordonnée de règles. Notez que cela ne se produit au moment de l’arrivée et uniquement dans la boîte de réception. Ces règles sont composés de trois parties : [Conditions](#bk_Conditions), [Actions](#bk_Actions)et [Exceptions](#bk_Exceptions).
  
À partir de la règle en haut de la liste des règles, le moteur de règles effectue les étapes suivantes jusqu'à la fin de la liste de règles :
  
1. Vérification du message pour déterminer si elle satisfait toutes les conditions spécifiées dans la règle.
    
1. S’il répond à toutes les conditions, l’évaluation continue à l’étape 2.
    
2. S’il ne respecte pas toutes les conditions, le moteur de règles charge la règle suivante dans la liste des règles et recommence à l’étape 1.
    
2. Vérification du message pour déterminer s’il répond aux exceptions spécifiées dans la règle.
    
1. S’il répond à des exceptions, le moteur de règles charge la règle suivante dans la liste des règles et recommence à l’étape 1.
    
2. Si elle ne répond pas aux exceptions, évaluation continue à l’étape 3.
    
3. Effectue les actions spécifiées dans la règle dans le message.
    
1. Si l’action « arrêter le traitement des règles plus » est spécifiée, le moteur de règles effectue toutes les autres actions dans le message, puis se ferme sans évaluer toutes les règles supplémentaires contre le message.
    
2. Si l’action « arrêter le traitement des règles plus » n’est pas spécifiée, le moteur de règles charge la règle suivante dans la liste des règles et recommence à l’étape 1.
    
La figure suivante illustre le processus que le moteur de règles suit.
  
**La figure 1 : Vue d’ensemble du moteur de règles**

![Diagramme indiquant les différentes étapes utilisées par le moteur de règles, en commençant par l’évaluation de la règle, puis la vérification visant à déterminer si les critères de la règle sont remplis, puis l’exécution de l’action ou le passage à la règle suivante jusqu’à la fin du processus.](media/Ex15_Rules_EngineOverview.png)
  
### <a name="putting-the-pieces-together---parts-of-a-rule"></a>Regroupement des différents éléments - composants d’une règle
<a name="bk_Pieces"> </a>

Permet de visualiser les composants d’une règle est d’imaginer que vous donnez à instructions à une personne qui est chargé de l’organisation de votre courrier électronique entrant. Vous pouvez dire à cette personne : « lorsqu’un message arrive qui \<insérer ici les conditions\>, procédez comme \<insérer ici les actions\>, à moins que le message \<insérer ici les exceptions\>. Prenons approfondie de chaque composant.
  
#### <a name="conditions"></a>Conditions
<a name="bk_Conditions"> </a>

[Conditions](http://msdn.microsoft.com/library/f049a48c-9585-43f7-8549-0b8cb19a5eea%28Office.15%29.aspx) décrivent quand une règle doit être appliquée. Alors que vous pouvez omettre les conditions d’une règle (entraînant une règle qui s’applique à tous les messages reçus), il est beaucoup plus courant pour les règles pour que les conditions qui s’appliquent à un sous-ensemble des messages entrants. « Lorsqu’un message provient Sadie » ou « lorsqu’un message est envoyé à la liste de distribution « Cat vidéo et » » sont des exemples. Règles peuvent avoir plusieurs conditions. Règles ont plusieurs conditions, toutes les conditions requises pour le moteur de règles d’effectuer l’action spécifiée par ordre. 
  
#### <a name="actions"></a>Actions
<a name="bk_Actions"> </a>

Décrivent les [actions](http://msdn.microsoft.com/library/c5aa96b1-2d8b-422f-8c2f-f118572ab23f%28Office.15%29.aspx) que se passe-t-il lorsqu’une règle s’applique. Exemples sont « déplacer le message vers le dossier « Chats » » ou « marquant le message avec une importance « Faible » ». Règles peuvent avoir plusieurs actions. Lorsque vous spécifiez plusieurs actions d’une règle, toutes les actions sont effectuées lors de la règle est appliquée. 
  
#### <a name="exceptions"></a>Exceptions
<a name="bk_Exceptions"> </a>

[Exceptions](http://msdn.microsoft.com/library/7cd63ac2-3441-4ed4-915b-6f90af4b28fc%28Office.15%29.aspx) décrivent quand une règle doit s’appliquer pas, même si les critères spécifiés dans les conditions sont remplies. « Sauf si le message est envoyé uniquement à moi » ou « sauf si le message provient Mom » sont des exemples. Une règle peut avoir plusieurs exceptions. Lorsque les règles ont plusieurs exceptions et des exceptions sont remplies, la règle n’est pas appliquée. 
  
### <a name="example-herding-those-cats"></a>Exemple : Regroupement de ces chats
<a name="bk_Example"> </a>

Examinons comment vos utilisateurs peuvent utiliser des règles pour éliminer le trafic de cette liste de distribution vidéo cat Internet. Supposons que les éléments suivants :
  
- Ces messages sont envoyés à une liste de distribution appelée « Internet Cat vidéo passionnés ».
    
- Vos utilisateurs à lire ces messages éventuellement, ils ne souhaitent les encombrer leur boîte de réception. Ils seraient plutôt les fichiers dans un dossier appelé « Chats ».
    
- Vos utilisateurs souhaitent lire les messages envoyés à cette liste de distribution à leur mère immédiatement, étant donné que Mom envoie les vidéos sous.
    
Ceci indique le moteur de règles ce qui suit : « lorsqu’un message arrive qui est envoyé à la liste de distribution « Internet Cat vidéo passionnés », déplacer vers le dossier « Chats », à moins que le message provient de Mom ». 
  
**Le tableau 2. Définition de la règle**

|**Composant de règle**|**Valeur**|
|:-----|:-----|
|Conditions  <br/> |Envoyé à la liste de distribution « Internet Cat vidéo passionnés »  <br/> |
|Actions  <br/> |Déplacer le message vers le dossier « Chats »  <br/> ET arrêter le traitement des règles  <br/> |
|Exceptions  <br/> |À partir de « Mom »  <br/> |
   
> [!NOTE]
> Notez que « arrêter le traitement des règles plus » est une des actions de la règle qui en résulte. En règle générale, il est préférable d’inclure cette action pour éviter toute confusion sur les règles agissent sur un message donné. Toutefois, en omettant cette action et correctement vos règles de tri, vous pouvez obtenir plus avancées de traitement de votre courrier entrant. Dans ce cas, il est probablement un résultat sûr que les messages vidéo Internet cat ne nécessitent pas beaucoup de cours de traitement avancé. 
  
Peu après la création de cette règle, un nouveau message est proposé sous. Un collègue expédition envoie un message à la liste de distribution. Si nous mentalement les tâches du moteur de règles, le message répond à toutes les conditions (il est envoyé à « Passionnés de vidéos Internet Cat »), et il répond à aucune des exceptions (il n’est pas de 'Mom'), si la règle s’applique et le message est déplacé vers le dossier « Chats ».
  
La figure suivante illustre la façon dont la règle est appliquée à un message électronique entrant.
  
**La figure 2. Message entrant est traité par une règle**

![Illustration présentant un nouveau message envoyé à la liste de distribution par un collègue. Le message remplit toutes les conditions et ne comprend aucune des exceptions définies dans la règle ; il est déplacé dans le dossier Chats.](media/Ex15_Rules_RuleEvaluationSample.png)
  
## <a name="blocking-senders"></a>Blocage des expéditeurs
<a name="bk_Blocking"> </a>

Bien que vous pouvez créer une règle qui va déplacer tous les messages d’un expéditeur spécifique dans le dossier courrier indésirable, vous pouvez également procéder ainsi à l’aide de la liste des expéditeurs bloqués dans vos options de courrier indésirable. Étant donné qu’une limite au nombre de règles un utilisateur peut avoir, il est logique d’utiliser la liste des expéditeurs bloqués. Vous pouvez [Ajouter ou supprimer des adresses de messagerie spécifiques à partir de la liste des expéditeurs bloqués](how-to-add-and-remove-email-addresses-from-blocked-senders-list-by-using-ews.md) à l’aide de la méthode d’API managées [ExchangeService.MarkAsJunk](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) ou l’opération EWS [MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) . Notez que pour accéder à la liste des expéditeurs bloqués EWS, boîte aux lettres de l’utilisateur doit contenir un message électronique à partir de l’adresse de messagerie que vous souhaitez ajouter ou supprimer. 
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_InThisSection"> </a>

- [Gérer les règles de boîte de réception à l’aide de EWS dans Exchange](how-to-manage-inbox-rules-by-using-ews-in-exchange.md)
    
- [Ajouter et supprimer des adresses de messagerie à partir de la liste des expéditeurs bloqués à l’aide de EWS dans Exchange](how-to-add-and-remove-email-addresses-from-blocked-senders-list-by-using-ews.md)
    
## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Opération de GetInboxRules](http://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx)
    
- [Opération de UpdateInboxRules](http://msdn.microsoft.com/library/f982a237-471e-45c5-a2b5-468cfc53150b%28Office.15%29.aspx)
    
- [Opération MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)
    

