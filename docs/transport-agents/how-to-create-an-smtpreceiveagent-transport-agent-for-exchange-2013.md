---
title: Créer un agent de transport SmtpReceiveAgent pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cdc7c462-74a7-49d6-95b2-155d783840e9
description: Découvrez comment créer un agent de transport SmtpReceiveAgent personnalisé à utiliser avec Exchange 2013.
ms.openlocfilehash: a74d5baae6334c5e17acb6335206964b48f320e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755241"
---
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="3b742-103">Créer un agent de transport SmtpReceiveAgent pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="3b742-103">Create an SmtpReceiveAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="3b742-104">Découvrez comment créer un agent de transport SmtpReceiveAgent personnalisé à utiliser avec Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="3b742-104">Find out how to create a custom SmtpReceiveAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="3b742-105">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="3b742-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="3b742-106">Extraits de code connexes et des exemples d’applications :</span><span class="sxs-lookup"><span data-stu-id="3b742-106">Related code snippets and sample apps:</span></span>

- [<span data-ttu-id="3b742-107">Exchange 2013 : Créer un agent de transport de conversion du corps</span><span class="sxs-lookup"><span data-stu-id="3b742-107">Exchange 2013: Build a body conversion transport agent</span></span>](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
<span data-ttu-id="3b742-108">Les classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) et [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) permettent d’étendre le comportement du service de Transport frontal sur un serveur d’accès au Client ou le service de Transport sur un serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="3b742-108">The [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes enable you to extend the behavior of the Front End Transport service on a Client Access Server or the Transport service on a Mailbox server.</span></span> <span data-ttu-id="3b742-109">Vous pouvez utiliser ces classes pour implémenter des agents de transport qui sont conçus pour répondre aux messages lorsqu’ils sont dans votre organisation.</span><span class="sxs-lookup"><span data-stu-id="3b742-109">You can use these classes to implement transport agents that are designed to respond to messages as they come into your organization.</span></span> 
  
<span data-ttu-id="3b742-110">Les classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) et [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) contiennent les événements répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="3b742-110">The [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes include the events listed in the following table.</span></span> 
  
<span data-ttu-id="3b742-111">**Le tableau 1. Événements de la classe SmtpReceiveAgent**</span><span class="sxs-lookup"><span data-stu-id="3b742-111">**Table 1. SmtpReceiveAgent class events**</span></span>

|<span data-ttu-id="3b742-112">**Événement**</span><span class="sxs-lookup"><span data-stu-id="3b742-112">**Event**</span></span>|<span data-ttu-id="3b742-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="3b742-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b742-114">OnAuthCommand</span><span class="sxs-lookup"><span data-stu-id="3b742-114">OnAuthCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnAuthCommand.aspx) <br/> |<span data-ttu-id="3b742-115">À utiliser lorsque votre agent nécessite des informations qui sont fournies uniquement dans la commande SMTP **AUTH** , comme un agent qui accepte ou rejette tente de remettre un message en fonction du type de méthode d’authentification utilisée.</span><span class="sxs-lookup"><span data-stu-id="3b742-115">Use when your agent requires information that is provided only in the SMTP **AUTH** command, such as an agent that accepts or rejects attempts to deliver a message based on the type of authentication method used.</span></span>  <br/> |
|[<span data-ttu-id="3b742-116">OnConnect</span><span class="sxs-lookup"><span data-stu-id="3b742-116">OnConnect</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnConnect.aspx) <br/> |<span data-ttu-id="3b742-117">À utiliser lorsque votre agent nécessite des informations qui sont fournies uniquement lors de l’ouverture d’une connexion via SMTP pour le service de Transport frontal, comme un agent qui effectue une action en fonction de l’adresse ou le domaine du serveur SMTP distant.</span><span class="sxs-lookup"><span data-stu-id="3b742-117">Use when your agent requires information that is provided only when a connection is opened via SMTP to the Front End Transport service, such as an agent that performs an action based on the address or domain of the remote SMTP server.</span></span>  <br/> |
|[<span data-ttu-id="3b742-118">OnDataCommand</span><span class="sxs-lookup"><span data-stu-id="3b742-118">OnDataCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDataCommand.aspx) <br/> |<span data-ttu-id="3b742-119">Utilisez cet événement lorsque votre agent nécessite des informations fournies dans la commande SMTP **données** .</span><span class="sxs-lookup"><span data-stu-id="3b742-119">Use this event when your agent requires information that is provided in the SMTP **DATA** command.</span></span>  <br/> |
|[<span data-ttu-id="3b742-120">OnDisconnect</span><span class="sxs-lookup"><span data-stu-id="3b742-120">OnDisconnect</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDisconnect.aspx) <br/> |<span data-ttu-id="3b742-121">À utiliser lorsque votre agent nécessite des informations qui sont disponibles au moment de la déconnexion, telles que la date et l’heure, afin d’effectuer des calculs de temps.</span><span class="sxs-lookup"><span data-stu-id="3b742-121">Use when your agent requires information that is available at the time of disconnection, such as the current date and time, in order to perform time calculations.</span></span>  <br/> |
|[<span data-ttu-id="3b742-122">OnEhloCommand</span><span class="sxs-lookup"><span data-stu-id="3b742-122">OnEhloCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEhloCommand.aspx) <br/> |<span data-ttu-id="3b742-123">À utiliser lorsque votre agent nécessite des informations fournies dans la commande SMTP **EHLO** ; par exemple, si votre agent accepte ou rejette les messages en fonction de l’identité fournie dans la commande **EHLO** .</span><span class="sxs-lookup"><span data-stu-id="3b742-123">Use when your agent requires information that is provided in the SMTP **EHLO** command; for example, if your agent accepts or rejects messages based on the identity provided in the **EHLO** command.</span></span>  <br/> |
|[<span data-ttu-id="3b742-124">OnEndOfAuthentication</span><span class="sxs-lookup"><span data-stu-id="3b742-124">OnEndOfAuthentication</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfAuthentication.aspx) <br/> |<span data-ttu-id="3b742-125">À utiliser lorsque votre agent nécessite des informations qui sont disponibles une fois le serveur distant termine le processus d’authentification ; par exemple, pour un agent qui effectue une action sur un message en fonction des informations d’authentification fournies par le client ou le serveur SMTP distant.</span><span class="sxs-lookup"><span data-stu-id="3b742-125">Use when your agent requires information that is available after the remote server completes the authentication process; for example, for an agent that performs an action on a message based on the authentication information provided by the remote SMTP server or client.</span></span>  <br/> |
|[<span data-ttu-id="3b742-126">OnEndOfData</span><span class="sxs-lookup"><span data-stu-id="3b742-126">OnEndOfData</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) <br/> |<span data-ttu-id="3b742-127">À utiliser lorsque votre agent doit effectuer une action en fonction des données qui sont disponibles dans le message.</span><span class="sxs-lookup"><span data-stu-id="3b742-127">Use when your agent must perform an action based on data that is available in the message.</span></span> <span data-ttu-id="3b742-128">Cet événement se déclenche pas sur le service de Transport frontal.</span><span class="sxs-lookup"><span data-stu-id="3b742-128">This event will not fire on the Front End Transport service.</span></span> <span data-ttu-id="3b742-129">Si l’agent de transport a utiliser cet événement, vous devez l’installer sur un serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="3b742-129">If your transport agent has to use this event, you have to install it on a Mailbox server.</span></span>  <br/> |
|[<span data-ttu-id="3b742-130">OnEndOfHeaders</span><span class="sxs-lookup"><span data-stu-id="3b742-130">OnEndOfHeaders</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) <br/> |<span data-ttu-id="3b742-131">À utiliser lorsque votre agent doit effectuer une action en fonction des informations qui est disponibles dans les en-têtes du message envoyé.</span><span class="sxs-lookup"><span data-stu-id="3b742-131">Use when your agent must perform an action based on information that is available in the headers of the submitted message.</span></span>  <br/> |
   
## <a name="creating-a-custom-smtpreceiveagent-transport-agent"></a><span data-ttu-id="3b742-132">Création d’un agent de transport SmtpReceiveAgent personnalisé</span><span class="sxs-lookup"><span data-stu-id="3b742-132">Creating a custom SmtpReceiveAgent transport agent</span></span>

<span data-ttu-id="3b742-133">La procédure suivante explique comment créer un agent de transport SmtpReceiveAgent personnalisé.</span><span class="sxs-lookup"><span data-stu-id="3b742-133">The following procedure describes how to create a custom SmtpReceiveAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="3b742-134">Pour créer l’agent de transport</span><span class="sxs-lookup"><span data-stu-id="3b742-134">To create the transport agent</span></span>

1. <span data-ttu-id="3b742-135">Ajoutez des références aux espaces de noms.</span><span class="sxs-lookup"><span data-stu-id="3b742-135">Add references to the namespaces.</span></span>
    
   ```cs
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Smtp;
      using Microsoft.Exchange.Data.Transport.Email;
      using Microsoft.Exchange.Data.TextConverters;
  
   ```

   <span data-ttu-id="3b742-136">Vous trouverez ces espaces de noms sur votre serveur Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="3b742-136">You can find these namespaces on your Exchange 2013 server.</span></span> <span data-ttu-id="3b742-137">Lorsque vous ajoutez une référence à ces espaces de noms, vous avez accès aux membres [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) ainsi que d’autres classes utilisées dans le [Exchange 2013 : créer un agent de transport de conversion de corps](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) exemple.</span><span class="sxs-lookup"><span data-stu-id="3b742-137">When you add a reference to these namespaces, you will have access to the [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) members as well as other classes used in the [Exchange 2013: Build a body conversion transport agent](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) sample.</span></span> 
    
2. <span data-ttu-id="3b742-138">Implémenter la classe dérivée de la classe [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) .</span><span class="sxs-lookup"><span data-stu-id="3b742-138">Implement the derived class for the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) class.</span></span> 
    
   ```cs
      public class BodyConversionFactory : SmtpReceiveAgentFactory
      {
          /// <summary>
          /// Create a new BodyConversion
          /// </summary>
          /// <param name="server">Exchange server</param>
          /// <returns>A new BodyConversion</returns>
          public override SmtpReceiveAgent CreateAgent(SmtpServer server)
          {
              return new BodyConversion();
          }
      }
  
   ```

   <span data-ttu-id="3b742-139">Ce code instancie la classe dérivée et substituer la méthode **CreateAgent** pour créer une instance de votre nouvel agent personnalisé.</span><span class="sxs-lookup"><span data-stu-id="3b742-139">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> 
    
