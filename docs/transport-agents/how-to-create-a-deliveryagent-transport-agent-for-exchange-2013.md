---
title: Créer un agent de transport DeliveryAgent pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 4af904d7-b315-4849-92b1-66018f76ffdf
description: Découvrez comment créer un agent de transport DeliveryAgent personnalisé à utiliser avec Exchange 2013.
ms.openlocfilehash: b465c3bbd4658bea700d5be9f4eb16ae81693717
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526932"
---
# <a name="create-a-deliveryagent-transport-agent-for-exchange-2013"></a>Créer un agent de transport DeliveryAgent pour Exchange 2013

Découvrez comment créer un agent de transport DeliveryAgent personnalisé à utiliser avec Exchange 2013.
  
**S’applique à :** Exchange Server 2013
  
Les classes [DeliveryAgentFactory \<Manager\> ](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) et [DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) sont les classes de base pour les agents de transport conçus pour s’exécuter sur le service de transport sur un serveur de boîtes aux lettres Exchange Server 2013. Vous pouvez implémenter des responsables dans votre agent de transport DeliveryAgent pour les événements fournis par la classe [DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) répertoriés dans le tableau suivant. 
  
**Tableau 1. Événements de classe DeliveryAgent**

|**Event**|**Description**|
|:-----|:-----|
|[OnCloseConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx) <br/> |Se produit après la livraison du dernier élément de courrier et la fermeture de la connexion.  <br/> |
|[OnDeliverMailItem](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx) <br/> |Se produit lorsqu’un élément de courrier est prêt à être remis.  <br/> |
|[OnOpenConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx) <br/> |Se produit lorsque l’agent de remise est ouvert pour la remise du courrier.  <br/> |
   
## <a name="creating-a-custom-deliveryagent-transport-agent"></a>Création d’un agent de transport DeliveryAgent personnalisé

La procédure suivante décrit comment créer un agent de transport DeliveryAgent personnalisé. 
  
### <a name="to-create-the-transport-agent"></a>Pour créer l’agent de transport

1. Ajoutez des références aux espaces de noms.
    
   ```cs
        using Microsoft.Exchange.Data.Transport;
        using Microsoft.Exchange.Data.Transport.Delivery;
    
   ```

   Vous pouvez trouver ces espaces de noms sur Exchange serveur. En ajoutant une référence à ces espaces de noms, vous aurez accès aux membres [DeliveryAgent.](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) 
    
2. Implémenter la classe dérivée pour [la classe \<Manager\> DeliveryAgentFactory.](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) 
    
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

   Ce code ins instantique la classe dérivée et remplace la méthode **CreateAgent** pour créer une instance de votre nouvel agent personnalisé. D’autres méthodes, telles que **Close,** peuvent également être overridées dans cette classe pour exécuter du code personnalisé. Une [classe DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx) est créée pour remplacer la propriété [SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx) et définir le protocole utilisé par votre agent. 
    
3. Définissez votre agent.
    
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

   Après avoir défini votre classe d’agent, vous pouvez ajouter des fonctionnalités personnalisées. Dans cet exemple, les trois [événements, OnCloseConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx), [OnDeliverMailItem](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)et [OnOpenConnection,](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx)sont redirigés vers vos handlers d’événements personnalisés. 
    
## <a name="see-also"></a>Voir aussi

- [Concepts sur les agents de transport dans Exchange 2013](transport-agent-concepts-in-exchange-2013.md)
- [Référence de l’agent de transport Exchange 2013](transport-agent-reference-for-exchange-2013.md)          

 