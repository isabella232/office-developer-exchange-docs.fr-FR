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
ms.openlocfilehash: 44ee5dc465f4435f0b835d264331cb719fe875c1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755115"
---
# <a name="create-a-deliveryagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="7285b-103">Créer un agent de transport DeliveryAgent pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="7285b-103">Create a DeliveryAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="7285b-104">Découvrez comment créer un agent de transport DeliveryAgent personnalisé à utiliser avec Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="7285b-104">Find out how to create a custom DeliveryAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="7285b-105">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="7285b-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="7285b-106">Le [DeliveryAgentFactory\<Manager\> ](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentFactory`1.aspx) et [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx) classes sont les classes de base pour les agents de transport sont conçues pour s’exécuter sur le service de Transport sur un serveur de boîtes aux lettres de Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7285b-106">The [DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentFactory`1.aspx) and [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx) classes are the base classes for transport agents that are designed to run on the Transport service on an Exchange Server 2013 Mailbox server.</span></span> <span data-ttu-id="7285b-107">Vous pouvez implémenter des gestionnaires dans votre DeliveryAgent l’agent de transport pour les événements fournis par la classe [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx) qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="7285b-107">You might implement handlers in your DeliveryAgent transport agent for the events provided by the [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx) class that are listed in the following table.</span></span> 
  
<span data-ttu-id="7285b-108">**Le tableau 1. Événements de la classe DeliveryAgent**</span><span class="sxs-lookup"><span data-stu-id="7285b-108">**Table 1. DeliveryAgent class events**</span></span>

|<span data-ttu-id="7285b-109">**Événement**</span><span class="sxs-lookup"><span data-stu-id="7285b-109">**Event**</span></span>|<span data-ttu-id="7285b-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="7285b-110">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7285b-111">OnCloseConnection</span><span class="sxs-lookup"><span data-stu-id="7285b-111">OnCloseConnection</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnCloseConnection.aspx) <br/> |<span data-ttu-id="7285b-112">Cet événement se produit après le dernier élément de courrier a été remis et la connexion est fermée.</span><span class="sxs-lookup"><span data-stu-id="7285b-112">Occurs after the last mail item has been delivered and the connection is closed.</span></span>  <br/> |
|[<span data-ttu-id="7285b-113">OnDeliverMailItem</span><span class="sxs-lookup"><span data-stu-id="7285b-113">OnDeliverMailItem</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnDeliverMailItem.aspx) <br/> |<span data-ttu-id="7285b-114">Se produit lorsqu’un élément de courrier est prêt à être remis.</span><span class="sxs-lookup"><span data-stu-id="7285b-114">Occurs when a mail item is ready to be delivered.</span></span>  <br/> |
|[<span data-ttu-id="7285b-115">OnOpenConnection</span><span class="sxs-lookup"><span data-stu-id="7285b-115">OnOpenConnection</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnOpenConnection.aspx) <br/> |<span data-ttu-id="7285b-116">Se produit lorsque l’agent de remise est ouvert pour la remise du courrier.</span><span class="sxs-lookup"><span data-stu-id="7285b-116">Occurs when the delivery agent is opened for mail delivery.</span></span>  <br/> |
   
## <a name="creating-a-custom-deliveryagent-transport-agent"></a><span data-ttu-id="7285b-117">Création d’un agent de transport DeliveryAgent personnalisé</span><span class="sxs-lookup"><span data-stu-id="7285b-117">Creating a custom DeliveryAgent transport agent</span></span>

<span data-ttu-id="7285b-118">La procédure suivante explique comment créer un agent de transport DeliveryAgent personnalisé.</span><span class="sxs-lookup"><span data-stu-id="7285b-118">The following procedure describes how to create a custom DeliveryAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="7285b-119">Pour créer l’agent de transport</span><span class="sxs-lookup"><span data-stu-id="7285b-119">To create the transport agent</span></span>