3. <span data-ttu-id="3b742-140">Définir votre agent.</span><span class="sxs-lookup"><span data-stu-id="3b742-140">Define your agent.</span></span>
    
   ```cs
     public class BodyConversion : SmtpReceiveAgent
      {
          // Your custom code goes here
          /// <summary>
          /// The constructor registers an end of data event handler.
          /// </summary>
          public BodyConversion()
          {
              Debug.WriteLine("[BodyConversion] Agent constructor");
              this.OnEndOfData += new EndOfDataEventHandler(this.OnEndOfDataHandler);
          }
      }
  
   ```

   <span data-ttu-id="3b742-141">Une fois que vous définissez votre classe agent, vous pouvez ajouter des fonctionnalités personnalisées.</span><span class="sxs-lookup"><span data-stu-id="3b742-141">After you define your agent class, you can add your custom functionality.</span></span> <span data-ttu-id="3b742-142">Dans cet exemple, l’événement [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) est redirigé vers votre gestionnaire d’événements personnalisé.</span><span class="sxs-lookup"><span data-stu-id="3b742-142">In this example, the [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) event is redirected to your custom event handler.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="3b742-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3b742-143">See also</span></span>

- [<span data-ttu-id="3b742-144">Concepts de l’agent d’Exchange 2013 de transport</span><span class="sxs-lookup"><span data-stu-id="3b742-144">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)    
- [<span data-ttu-id="3b742-145">Référence de l’agent de transport pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="3b742-145">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)    
- [<span data-ttu-id="3b742-146">SmtpReceiveAgentFactory</span><span class="sxs-lookup"><span data-stu-id="3b742-146">SmtpReceiveAgentFactory</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [<span data-ttu-id="3b742-147">SmtpReceiveAgent</span><span class="sxs-lookup"><span data-stu-id="3b742-147">SmtpReceiveAgent</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

