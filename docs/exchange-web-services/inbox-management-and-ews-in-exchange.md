---
title: Gestion de la boîte de réception et EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 3dfa0fc9-64bb-4d18-bff7-bf6b3bed4a0d
description: Découvrez comment gérer votre boîte de réception dans votre API gérée EWS ou votre application EWS à l’aide de règles de boîte de réception et de la liste des expéditeurs bloqués.
ms.openlocfilehash: 6dddb8d462276c4983fd04a0206d4d4a9be32df8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522214"
---
# <a name="inbox-management-and-ews-in-exchange"></a>Gestion de la boîte de réception et EWS dans Exchange

Découvrez comment gérer votre boîte de réception dans votre API gérée EWS ou votre application EWS à l’aide de règles de boîte de réception et de la liste des expéditeurs bloqués.
  
Exchange boîtes aux lettres sont dotées de fonctionnalités pour aider les utilisateurs à organiser automatiquement leur courrier entrant. Ces fonctionnalités fonctionnent toutes sur le serveur sans intervention de l’utilisateur, mais elles servent des besoins différents. L’API gérée EWS et EWS permettent d’accéder à ces fonctionnalités, ce qui permet à vos utilisateurs de gérer leurs boîtes de réception.
  
**Tableau 1. Fonctionnalités de gestion de la boîte de réception**

|**Si vous souhaitez...**|**Utilisez...**|
|:-----|:-----|
|Prendre des mesures sur les messages entrants (par exemple, les déplacer vers un autre dossier ou les supprimer) en fonction de critères spécifiques (expéditeur, objet ou pièces jointes, par exemple)  <br/> |Règles de la boîte de réception  <br/> |
|Supprimer tous les messages entrants d’un expéditeur particulier  <br/> |liste des expéditeurs bloqués  <br/> |
   
## <a name="inbox-rules"></a>Règles de la boîte de réception
<a name="bk_InboxRules"> </a>

Nous allons le faire : tous les messages électroniques ne sont pas égaux. Pour chaque e-mail qu’un utilisateur reçoit de son responsable, il en existe un à partir d’une liste de distribution de vidéos de chat Internet qu’il a rejointe il y a des années et qu’il n’a jamais pu quitter. Bien que les vidéos de chat Sur Internet soient agréables, la quantité de trafic qu’obtient la liste de distribution peut se perdre et les messages importants peuvent facilement être perdus dans la mer des messages de la liste de distribution dans une boîte de réception. De nombreux utilisateurs se tournent vers les règles de boîte de réception pour les aider à les parer et à les rendre beaucoup plus agréables. Avec Exchange Web Services (EWS), votre application peut prendre en compte la puissance des règles.
  
