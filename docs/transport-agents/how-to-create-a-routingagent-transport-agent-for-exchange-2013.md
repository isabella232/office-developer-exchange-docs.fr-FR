---
title: Créer un agent de transport RoutingAgent pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3f0e745f-9289-4f31-8877-926692a8c133
description: Découvrez comment créer un agent de transport RoutingAgent personnalisé à utiliser avec Exchange 2013.
ms.openlocfilehash: 70dbfc3c25e18195bb4b42fd3e750da11b0423d6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534173"
---
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a>Créer un agent de transport RoutingAgent pour Exchange 2013

Découvrez comment créer un agent de transport RoutingAgent personnalisé à utiliser avec Exchange 2013.
  
**S’applique à :** Exchange Server 2013
  
Extraits de code associés et exemples d’applications :

- [Exchange 2013 : Créer un agent de transport de journalisation de la bande passante](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
Les classes [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) et [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) sont les classes de base des agents de transport conçus pour s’exécuter sur le service de transport sur un serveur de boîtes aux lettres Exchange Server 2013. La [classe RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) fournit les événements répertoriés dans le tableau suivant pour lesquels vous pouvez implémenter des handlers dans votre agent de transport RoutingAgent. 
  
**Tableau 1. Événements de classe RoutingAgent**

|**Event**|**Description**|
|:-----|:-----|
|[OnCategorizedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |Se produit une fois que le serveur a effectué la conversion de contenu, si nécessaire.  <br/> |
|[OnResolvedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |Se produit après la résolution de tous les destinataires du message et avant la détermination du routage.  <br/> |
|[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |Se produit après que le serveur a route le message vers le saut suivant et effectue la conversion de contenu, si nécessaire. Le serveur peut utiliser plus de ressources pour traiter chaque message dans l’événement [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) que l’événement [OnSubmittedMessage,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) car le serveur effectue toute conversion de contenu nécessaire et détermine le saut suivant dans l’itinéraire du message avant d’exécuter le code dans le [handler d’événements OnRoutedMessage.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)  <br/> |
|[OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |Se produit une fois que le message est retiré de la file d’attente d’envoi. Utilisez [l’événement OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) si votre agent de transport RoutingAgent ne nécessite pas de conversion de contenu, de destinataires résolus ou de données de routage.  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a>Création d’un agent de transport RoutingAgent personnalisé

La procédure suivante décrit comment créer un agent de transport RoutingAgent personnalisé. 
  
### <a name="to-create-the-transport-agent"></a>Pour créer l’agent de transport

1. Ajoutez des références aux espaces de noms.
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   Vous pouvez trouver ces espaces de noms sur Exchange serveur. En ajoutant une référence à ces espaces de noms, vous aurez accès aux membres [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) ainsi qu’aux autres classes utilisées dans [Exchange 2013 :](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) créer un exemple d’agent de transport de journalisation de bande passante. 
    
2. Implémenter la classe dérivée pour la [classe RoutingAgentFactory.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) 
    
   ```cs
      public class BandwidthLoggerFactory : RoutingAgentFactory
      {
          public override RoutingAgent CreateAgent(SmtpServer server)
          {
              return new BandwidthLogger(server);
          }
      }
  
   ```

   Ce code ins instantique la classe dérivée et remplace la méthode **CreateAgent** pour créer une instance de votre nouvel agent personnalisé. D’autres méthodes, telles que **Close,** peuvent également être overridées dans cette classe pour exécuter du code personnalisé. 
    
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

   Après avoir défini votre classe d’agent, vous pouvez ajouter des fonctionnalités personnalisées. Dans cet exemple, les deux événements [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) et [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)sont redirigés vers vos handlers d’événements personnalisés. 
    
## <a name="see-also"></a>Voir aussi

- [Concepts sur les agents de transport dans Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Référence de l’agent de transport Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

