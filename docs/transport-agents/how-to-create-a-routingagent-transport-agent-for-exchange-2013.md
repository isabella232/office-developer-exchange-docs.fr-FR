---
title: Créer un agent de transport RoutingAgent pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f0e745f-9289-4f31-8877-926692a8c133
description: Découvrez comment créer un agent de transport RoutingAgent personnalisé à utiliser avec Exchange 2013.
ms.openlocfilehash: d07f68494acd26940a4837bbbfc7a0505114bd20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755125"
---
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a>Créer un agent de transport RoutingAgent pour Exchange 2013

Découvrez comment créer un agent de transport RoutingAgent personnalisé à utiliser avec Exchange 2013.
  
**S’applique à :** Exchange Server 2013
  
Extraits de code connexes et des exemples d’applications :

- [Exchange 2013 : Créer un agent de transport de journalisation de bande passante](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
Les classes [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) et [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) sont les classes de base pour les agents de transport sont conçues pour s’exécuter sur le service de transport sur un serveur de boîtes aux lettres de Exchange Server 2013. La classe [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) fournit les événements répertoriés dans le tableau suivant pour laquelle vous pouvez implémenter des gestionnaires dans votre RoutingAgent l’agent de transport. 
  
**Le tableau 1. Événements de la classe RoutingAgent**

|**Événement**|**Description**|
|:-----|:-----|
|[OnCategorizedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |Cet événement se produit une fois que le serveur effectue la conversion de contenu, si cela est nécessaire.  <br/> |
|[OnResolvedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |Se produit une fois que tous les destinataires du message ont été résolus et avant de routage est déterminé.  <br/> |
|[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |Cet événement se produit une fois que le serveur achemine le message vers le tronçon suivant et effectue la conversion de contenu, si nécessaire. Le serveur peut utiliser plus de ressources pour traiter chaque message dans l’événement [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) que l’événement [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) , car le serveur effectuer une conversion de contenu nécessaire et déterminer le tronçon suivant dans l’itinéraire pour le message avant d’exécuter le code dans le Gestionnaire d’événements [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) .  <br/> |
|[OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |Cet événement se produit une fois que le message est retiré de la file d’attente d’envoi. Utilisez l’événement [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) si l’agent de transport RoutingAgent ne requiert pas de conversion de contenu, destinataires résolus ou des données de routage.  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a>Création d’un agent de transport RoutingAgent personnalisé

La procédure suivante explique comment créer un agent de transport RoutingAgent personnalisé. 
  
### <a name="to-create-the-transport-agent"></a>Pour créer l’agent de transport

1. Ajoutez des références aux espaces de noms.
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   Vous trouverez ces espaces de noms sur votre serveur Exchange. En ajoutant une référence à ces espaces de noms, vous devez accéder aux membres [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) ainsi que d’autres classes utilisées dans le [Exchange 2013 : créer un agent de transport de journalisation de bande passante](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) exemple. 
    
2. Implémenter la classe dérivée de la classe [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) . 
    
   ```cs
      public class BandwidthLoggerFactory : RoutingAgentFactory
      {
          public override RoutingAgent CreateAgent(SmtpServer server)
          {
              return new BandwidthLogger(server);
          }
      }
  
   ```

   Ce code instancie la classe dérivée et substituer la méthode **CreateAgent** pour créer une instance de votre nouvel agent personnalisé. Méthodes supplémentaires, telles que **Close**, peuvent également être remplacés dans cette classe pour exécuter du code personnalisé. 
    
3. Définir votre agent.
    
   ```cs
      public class BandwidthLogger : RoutingAgent
      {
          // Your custom code goes here
          public BandwidthLogger(SmtpServer server)
          {
              Debug.WriteLine(logPrefix + "Agent constructor");
              this.server = server;
              this.OnSubmittedMessage += SubmittedMessage;
              this.OnRoutedMessage += RoutedMessage;
          }
      }
  
   ```

   Une fois que vous définissez votre classe agent, vous pouvez vous ajouter des fonctionnalités personnalisées. Dans cet exemple, les deux événements [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) et [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)sont redirigés vers vos gestionnaires d’événements personnalisés. 
    
## <a name="see-also"></a>Voir aussi

- [Concepts de l’agent d’Exchange 2013 de transport](transport-agent-concepts-in-exchange-2013.md)    
- [Référence de l’agent de transport pour Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

