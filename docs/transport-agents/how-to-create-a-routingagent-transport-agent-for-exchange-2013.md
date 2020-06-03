---
title: Création d’un agent de transport RoutingAgent pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f0e745f-9289-4f31-8877-926692a8c133
description: Découvrez comment créer un agent de transport RoutingAgent personnalisé à utiliser avec Exchange 2013.
ms.openlocfilehash: 9acf30be0dd795098f757effaa34b2e72183b000
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463698"
---
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a>Création d’un agent de transport RoutingAgent pour Exchange 2013

Découvrez comment créer un agent de transport RoutingAgent personnalisé à utiliser avec Exchange 2013.
  
**S’applique à :** Exchange Server 2013
  
Extraits de code et exemples d’applications connexes :

- [Exchange 2013 : créer un agent de transport de journalisation de bande passante](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
Les classes [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) et [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) sont les classes de base pour les agents de transport qui sont conçus pour s’exécuter sur le service de transport sur un serveur de boîtes aux lettres Exchange Server 2013. La classe [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) fournit les événements figurant dans le tableau suivant pour lequel vous pouvez implémenter les gestionnaires dans votre agent de transport RoutingAgent. 
  
**Tableau 1. Événements de classe RoutingAgent**

|**Event**|**Description**|
|:-----|:-----|
|[OnCategorizedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |Se produit après que le serveur effectue une conversion de contenu, si nécessaire.  <br/> |
|[OnResolvedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |Se produit après que tous les destinataires du message ont été résolus et avant que le routage soit déterminé.  <br/> |
|[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |Se produit après que le serveur a acheminé le message vers le tronçon suivant et effectue une conversion de contenu, si nécessaire. Le serveur peut utiliser plus de ressources pour traiter chaque message dans l’événement [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) que l’événement [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) , car le serveur effectuera toute conversion de contenu nécessaire et déterminera le tronçon suivant dans l’itinéraire du message avant d’exécuter le code dans le gestionnaire d’événements [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) .  <br/> |
|[OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |Se produit après la suppression du message de la file d’attente de soumission. Utilisez l’événement [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) si votre agent de transport RoutingAgent ne requiert pas de conversion de contenu, de destinataires résolus ou de données de routage.  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a>Création d’un agent de transport RoutingAgent personnalisé

La procédure suivante décrit comment créer un agent de transport RoutingAgent personnalisé. 
  
### <a name="to-create-the-transport-agent"></a>Pour créer l’agent de transport

1. Ajoutez des références aux espaces de noms.
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   Ces espaces de noms se trouvent sur votre serveur Exchange. En ajoutant une référence à ces espaces de noms, vous aurez accès aux membres [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) , ainsi qu’aux autres classes utilisées dans l’exemple [Exchange 2013 : créer un agent de transport de journalisation de bande passante](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) . 
    
2. Implémentez la classe dérivée pour la classe [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) . 
    
   ```cs
      public class BandwidthLoggerFactory : RoutingAgentFactory
      {
          public override RoutingAgent CreateAgent(SmtpServer server)
          {
              return new BandwidthLogger(server);
          }
      }
  
   ```

   Ce code instancie la classe dérivée et remplace la méthode **CreateAgent** pour créer une instance de votre nouvel agent personnalisé. Des méthodes supplémentaires, telles que **Close**, peuvent également être remplacées dans cette classe pour exécuter du code personnalisé. 
    
3. Définissez votre agent.
    
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

   Une fois que vous avez défini votre classe d’agent, vous pouvez ajouter des fonctionnalités personnalisées. Dans cet exemple, les deux événements [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) et [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)sont redirigés vers vos gestionnaires d’événements personnalisés. 
    
## <a name="see-also"></a>Voir aussi

- [Concepts sur les agents de transport dans Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Référence de l’agent de transport pour Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