1. <span data-ttu-id="7285b-120">Ajoutez des références aux espaces de noms.</span><span class="sxs-lookup"><span data-stu-id="7285b-120">Add references to the namespaces.</span></span>
    
   ```cs
        using Microsoft.Exchange.Data.Transport;
        using Microsoft.Exchange.Data.Transport.Delivery;
    
   ```

   <span data-ttu-id="7285b-121">Vous trouverez ces espaces de noms sur votre serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="7285b-121">You can find these namespaces on your Exchange server.</span></span> <span data-ttu-id="7285b-122">En ajoutant une référence à ces espaces de noms, vous aurez accès aux membres [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx) .</span><span class="sxs-lookup"><span data-stu-id="7285b-122">By adding a reference to these namespaces, you will have access to the [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx) members.</span></span> 
    
2. <span data-ttu-id="7285b-123">Implémenter la classe dérivée pour le [DeliveryAgentFactory\<Manager\> ](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentFactory`1.aspx) classe.</span><span class="sxs-lookup"><span data-stu-id="7285b-123">Implement the derived class for the [DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentFactory`1.aspx) class.</span></span> 
    
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

   <span data-ttu-id="7285b-124">Ce code instancie la classe dérivée et substituer la méthode **CreateAgent** pour créer une instance de votre nouvel agent personnalisé.</span><span class="sxs-lookup"><span data-stu-id="7285b-124">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> <span data-ttu-id="7285b-125">Méthodes supplémentaires, telles que **Close**, peuvent également être remplacés dans cette classe pour exécuter du code personnalisé.</span><span class="sxs-lookup"><span data-stu-id="7285b-125">Additional methods, such as **Close**, can also be overridden in this class to execute custom code.</span></span> <span data-ttu-id="7285b-126">Une classe [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx) est créée pour remplacer la propriété [SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx) et de définir le protocole utilisé par l’agent.</span><span class="sxs-lookup"><span data-stu-id="7285b-126">A [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx) class is created to override the [SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx) property and set the protocol your agent will use.</span></span> 
    
3. <span data-ttu-id="7285b-127">Définir votre agent.</span><span class="sxs-lookup"><span data-stu-id="7285b-127">Define your agent.</span></span>
    
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

   <span data-ttu-id="7285b-128">Une fois que vous définissez votre classe agent, vous pouvez vous ajouter des fonctionnalités personnalisées.</span><span class="sxs-lookup"><span data-stu-id="7285b-128">After you define your agent class, you can add you custom functionality.</span></span> <span data-ttu-id="7285b-129">Dans cet exemple, les trois événements, [OnCloseConnection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnCloseConnection.aspx) , [OnDeliverMailItem](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnDeliverMailItem.aspx) et [OnOpenConnection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnOpenConnection.aspx) , sont redirigés vers vos gestionnaires d’événements personnalisés.</span><span class="sxs-lookup"><span data-stu-id="7285b-129">In this example, the three events, [OnCloseConnection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnCloseConnection.aspx) , [OnDeliverMailItem](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnDeliverMailItem.aspx) and [OnOpenConnection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnOpenConnection.aspx) , are redirected to your custom event handlers.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="7285b-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7285b-130">See also</span></span>

- [<span data-ttu-id="7285b-131">Concepts de l’agent d’Exchange 2013 de transport</span><span class="sxs-lookup"><span data-stu-id="7285b-131">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
- [<span data-ttu-id="7285b-132">Référence de l’agent de transport pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="7285b-132">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)    
- [<span data-ttu-id="7285b-133">DeliveryAgentFactory\<Manager\></span><span class="sxs-lookup"><span data-stu-id="7285b-133">DeliveryAgentFactory\<Manager\></span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentFactory`1.aspx)   
- [<span data-ttu-id="7285b-134">DeliveryAgent</span><span class="sxs-lookup"><span data-stu-id="7285b-134">DeliveryAgent</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx)    
- [<span data-ttu-id="7285b-135">DeliveryAgentManager</span><span class="sxs-lookup"><span data-stu-id="7285b-135">DeliveryAgentManager</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx)
    