L’API gérée EWS fournit les méthodes [ExchangeService.GetInboxRules](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getinboxrules%28v=exchg.80%29.aspx) et [ExchangeService.UpdateInboxRules](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.updateinboxrules%28v=exchg.80%29.aspx) pour l’application de règles. EWS fournit les opérations [GetInboxRules](https://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx) et [UpdateInboxRules](https://msdn.microsoft.com/library/f982a237-471e-45c5-a2b5-468cfc53150b%28Office.15%29.aspx) pour l’exploitation des règles. Toutefois, notez que l’API gérée EWS et EWS ont les limitations suivantes lorsque vous travaillez avec des règles de boîte de réception : 
  
- EWS ne peut pas accéder ou créer des règles « client uniquement » ou des règles définies dans Outlook pour s’exécuter « sur cet ordinateur uniquement ».
    
- Pour modifier l’ensemble actuel de règles à l’aide d’EWS, vous devez supprimer les règles Outlook BLOB, si elles sont présentes. Cela signifie que l’utilisation d’EWS pour modifier des règles supprime toutes les règles qui ont été précédemment désactivées (désactivées) à l’aide de Outlook. 
    
### <a name="how-do-rules-work"></a>Comment fonctionnent les règles ?
<a name="bk_HowRulesWork"> </a>

Le moteur de règles agit comme un garde d’accès à la boîte aux lettres d’un utilisateur. À mesure qu’un message arrive dans la boîte aux lettres de l’utilisateur, mais avant qu’il apparaisse dans la boîte de réception, ce message est évalué par rapport à une liste de règles ordonnée. Notez que cela se produit uniquement au moment de l’arrivée et uniquement dans la boîte de réception. Ces règles sont composées de trois parties : [Conditions,](#bk_Conditions) [Actions](#bk_Actions)et [Exceptions.](#bk_Exceptions)
  
En commençant par la règle en haut de la liste de règles, le moteur de règles effectue les étapes suivantes jusqu’à ce qu’il atteigne la fin de la liste de règles :
  
1. Vérifie le message pour déterminer s’il répond à toutes les conditions spécifiées dans la règle.
    
1. Si elle répond à toutes les conditions, l’évaluation se poursuit à l’étape 2.
    
2. S’il ne répond pas à toutes les conditions, le moteur de règles charge la règle suivante dans la liste de règles et recommence à l’étape 1.
    
2. Vérifie le message pour déterminer s’il répond à l’une des exceptions spécifiées dans la règle.
    
1. S’il répond à l’une des exceptions, le moteur de règles charge la règle suivante dans la liste des règles et recommence à l’étape 1.
    
2. Si elle ne répond à aucune des exceptions, l’évaluation se poursuit à l’étape 3.
    
3. Effectue les actions spécifiées dans la règle sur le message.
    
1. Si l’action « Arrêter de traiter plus de règles » est spécifiée, le moteur de règles effectue toutes les autres actions sur le message, puis se quitte sans évaluer de règles supplémentaires par rapport au message.
    
2. Si l’action « Arrêter de traiter plus de règles » n’est pas spécifiée, le moteur de règles charge la règle suivante dans la liste des règles et recommence à l’étape 1.
    
La figure suivante illustre le processus suivi par le moteur de règles.
  
**Figure 1 : Vue d’ensemble du moteur de règles**

![Diagramme indiquant les différentes étapes utilisées par le moteur de règles, en commençant par l’évaluation de la règle, puis la vérification visant à déterminer si les critères de la règle sont remplis, puis l’exécution de l’action ou le passage à la règle suivante jusqu’à la fin du processus.](media/Ex15_Rules_EngineOverview.png)
  
### <a name="putting-the-pieces-together---parts-of-a-rule"></a>Rassembler les éléments - parties d’une règle
<a name="bk_Pieces"> </a>

Une façon de visualiser les parties d’une règle consiste à imaginer que vous donnez des instructions à une personne chargée d’organiser votre courrier entrant. Vous pouvez dire à cette personne : « Lorsqu’un message arrive, \<insert conditions here\> \<insert actions here\> faites, sauf si le message \<insert exceptions here\> . Examinons chaque partie de plus près.
  
#### <a name="conditions"></a>Conditions
<a name="bk_Conditions"> </a>

[Les conditions](https://msdn.microsoft.com/library/f049a48c-9585-43f7-8549-0b8cb19a5eea%28Office.15%29.aspx) décrivent quand une règle doit être appliquée. Bien que vous pouvez omettre les conditions d’une règle (ce qui entraîne une règle qui s’applique à chaque message reçu), il est beaucoup plus courant pour les règles d’avoir des conditions qui s’appliquent à un sous-ensemble de messages entrants. Voici quelques exemples : « lorsqu’un message est de Sadie » ou « lorsqu’un message est envoyé à la liste de distribution « Cat Video Fanss ». Les règles peuvent avoir plusieurs conditions. Lorsque les règles ont plusieurs conditions, toutes les conditions doivent être remplies pour que le moteur de règles prenne l’action spécifiée. 
  
#### <a name="actions"></a>Actions
<a name="bk_Actions"> </a>

[Les actions](https://msdn.microsoft.com/library/c5aa96b1-2d8b-422f-8c2f-f118572ab23f%28Office.15%29.aspx) décrivent ce qui se produit lorsqu’une règle s’applique. Par exemple, « déplacer le message vers le dossier Chats » ou « marquer le message avec une importance faible ». Les règles peuvent avoir plusieurs actions. Lorsque vous spécifiez plusieurs actions pour une règle, toutes les actions sont effectuées lorsque la règle est appliquée. 
  
#### <a name="exceptions"></a>Exceptions
<a name="bk_Exceptions"> </a>

[Les exceptions](https://msdn.microsoft.com/library/7cd63ac2-3441-4ed4-915b-6f90af4b28fc%28Office.15%29.aspx) décrivent quand une règle ne doit pas s’appliquer, même si les critères spécifiés dans les conditions sont satisfaits. Par exemple, « sauf si le message m’est envoyé uniquement » ou « sauf si le message est de Mom ». Une règle peut avoir plusieurs exceptions. Lorsque les règles ont plusieurs exceptions et qu’aucune des exceptions n’est remplie, la règle n’est pas appliquée. 
  
### <a name="example-herding-those-cats"></a>Exemple : l’antage de ces chats
<a name="bk_Example"> </a>

Examinons comment vos utilisateurs peuvent utiliser des règles pour éliminer le trafic de cette liste de distribution de vidéos de chat Internet. Supposons les choses suivantes :
  
- Ces messages sont envoyés à une liste de distribution appelée « Internet Cat Video Enthusiasts ».
    
- Vos utilisateurs souhaitent finir par lire ces messages, ils ne veulent simplement pas qu’ils encombrent leur boîte de réception. Ils préfèrent les déposer dans un dossier appelé « Chats ».
    
- Vos utilisateurs souhaitent lire immédiatement les messages envoyés à cette liste de distribution par leur mère, car Mom envoie les vidéos les plus agréables.
    
Cela indique au moteur de règles ce qui suit : « Lorsqu’un message est envoyé à la liste de distribution « Internet Cat Video Enthusiasts », déplacez-le vers le dossier « Chats », sauf si le message est de Mom. 
  
**Tableau 2. Définition de règle**

|**Partie de règle**|**Valeur**|
|:-----|:-----|
|Conditions  <br/> |Envoyé à la liste de distribution « Fans d’Internet Cat Video »  <br/> |
|Actions  <br/> |Déplacer le message vers le dossier « Chats »  <br/> ET arrêter le traitement d’autres règles  <br/> |
|Exceptions  <br/> |À partir de « Mom »  <br/> |
   
> [!NOTE]
> Notez que « arrêter le traitement d’autres règles » est l’une des actions de la règle résultante. En règle générale, il est bon d’inclure cette action pour éviter toute confusion quant aux règles qui agissent sur un message donné. Toutefois, en omettant cette action et en orderant correctement vos règles, vous pouvez obtenir un traitement plus avancé de votre courrier entrant. Dans ce cas, il est probable que les messages vidéo de chat Internet ne nécessitent pas beaucoup de traitement avancé. 
  
Peu de temps après la création de cette règle, un nouveau message entre. Un collègue Espér envoie un message à la liste de distribution. Si nous insérons effectuer le travail du moteur de règles, le message répond à toutes les conditions (il est envoyé aux « fans de vidéos de chat Internet » et ne répond à aucune des exceptions (il ne vient pas de « Mom », donc la règle s’applique et le message est déplacé vers le dossier « Chats ».
  
La figure suivante montre comment la règle est appliquée à un message électronique entrant.
  
**Figure 2. Le message entrant est traitée par une règle**

![Illustration présentant un nouveau message envoyé à la liste de distribution par un collègue. Le message remplit toutes les conditions et ne comprend aucune des exceptions définies dans la règle ; il est déplacé dans le dossier Chats.](media/Ex15_Rules_RuleEvaluationSample.png)
  
## <a name="blocking-senders"></a>Blocage des expéditeurs
<a name="bk_Blocking"> </a>

Bien que vous pouvez créer une règle qui déplacera tous les messages d’un expéditeur spécifique vers le dossier Courrier indésirable, vous pouvez également le faire à l’aide de la liste des expéditeurs bloqués dans vos options de courrier indésirable. Étant donné qu’il existe une limite au nombre de règles qu’un utilisateur peut avoir, il est logique d’utiliser la liste des expéditeurs bloqués. Vous pouvez ajouter ou supprimer des adresses de messagerie spécifiques de la liste des [expéditeurs bloqués](how-to-add-and-remove-email-addresses-from-blocked-senders-list-by-using-ews.md) à l’aide de la méthode d’API gérée EWS [ExchangeService.MarkAsJunk](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) ou de l’opération EWS [MarkAsJunk.](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) Notez que pour qu’EWS accède à la liste des expéditeurs bloqués, la boîte aux lettres de l’utilisateur doit contenir un message électronique provenant de l’adresse de messagerie que vous souhaitez ajouter ou supprimer. 
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_InThisSection"> </a>

- [Gérer les règles de boîte de réception à l’aide d’EWS dans Exchange](how-to-manage-inbox-rules-by-using-ews-in-exchange.md)
    
- [Ajouter et supprimer des adresses de messagerie de la liste des expéditeurs bloqués à l’aide d’EWS dans Exchange](how-to-add-and-remove-email-addresses-from-blocked-senders-list-by-using-ews.md)
    
## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Opération de GetInboxRules](https://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx)
    
- [Opération de UpdateInboxRules](https://msdn.microsoft.com/library/f982a237-471e-45c5-a2b5-468cfc53150b%28Office.15%29.aspx)
    
- [Opération MarkAsJunk](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)
    

