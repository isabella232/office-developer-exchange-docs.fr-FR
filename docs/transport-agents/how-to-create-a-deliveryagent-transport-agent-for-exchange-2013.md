---
title: Créer un agent de transport DeliveryAgent pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4af904d7-b315-4849-92b1-66018f76ffdf
description: Découvrez comment créer un agent de transport DeliveryAgent personnalisé à utiliser avec Exchange 2013.
ms.openlocfilehash: bc36c7b5e0fb8006c5927d423d7767dcc7382ce0
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353307"
---
# <a name="create-a-deliveryagent-transport-agent-for-exchange-2013"></a>Créer un agent de transport DeliveryAgent pour Exchange 2013

Découvrez comment créer un agent de transport DeliveryAgent personnalisé à utiliser avec Exchange 2013.
  
**S’applique à :** Exchange Server 2013
  
Le [DeliveryAgentFactory\<Manager\> ](https://msdn.microsoft.com/en-us/library/dd877550(v=exchg.150).aspx) et [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) classes sont les classes de base pour les agents de transport sont conçues pour s’exécuter sur le service de Transport sur un serveur de boîtes aux lettres de Exchange Server 2013. Vous pouvez implémenter des gestionnaires dans votre DeliveryAgent l’agent de transport pour les événements fournis par la classe [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) qui sont répertoriés dans le tableau suivant. 
  
**Le tableau 1. Événements de la classe DeliveryAgent**

|**Événement**|**Description**|
|:-----|:-----|
|[OnCloseConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx) <br/> |Cet événement se produit après le dernier élément de courrier a été remis et la connexion est fermée.  <br/> |
|[OnDeliverMailItem](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx) <br/> |Se produit lorsqu’un élément de courrier est prêt à être remis.  <br/> |
|[OnOpenConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx) <br/> |Se produit lorsque l’agent de remise est ouvert pour la remise du courrier.  <br/> |
   
## <a name="creating-a-custom-deliveryagent-transport-agent"></a>Création d’un agent de transport DeliveryAgent personnalisé

La procédure suivante explique comment créer un agent de transport DeliveryAgent personnalisé. 
  
### <a name="to-create-the-transport-agent"></a>Pour créer l’agent de transport

1. Ajoutez des références aux espaces de noms.
    
   ```cs
        using Microsoft.Exchange.Data.Transport;
        using Microsoft.Exchange.Data.Transport.Delivery;
    
   ```

   Vous trouverez ces espaces de noms sur votre serveur Exchange. En ajoutant une référence à ces espaces de noms, vous aurez accès aux membres [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) . 
    
2. Implémenter la classe dérivée pour le [DeliveryAgentFactory\<Manager\> ](https://msdn.microsoft.com/en-us/library/dd877550(v=exchg.150).aspx) classe. 
    
   ```cs
      public class MyDeliveryAgentFactory : DeliveryAgentFactory<MyDeliveryAgentFactory.MyDeliveryAgentManager>
      {
          static MyDeliveryAgentFactory()
          {
          }
          public override DeliveryAgent CreateAgent(SmtpServer server)
          {
              return new MyDeliveryAgent(server);
          }
          public sealed class MyDeliveryAgentManager : DeliveryAgentManager
          {
              /// <summary>
              /// Gets the supported delivery protocol.
              /// </summary>
              public override string SupportedDeliveryProtocol
              {
                  get { return "MyProtocol"; }
              }
          }
      }
  
   ```

   Ce code instancie la classe dérivée et substituer la méthode **CreateAgent** pour créer une instance de votre nouvel agent personnalisé. Méthodes supplémentaires, telles que **Close**, peuvent également être remplacés dans cette classe pour exécuter du code personnalisé. Une classe [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx) est créée pour remplacer la propriété [SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx) et de définir le protocole utilisé par l’agent. 
    
3. Définir votre agent.
    
   ```cs
      public class MyDeliveryAgent : DeliveryAgent
      {
          public MyDeliveryAgent(SmtpServer server)
          {
              this.OnCloseConnection += CloseConnection;
              this.OnDeliverMailItem += DeliverMailItem;
              this.OnOpenConnection += OpenConnection;
          }
      }
  
   ```

   Une fois que vous définissez votre classe agent, vous pouvez vous ajouter des fonctionnalités personnalisées. Dans cet exemple, les trois événements, [OnCloseConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx), [OnDeliverMailItem](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)et [OnOpenConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx), sont redirigés vers vos gestionnaires d’événements personnalisés. 
    
## <a name="see-also"></a>Voir aussi

- [Concepts sur les agents de transport dans Exchange 2013](transport-agent-concepts-in-exchange-2013.md)
- [Référence de l’agent de transport pour Exchange 2013](transport-agent-reference-for-exchange-2013.md)          

 