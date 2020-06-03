---
title: Gestion de la boîte de réception et EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3dfa0fc9-64bb-4d18-bff7-bf6b3bed4a0d
description: Découvrez comment gérer votre boîte de réception dans votre application EWS ou l’API managée EWS à l’aide de règles de boîte de réception et de la liste des expéditeurs bloqués.
ms.openlocfilehash: 7c88015386dc882f14184765e0046a866e8c0e10
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456314"
---
# <a name="inbox-management-and-ews-in-exchange"></a>Gestion de la boîte de réception et EWS dans Exchange

Découvrez comment gérer votre boîte de réception dans votre application EWS ou l’API managée EWS à l’aide de règles de boîte de réception et de la liste des expéditeurs bloqués.
  
Les boîtes aux lettres Exchange sont équipées de fonctionnalités permettant aux utilisateurs d’organiser automatiquement leurs courriers électroniques entrants. Ces fonctionnalités fonctionnent toutes sur le serveur sans intervention de l’utilisateur, mais elles répondent à différents besoins. L’API managée EWS et EWS fournissent un accès à ces fonctionnalités, permettant ainsi à vos utilisateurs de gérer leur boîte de réception.
  
**Tableau 1. Fonctionnalités de gestion de la boîte de réception**

|**Si vous souhaitez...**|**Utiliser...**|
|:-----|:-----|
|Effectuer des actions sur les messages entrants (tels que les placer dans un autre dossier ou les supprimer) en fonction de critères spécifiques (tels que l’expéditeur, l’objet ou les pièces jointes)  <br/> |Règles de la boîte de réception  <br/> |
|Supprimer tous les messages entrants d’un expéditeur particulier  <br/> |liste des expéditeurs bloqués  <br/> |
   
## <a name="inbox-rules"></a>Règles de la boîte de réception
<a name="bk_InboxRules"> </a>

Nous allons le faire face : les messages électroniques ne sont pas tous égaux. Pour chaque message envoyé par un utilisateur à partir de son responsable, il s’agit d’une liste de distribution vidéo de chat Internet qu’il a rejoint les années et qu’il n’a jamais eu le temps de quitter. Bien que les vidéos de chat Internet soient divertissantes, la quantité de trafic qu’elle obtient peut être indisponible et des messages importants peuvent facilement être perdus dans la boîte aux lettres de liste de distribution dans une boîte de réception. De nombreux utilisateurs contournent des règles de boîte de réception pour réduire ces messages et faire de leur boîte de réception un bien plus attrayant. Avec les services Web Exchange (EWS), votre application peut mettre en place la puissance des règles.
  
