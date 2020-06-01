---
title: Création d’un agent de transport SmtpReceiveAgent pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cdc7c462-74a7-49d6-95b2-155d783840e9
description: Découvrez comment créer un agent de transport SmtpReceiveAgent personnalisé à utiliser avec Exchange 2013.
ms.openlocfilehash: 5ba021d02849ffc7e125029f0fd18ebf14c3f8da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459138"
---
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="79de3-103">Création d’un agent de transport SmtpReceiveAgent pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="79de3-103">Create an SmtpReceiveAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="79de3-104">Découvrez comment créer un agent de transport SmtpReceiveAgent personnalisé à utiliser avec Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="79de3-104">Find out how to create a custom SmtpReceiveAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="79de3-105">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="79de3-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="79de3-106">Extraits de code et exemples d’applications connexes :</span><span class="sxs-lookup"><span data-stu-id="79de3-106">Related code snippets and sample apps:</span></span>

- [<span data-ttu-id="79de3-107">Exchange 2013 : création d’un agent de transport de conversion corporelle</span><span class="sxs-lookup"><span data-stu-id="79de3-107">Exchange 2013: Build a body conversion transport agent</span></span>](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
<span data-ttu-id="79de3-108">Les classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) et [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) vous permettent d’étendre le comportement du service de transport frontal sur un serveur d’accès au client ou le service de transport sur un serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="79de3-108">The [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes enable you to extend the behavior of the Front End Transport service on a Client Access Server or the Transport service on a Mailbox server.</span></span> <span data-ttu-id="79de3-109">Vous pouvez utiliser ces classes pour implémenter des agents de transport qui sont conçus pour répondre aux messages au fur et à mesure qu’ils arrivent dans votre organisation.</span><span class="sxs-lookup"><span data-stu-id="79de3-109">You can use these classes to implement transport agents that are designed to respond to messages as they come into your organization.</span></span> 
  
<span data-ttu-id="79de3-110">Les classes [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) et [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) incluent les événements présentés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="79de3-110">The [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes include the events listed in the following table.</span></span> 
  
<span data-ttu-id="79de3-111">**Tableau 1. Événements de classe SmtpReceiveAgent**</span><span class="sxs-lookup"><span data-stu-id="79de3-111">**Table 1. SmtpReceiveAgent class events**</span></span>

|<span data-ttu-id="79de3-112">**Event**</span><span class="sxs-lookup"><span data-stu-id="79de3-112">**Event**</span></span>|<span data-ttu-id="79de3-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="79de3-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79de3-114">OnAuthCommand</span><span class="sxs-lookup"><span data-stu-id="79de3-114">OnAuthCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnAuthCommand.aspx) <br/> |<span data-ttu-id="79de3-115">À utiliser lorsque votre agent requiert des informations fournies uniquement dans la commande SMTP **auth** , comme un agent qui accepte ou rejette les tentatives de remise d’un message en fonction du type de méthode d’authentification utilisée.</span><span class="sxs-lookup"><span data-stu-id="79de3-115">Use when your agent requires information that is provided only in the SMTP **AUTH** command, such as an agent that accepts or rejects attempts to deliver a message based on the type of authentication method used.</span></span>  <br/> |
|[<span data-ttu-id="79de3-116">OnConnect</span><span class="sxs-lookup"><span data-stu-id="79de3-116">OnConnect</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnConnect.aspx) <br/> |<span data-ttu-id="79de3-117">À utiliser lorsque votre agent nécessite des informations fournies uniquement lorsqu’une connexion est ouverte via SMTP vers le service de transport frontal, tel qu’un agent qui effectue une action basée sur l’adresse ou le domaine du serveur SMTP distant.</span><span class="sxs-lookup"><span data-stu-id="79de3-117">Use when your agent requires information that is provided only when a connection is opened via SMTP to the Front End Transport service, such as an agent that performs an action based on the address or domain of the remote SMTP server.</span></span>  <br/> |
|[<span data-ttu-id="79de3-118">OnDataCommand</span><span class="sxs-lookup"><span data-stu-id="79de3-118">OnDataCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDataCommand.aspx) <br/> |<span data-ttu-id="79de3-119">Utilisez cet événement lorsque votre agent requiert des informations fournies dans la commande de **données** SMTP.</span><span class="sxs-lookup"><span data-stu-id="79de3-119">Use this event when your agent requires information that is provided in the SMTP **DATA** command.</span></span>  <br/> |
|[<span data-ttu-id="79de3-120">OnDisconnect</span><span class="sxs-lookup"><span data-stu-id="79de3-120">OnDisconnect</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDisconnect.aspx) <br/> |<span data-ttu-id="79de3-121">À utiliser lorsque votre agent requiert des informations qui sont disponibles au moment de la déconnexion, telles que la date et l’heure actuelles, afin d’effectuer des calculs de temps.</span><span class="sxs-lookup"><span data-stu-id="79de3-121">Use when your agent requires information that is available at the time of disconnection, such as the current date and time, in order to perform time calculations.</span></span>  <br/> |
|[<span data-ttu-id="79de3-122">OnEhloCommand</span><span class="sxs-lookup"><span data-stu-id="79de3-122">OnEhloCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEhloCommand.aspx) <br/> |<span data-ttu-id="79de3-123">À utiliser lorsque votre agent requiert des informations fournies dans la commande SMTP **EHLO** ; par exemple, si votre agent accepte ou rejette les messages en fonction de l’identité fournie dans la commande **EHLO** .</span><span class="sxs-lookup"><span data-stu-id="79de3-123">Use when your agent requires information that is provided in the SMTP **EHLO** command; for example, if your agent accepts or rejects messages based on the identity provided in the **EHLO** command.</span></span>  <br/> |
|[<span data-ttu-id="79de3-124">OnEndOfAuthentication</span><span class="sxs-lookup"><span data-stu-id="79de3-124">OnEndOfAuthentication</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfAuthentication.aspx) <br/> |<span data-ttu-id="79de3-125">À utiliser lorsque votre agent requiert des informations qui sont disponibles après que le serveur distant a terminé le processus d’authentification ; par exemple, pour un agent qui effectue une action sur un message en fonction des informations d’authentification fournies par le serveur ou le client SMTP distant.</span><span class="sxs-lookup"><span data-stu-id="79de3-125">Use when your agent requires information that is available after the remote server completes the authentication process; for example, for an agent that performs an action on a message based on the authentication information provided by the remote SMTP server or client.</span></span>  <br/> |
|[<span data-ttu-id="79de3-126">OnEndOfData</span><span class="sxs-lookup"><span data-stu-id="79de3-126">OnEndOfData</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) <br/> |<span data-ttu-id="79de3-127">À utiliser lorsque votre agent doit effectuer une action basée sur les données disponibles dans le message.</span><span class="sxs-lookup"><span data-stu-id="79de3-127">Use when your agent must perform an action based on data that is available in the message.</span></span> <span data-ttu-id="79de3-128">Cet événement ne se déclenche pas sur le service de transport frontal.</span><span class="sxs-lookup"><span data-stu-id="79de3-128">This event will not fire on the Front End Transport service.</span></span> <span data-ttu-id="79de3-129">Si votre agent de transport doit utiliser cet événement, vous devez l’installer sur un serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="79de3-129">If your transport agent has to use this event, you have to install it on a Mailbox server.</span></span>  <br/> |
|[<span data-ttu-id="79de3-130">OnEndOfHeaders</span><span class="sxs-lookup"><span data-stu-id="79de3-130">OnEndOfHeaders</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) <br/> |<span data-ttu-id="79de3-131">À utiliser lorsque votre agent doit effectuer une action basée sur les informations disponibles dans les en-têtes du message envoyé.</span><span class="sxs-lookup"><span data-stu-id="79de3-131">Use when your agent must perform an action based on information that is available in the headers of the submitted message.</span></span>  <br/> |
   
## <a name="creating-a-custom-smtpreceiveagent-transport-agent"></a><span data-ttu-id="79de3-132">Création d’un agent de transport SmtpReceiveAgent personnalisé</span><span class="sxs-lookup"><span data-stu-id="79de3-132">Creating a custom SmtpReceiveAgent transport agent</span></span>

<span data-ttu-id="79de3-133">La procédure suivante décrit comment créer un agent de transport SmtpReceiveAgent personnalisé.</span><span class="sxs-lookup"><span data-stu-id="79de3-133">The following procedure describes how to create a custom SmtpReceiveAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="79de3-134">Pour créer l’agent de transport</span><span class="sxs-lookup"><span data-stu-id="79de3-134">To create the transport agent</span></span>

1. <span data-ttu-id="79de3-135">Ajoutez des références aux espaces de noms.</span><span class="sxs-lookup"><span data-stu-id="79de3-135">Add references to the namespaces.</span></span>
    
   ```cs
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Smtp;
      using Microsoft.Exchange.Data.Transport.Email;
      using Microsoft.Exchange.Data.TextConverters;
  
   ```

   <span data-ttu-id="79de3-136">Ces espaces de noms se trouvent sur votre serveur Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="79de3-136">You can find these namespaces on your Exchange 2013 server.</span></span> <span data-ttu-id="79de3-137">Lorsque vous ajoutez une référence à ces espaces de noms, vous avez accès aux membres du [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) , ainsi qu’aux autres classes utilisées dans l’exemple [Exchange 2013 : Build a Body conversion agent](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) .</span><span class="sxs-lookup"><span data-stu-id="79de3-137">When you add a reference to these namespaces, you will have access to the [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) members as well as other classes used in the [Exchange 2013: Build a body conversion transport agent](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) sample.</span></span> 
    
2. <span data-ttu-id="79de3-138">Implémentez la classe dérivée pour la classe [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) .</span><span class="sxs-lookup"><span data-stu-id="79de3-138">Implement the derived class for the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) class.</span></span> 
    
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

   <span data-ttu-id="79de3-139">Ce code instancie la classe dérivée et remplace la méthode **CreateAgent** pour créer une instance de votre nouvel agent personnalisé.</span><span class="sxs-lookup"><span data-stu-id="79de3-139">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> 
    
3. <span data-ttu-id="79de3-140">Définissez votre agent.</span><span class="sxs-lookup"><span data-stu-id="79de3-140">Define your agent.</span></span>
    
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

   <span data-ttu-id="79de3-141">Une fois que vous avez défini votre classe d’agent, vous pouvez ajouter vos fonctionnalités personnalisées.</span><span class="sxs-lookup"><span data-stu-id="79de3-141">After you define your agent class, you can add your custom functionality.</span></span> <span data-ttu-id="79de3-142">Dans cet exemple, l’événement [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) est redirigé vers votre gestionnaire d’événements personnalisé.</span><span class="sxs-lookup"><span data-stu-id="79de3-142">In this example, the [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) event is redirected to your custom event handler.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="79de3-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="79de3-143">See also</span></span>

- [<span data-ttu-id="79de3-144">Concepts sur les agents de transport dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="79de3-144">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)    
- [<span data-ttu-id="79de3-145">Référence de l’agent de transport pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="79de3-145">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)    
- [<span data-ttu-id="79de3-146">SmtpReceiveAgentFactory</span><span class="sxs-lookup"><span data-stu-id="79de3-146">SmtpReceiveAgentFactory</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [<span data-ttu-id="79de3-147">SmtpReceiveAgent</span><span class="sxs-lookup"><span data-stu-id="79de3-147">SmtpReceiveAgent</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

