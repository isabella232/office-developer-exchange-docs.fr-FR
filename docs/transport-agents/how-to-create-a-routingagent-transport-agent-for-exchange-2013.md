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
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="ff8c5-103">Créer un agent de transport RoutingAgent pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="ff8c5-103">Create a RoutingAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="ff8c5-104">Découvrez comment créer un agent de transport RoutingAgent personnalisé à utiliser avec Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="ff8c5-104">Find out how to create a custom RoutingAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="ff8c5-105">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="ff8c5-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="ff8c5-106">Extraits de code connexes et des exemples d’applications :</span><span class="sxs-lookup"><span data-stu-id="ff8c5-106">Related code snippets and sample apps:</span></span>

- [<span data-ttu-id="ff8c5-107">Exchange 2013 : Créer un agent de transport de journalisation de bande passante</span><span class="sxs-lookup"><span data-stu-id="ff8c5-107">Exchange 2013: Build a bandwidth logging transport agent</span></span>](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
<span data-ttu-id="ff8c5-108">Les classes [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) et [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) sont les classes de base pour les agents de transport sont conçues pour s’exécuter sur le service de transport sur un serveur de boîtes aux lettres de Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ff8c5-108">The [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) and [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) classes are the base classes for transport agents that are designed to run on the transport service on an Exchange Server 2013 Mailbox server.</span></span> <span data-ttu-id="ff8c5-109">La classe [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) fournit les événements répertoriés dans le tableau suivant pour laquelle vous pouvez implémenter des gestionnaires dans votre RoutingAgent l’agent de transport.</span><span class="sxs-lookup"><span data-stu-id="ff8c5-109">The [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) class provides the events listed in the following table for which you might implement handlers in your RoutingAgent transport agent.</span></span> 
  
<span data-ttu-id="ff8c5-110">**Le tableau 1. Événements de la classe RoutingAgent**</span><span class="sxs-lookup"><span data-stu-id="ff8c5-110">**Table 1. RoutingAgent class events**</span></span>

|<span data-ttu-id="ff8c5-111">**Événement**</span><span class="sxs-lookup"><span data-stu-id="ff8c5-111">**Event**</span></span>|<span data-ttu-id="ff8c5-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ff8c5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff8c5-113">OnCategorizedMessage</span><span class="sxs-lookup"><span data-stu-id="ff8c5-113">OnCategorizedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |<span data-ttu-id="ff8c5-114">Cet événement se produit une fois que le serveur effectue la conversion de contenu, si cela est nécessaire.</span><span class="sxs-lookup"><span data-stu-id="ff8c5-114">Occurs after the server performs content conversion, if it is required.</span></span>  <br/> |
|[<span data-ttu-id="ff8c5-115">OnResolvedMessage</span><span class="sxs-lookup"><span data-stu-id="ff8c5-115">OnResolvedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |<span data-ttu-id="ff8c5-116">Se produit une fois que tous les destinataires du message ont été résolus et avant de routage est déterminé.</span><span class="sxs-lookup"><span data-stu-id="ff8c5-116">Occurs after all the recipients of the message have been resolved and before routing is determined.</span></span>  <br/> |
|[<span data-ttu-id="ff8c5-117">OnRoutedMessage</span><span class="sxs-lookup"><span data-stu-id="ff8c5-117">OnRoutedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |<span data-ttu-id="ff8c5-118">Cet événement se produit une fois que le serveur achemine le message vers le tronçon suivant et effectue la conversion de contenu, si nécessaire.</span><span class="sxs-lookup"><span data-stu-id="ff8c5-118">Occurs after the server routes the message to the next hop and performs content conversion, if required.</span></span> <span data-ttu-id="ff8c5-119">Le serveur peut utiliser plus de ressources pour traiter chaque message dans l’événement [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) que l’événement [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) , car le serveur effectuer une conversion de contenu nécessaire et déterminer le tronçon suivant dans l’itinéraire pour le message avant d’exécuter le code dans le Gestionnaire d’événements [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ff8c5-119">The server might use more resources to process each message in the [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) event than the [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) event because the server will perform any necessary content conversion and determine the next hop in the route for the message before it executes the code in the [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) event handler.</span></span>  <br/> |
|[<span data-ttu-id="ff8c5-120">OnSubmittedMessage</span><span class="sxs-lookup"><span data-stu-id="ff8c5-120">OnSubmittedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |<span data-ttu-id="ff8c5-121">Cet événement se produit une fois que le message est retiré de la file d’attente d’envoi.</span><span class="sxs-lookup"><span data-stu-id="ff8c5-121">Occurs after the message is taken off the submit queue.</span></span> <span data-ttu-id="ff8c5-122">Utilisez l’événement [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) si l’agent de transport RoutingAgent ne requiert pas de conversion de contenu, destinataires résolus ou des données de routage.</span><span class="sxs-lookup"><span data-stu-id="ff8c5-122">Use the [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) event if your RoutingAgent transport agent does not require content conversion, resolved recipients, or routing data.</span></span>  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a><span data-ttu-id="ff8c5-123">Création d’un agent de transport RoutingAgent personnalisé</span><span class="sxs-lookup"><span data-stu-id="ff8c5-123">Creating a custom RoutingAgent transport agent</span></span>

<span data-ttu-id="ff8c5-124">La procédure suivante explique comment créer un agent de transport RoutingAgent personnalisé.</span><span class="sxs-lookup"><span data-stu-id="ff8c5-124">The following procedure describes how to create a custom RoutingAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="ff8c5-125">Pour créer l’agent de transport</span><span class="sxs-lookup"><span data-stu-id="ff8c5-125">To create the transport agent</span></span>

1. <span data-ttu-id="ff8c5-126">Ajoutez des références aux espaces de noms.</span><span class="sxs-lookup"><span data-stu-id="ff8c5-126">Add references to the namespaces.</span></span>
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   <span data-ttu-id="ff8c5-127">Vous trouverez ces espaces de noms sur votre serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff8c5-127">You can find these namespaces on your Exchange server.</span></span> <span data-ttu-id="ff8c5-128">En ajoutant une référence à ces espaces de noms, vous devez accéder aux membres [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) ainsi que d’autres classes utilisées dans le [Exchange 2013 : créer un agent de transport de journalisation de bande passante](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) exemple.</span><span class="sxs-lookup"><span data-stu-id="ff8c5-128">By adding a reference to these namespaces, you will have access to the [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) members as well as other classes used in the [Exchange 2013: Build a bandwidth logging transport agent](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) sample.</span></span> 
    
2. <span data-ttu-id="ff8c5-129">Implémenter la classe dérivée de la classe [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ff8c5-129">Implement the derived class for the [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) class.</span></span> 
    
   ```cs
      public class BandwidthLoggerFactory : RoutingAgentFactory
      {
          public override RoutingAgent CreateAgent(SmtpServer server)
          {
              return new BandwidthLogger(server);
          }
      }
  
   ```

   <span data-ttu-id="ff8c5-130">Ce code instancie la classe dérivée et substituer la méthode **CreateAgent** pour créer une instance de votre nouvel agent personnalisé.</span><span class="sxs-lookup"><span data-stu-id="ff8c5-130">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> <span data-ttu-id="ff8c5-131">Méthodes supplémentaires, telles que **Close**, peuvent également être remplacés dans cette classe pour exécuter du code personnalisé.</span><span class="sxs-lookup"><span data-stu-id="ff8c5-131">Additional methods, such as **Close**, can also be overridden in this class to execute custom code.</span></span> 
    
3. <span data-ttu-id="ff8c5-132">Définir votre agent.</span><span class="sxs-lookup"><span data-stu-id="ff8c5-132">Define your agent.</span></span>
    
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

   <span data-ttu-id="ff8c5-133">Une fois que vous définissez votre classe agent, vous pouvez vous ajouter des fonctionnalités personnalisées.</span><span class="sxs-lookup"><span data-stu-id="ff8c5-133">After you define your agent class, you can add you custom functionality.</span></span> <span data-ttu-id="ff8c5-134">Dans cet exemple, les deux événements [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) et [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)sont redirigés vers vos gestionnaires d’événements personnalisés.</span><span class="sxs-lookup"><span data-stu-id="ff8c5-134">In this example, the two events [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) and [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)are redirected to your custom event handlers.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="ff8c5-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ff8c5-135">See also</span></span>

- [<span data-ttu-id="ff8c5-136">Concepts de l’agent d’Exchange 2013 de transport</span><span class="sxs-lookup"><span data-stu-id="ff8c5-136">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)    
- [<span data-ttu-id="ff8c5-137">Référence de l’agent de transport pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="ff8c5-137">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)    
- [<span data-ttu-id="ff8c5-138">RoutingAgentFactory</span><span class="sxs-lookup"><span data-stu-id="ff8c5-138">RoutingAgentFactory</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [<span data-ttu-id="ff8c5-139">RoutingAgent</span><span class="sxs-lookup"><span data-stu-id="ff8c5-139">RoutingAgent</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