L’API managée EWS fournit les méthodes [ExchangeService. GetInboxRules](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getinboxrules%28v=exchg.80%29.aspx) et [ExchangeService. UpdateInboxRules](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.updateinboxrules%28v=exchg.80%29.aspx) pour l’utilisation de règles. EWS fournit les opérations [GetInboxRules](https://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx) et [UpdateInboxRules](https://msdn.microsoft.com/library/f982a237-471e-45c5-a2b5-468cfc53150b%28Office.15%29.aspx) pour l’utilisation de règles. Toutefois, Notez que l’API managée EWS et EWS ont les limitations suivantes lorsque vous utilisez des règles de boîte de réception : 
  
- EWS ne peut pas accéder à ou créer des règles ou des règles qui sont définies dans Outlook pour s’exécuter uniquement sur cet ordinateur.
    
- Pour modifier l’ensemble actuel de règles à l’aide d’EWS, vous devez supprimer l’objet BLOB de règles Outlook, s’il est présent. Cela signifie que l’utilisation d’EWS pour modifier des règles supprime toutes les règles désactivées précédemment désactivées à l’aide d’Outlook. 
    
### <a name="how-do-rules-work"></a>Comment fonctionnent les règles ?
<a name="bk_HowRulesWork"> </a>

Le moteur de règles agit comme un opérateur d’appels vers la boîte aux lettres d’un utilisateur. Lorsqu’un message arrive dans la boîte aux lettres de l’utilisateur, mais avant que le message s’affiche dans la boîte de réception, ce message est évalué par rapport à une liste ordonnée de règles. Notez que cette opération ne se produit qu’au moment de l’arrivée, et uniquement dans la boîte de réception. Ces règles se composent de trois parties : [conditions](#bk_Conditions), [actions](#bk_Actions)et [exceptions](#bk_Exceptions).
  
En commençant par la règle en haut de la liste des règles, le moteur de règles effectue les étapes suivantes jusqu’à la fin de la liste des règles :
  
1. Vérifie le message pour déterminer s’il remplit toutes les conditions spécifiées dans la règle.
    
1. Si elle répond à toutes les conditions, l’évaluation continue à l’étape 2.
    
2. Si elle ne remplit pas toutes les conditions, le moteur de règles charge la règle suivante dans la liste de règles et recommence à l’étape 1.
    
2. Vérifie le message pour déterminer s’il répond à l’une des exceptions spécifiées dans la règle.
    
1. Si elle répond à l’une des exceptions, le moteur de règles charge la règle suivante dans la liste de règles et recommence à l’étape 1.
    
2. S’il ne répond à aucune des exceptions, l’évaluation continue à l’étape 3.
    
3. Effectue les actions spécifiées dans la règle sur le message.
    
1. Si l’action « arrêter de traiter plus de règles » est spécifiée, le moteur de règles effectue toutes les autres actions sur le message, puis quitte sans évaluer les règles supplémentaires sur le message.
    
2. Si l’action « arrêter de traiter plus de règles » n’est pas spécifiée, le moteur de règles charge la règle suivante dans la liste de règles et recommence à l’étape 1.
    
La figure suivante illustre le processus suivi par le moteur de règles.
  
**Figure 1 : présentation du moteur de règles**

![Diagramme indiquant les différentes étapes utilisées par le moteur de règles, en commençant par l’évaluation de la règle, puis la vérification visant à déterminer si les critères de la règle sont remplis, puis l’exécution de l’action ou le passage à la règle suivante jusqu’à la fin du processus.](media/Ex15_Rules_EngineOverview.png)
  
### <a name="putting-the-pieces-together---parts-of-a-rule"></a>Regroupement des parties d’une règle
<a name="bk_Pieces"> </a>

Pour visualiser les parties d’une règle, imaginez que vous donnez des instructions à une personne chargée de l’organisation de votre courrier entrant. Vous pouvez indiquer à cette personne : «lorsqu’un message arrive \<insert conditions here\> , faites \<insert actions here\> , sauf si le message s’affiche \<insert exceptions here\> . Examinons de plus près chaque partie.
  
#### <a name="conditions"></a>Conditions
<a name="bk_Conditions"> </a>

Les [conditions](https://msdn.microsoft.com/library/f049a48c-9585-43f7-8549-0b8cb19a5eea%28Office.15%29.aspx) indiquent quand une règle doit être appliquée. Bien que vous puissiez omettre les conditions d’une règle (ce qui entraîne une règle qui s’applique à tous les messages reçus), il est beaucoup plus courant que les règles aient des conditions qui s’appliquent à un sous-ensemble de messages entrants. Voici quelques exemples : « lorsqu’un message provient de Sadie » ou « lorsqu’un message est envoyé à la liste de distribution «Cat Video Lovers ». Les règles peuvent avoir plusieurs conditions. Lorsque les règles ont plusieurs conditions, toutes les conditions doivent être remplies pour que le moteur de règles prenne l’action spécifiée. 
  
#### <a name="actions"></a>Actions
<a name="bk_Actions"> </a>

Les [actions](https://msdn.microsoft.com/library/c5aa96b1-2d8b-422f-8c2f-f118572ab23f%28Office.15%29.aspx) décrivent ce qui se produit lorsqu’une règle s’applique. Les exemples sont « déplacer le message vers le dossier «chats » ou « marquer le message avec une importance faible ». Les règles peuvent avoir plusieurs actions. Lorsque vous spécifiez plusieurs actions pour une règle, toutes les actions sont exécutées lors de l’application de la règle. 
  
#### <a name="exceptions"></a>Exceptions
<a name="bk_Exceptions"> </a>

Les [exceptions](https://msdn.microsoft.com/library/7cd63ac2-3441-4ed4-915b-6f90af4b28fc%28Office.15%29.aspx) indiquent quand une règle ne doit pas s’appliquer, même si les critères spécifiés dans les conditions sont satisfaits. Les exemples sont « sauf si le message est envoyé uniquement à moi » ou « sauf si le message provient de MOM ». Une règle peut avoir plusieurs exceptions. Lorsque les règles ont plusieurs exceptions et que n’importe quelle exception est satisfaite, la règle n’est pas appliquée. 
  
### <a name="example-herding-those-cats"></a>Exemple : troupeau de ces chats
<a name="bk_Example"> </a>

Examinons comment vos utilisateurs peuvent utiliser des règles pour éliminer le trafic provenant de cette liste de distribution vidéo de chat Internet. Supposons les points suivants :
  
- Ces messages sont envoyés à une liste de distribution appelée « passionnés de vidéo de chat Internet ».
    
- Vos utilisateurs veulent lire ces messages finalement, ils ne souhaitent pas encombrer leur boîte de réception. Ils préfèrent les classer dans un dossier appelé « chats ».
    
- Vos utilisateurs souhaitent lire les messages envoyés à cette liste de distribution directement par leur mère, car MOM envoie les vidéos Funniest.
    
Cela indique au moteur de règles ce qui suit : « lorsqu’un message arrive, envoyé à la liste de distribution «passionnés de vidéos de chat Internet », déplacez-le vers le dossier « chats », sauf si le message provient de MOM. 
  
**Tableau 2. Définition de la règle**

|**Composant de règle**|**Valeur**|
|:-----|:-----|
|Conditions  <br/> |Envoyé à la liste de distribution « passionnés de vidéo de catégorie Internet »  <br/> |
|Actions  <br/> |Déplacer le message vers le dossier « chats »  <br/> ET arrêter le traitement de règles supplémentaires  <br/> |
|Exceptions  <br/> |À partir de « MOM »  <br/> |
   
> [!NOTE]
> Notez que « arrêter de traiter plus de règles » est l’une des actions de la règle qui en résulte. En règle générale, il est recommandé d’inclure cette action afin d’éviter toute confusion quant aux règles qui agissent sur un message donné. Toutefois, en omettant cette action et en commandant correctement vos règles, vous pouvez obtenir un traitement plus avancé de vos messages entrants. Dans ce cas, il s’agit probablement d’un pari sûr que les messages vidéo de catégorie Internet ne nécessitent pas un traitement avancé. 
  
Peu de plus après la création de cette règle, un nouveau message arrive. Un collègue espère envoyer un message à la liste de distribution. Si nous avions le travail du moteur de règles, le message remplit toutes les conditions (il est envoyé aux passionnés de vidéos de catégorie Internet) et il ne répond à aucune des exceptions (il ne provient pas de « MOM »), de sorte que la règle s’applique et que le message est déplacé vers le dossier « chats ».
  
La figure suivante illustre l’application de la règle à un message électronique entrant.
  
**Figure 2. Le message entrant est traité par une règle**

![Illustration présentant un nouveau message envoyé à la liste de distribution par un collègue. Le message remplit toutes les conditions et ne comprend aucune des exceptions définies dans la règle ; il est déplacé dans le dossier Chats.](media/Ex15_Rules_RuleEvaluationSample.png)
  
## <a name="blocking-senders"></a>Blocage des expéditeurs
<a name="bk_Blocking"> </a>

Bien que vous puissiez créer une règle qui déplace tous les messages d’un expéditeur spécifique vers le dossier courrier indésirable, vous pouvez également le faire à l’aide de la liste des expéditeurs bloqués dans vos options de courrier indésirable. Étant donné que le nombre de règles dont dispose un utilisateur est limité, il est logique d’utiliser la liste des expéditeurs bloqués. Vous pouvez [Ajouter ou supprimer des adresses de messagerie spécifiques de la liste des expéditeurs bloqués](how-to-add-and-remove-email-addresses-from-blocked-senders-list-by-using-ews.md) à l’aide de la méthode de l’API managée EWS [ExchangeService. MarkAsJunk](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) ou de l’opération EWS [MarkAsJunk](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) . Notez que pour que EWS puisse accéder à la liste des expéditeurs bloqués, la boîte aux lettres de l’utilisateur doit contenir un message électronique à partir de l’adresse de messagerie que vous souhaitez ajouter ou supprimer. 
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_InThisSection"> </a>

- [Gérer les règles de boîte de réception à l’aide d’EWS dans Exchange](how-to-manage-inbox-rules-by-using-ews-in-exchange.md)
    
- [Ajouter et supprimer des adresses de messagerie de la liste des expéditeurs bloqués à l’aide d’EWS dans Exchange](how-to-add-and-remove-email-addresses-from-blocked-senders-list-by-using-ews.md)
    
## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Opération de GetInboxRules](https://msdn.microsoft.com/library/b4b2701a-4a23-4acc-8c75-19f7955ad7ae%28Office.15%29.aspx)
    
- [Opération de UpdateInboxRules](https://msdn.microsoft.com/library/f982a237-471e-45c5-a2b5-468cfc53150b%28Office.15%29.aspx)
    
- [Opération MarkAsJunk](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)
    

