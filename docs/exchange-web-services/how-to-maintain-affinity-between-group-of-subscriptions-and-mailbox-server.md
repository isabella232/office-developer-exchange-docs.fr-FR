---
title: Conserver l’affinité entre un groupe d'abonnements et le serveur de boîtes aux lettres dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 1bda4094-88c3-4f61-9219-6ee70f6e81cf
description: Découvrez comment maintenir l’affinité entre un groupe d’abonnements et le serveur de boîtes aux lettres.
localization_priority: Priority
ms.openlocfilehash: 1618216cf69e08b2ae774264e0910856a59851af
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44455756"
---
# <a name="maintain-affinity-between-a-group-of-subscriptions-and-the-mailbox-server-in-exchange"></a><span data-ttu-id="6ad50-103">Conserver l’affinité entre un groupe d'abonnements et le serveur de boîtes aux lettres dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6ad50-103">Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>

<span data-ttu-id="6ad50-104">Découvrez comment maintenir l’affinité entre un groupe d’abonnements et le serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6ad50-104">Find out about maintaining the affinity between a group of subscriptions and the Mailbox server.</span></span>
  
<span data-ttu-id="6ad50-105">L’affinité est l’Association d’une séquence de messages de demande et de réponse à un serveur de boîtes aux lettres particulier.</span><span class="sxs-lookup"><span data-stu-id="6ad50-105">Affinity is the association of a sequence of request and response messages with a particular Mailbox server.</span></span> <span data-ttu-id="6ad50-106">Pour la plupart des fonctionnalités dans Exchange, l’affinité est gérée par le serveur.</span><span class="sxs-lookup"><span data-stu-id="6ad50-106">For most functionality in Exchange, affinity is handled by the server.</span></span> <span data-ttu-id="6ad50-107">Toutefois, les notifications sont des exceptions.</span><span class="sxs-lookup"><span data-stu-id="6ad50-107">Notifications, however, are an exception.</span></span> <span data-ttu-id="6ad50-108">Le client est responsable de la maintenance de l’affinité avec le serveur de boîtes aux lettres pour les abonnements aux notifications.</span><span class="sxs-lookup"><span data-stu-id="6ad50-108">The client is responsible for maintaining the affinity with the Mailbox server for notification subscriptions.</span></span> <span data-ttu-id="6ad50-109">Cette affinité active l’équilibreur de charge et les serveurs d’accès au client entre le client et le serveur pour acheminer les abonnements aux notifications et les demandes associées vers le serveur de boîtes aux lettres qui gère l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="6ad50-109">This affinity enables the load balancer and Client Access servers between the client and the server to route notification subscriptions and related requests to the Mailbox server that maintains the subscription.</span></span> <span data-ttu-id="6ad50-110">Sans affinité, la demande peut être acheminée vers un autre serveur de boîtes aux lettres qui n’inclut pas les abonnements du client, ce qui peut entraîner le renvoi d’une erreur [ErrorSubscriptionNotFound](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6ad50-110">Without affinity, the request might get routed to a different Mailbox server that does not include the client's subscriptions, which can cause an [ErrorSubscriptionNotFound](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) error to be returned.</span></span> 
  
## <a name="how-is-affinity-maintained"></a><span data-ttu-id="6ad50-111">Comment l’affinité est-elle conservée ?</span><span class="sxs-lookup"><span data-stu-id="6ad50-111">How is affinity maintained?</span></span>
<span data-ttu-id="6ad50-112"><a name="bk_howmaintained"> </a></span><span class="sxs-lookup"><span data-stu-id="6ad50-112"><a name="bk_howmaintained"> </a></span></span>

<span data-ttu-id="6ad50-113">L’affinité dans Exchange est basée sur les cookies.</span><span class="sxs-lookup"><span data-stu-id="6ad50-113">Affinity in Exchange is cookie based.</span></span> <span data-ttu-id="6ad50-114">Le client déclenche la création du cookie en incluant des en-têtes spécifiques dans la demande d’abonnement, puis la réponse de l’abonnement contient le cookie.</span><span class="sxs-lookup"><span data-stu-id="6ad50-114">The client triggers the creation of the cookie by including specific headers in the subscription request, and then the subscription response contains the cookie.</span></span> <span data-ttu-id="6ad50-115">Le client envoie ensuite ce cookie dans les demandes suivantes pour s’assurer que la demande est routée vers le serveur de boîtes aux lettres approprié.</span><span class="sxs-lookup"><span data-stu-id="6ad50-115">The client then sends that cookie in subsequent requests to ensure that the request is routed to the right Mailbox server.</span></span>
  
<span data-ttu-id="6ad50-116">Plus spécifiquement, l’affinité dans Exchange est gérée par les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="6ad50-116">More specifically, affinity in Exchange is handled by the following:</span></span> 
  
- <span data-ttu-id="6ad50-117">X-AnchorMailbox : en-tête HTTP inclus dans la demande d’abonnement initiale.</span><span class="sxs-lookup"><span data-stu-id="6ad50-117">X-AnchorMailbox — An HTTP header that is included in the initial subscription request.</span></span> <span data-ttu-id="6ad50-118">Il identifie la première boîte aux lettres d’un groupe de boîtes aux lettres qui partagent l’affinité avec le même serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6ad50-118">It identifies the first mailbox in a group of mailboxes that share affinity with the same Mailbox server.</span></span>
    
- <span data-ttu-id="6ad50-119">X-PreferServerAffinity : en-tête HTTP inclus dans la demande d’abonnement initiale avec l’en-tête X-AnchorMailbox et est défini sur true pour indiquer que le client demande que l’affinité soit maintenue avec le serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6ad50-119">X-PreferServerAffinity — An HTTP header that is included in the initial subscription request with the X-AnchorMailbox header and is set to true to indicate that the client is requesting that affinity be maintained with the Mailbox server.</span></span>
    
- <span data-ttu-id="6ad50-120">X-BackEndOverrideCookie — cookie inclus dans la réponse d’abonnement initiale et contenant un cookie que l’équilibreur de charge et le serveur d’accès au client utilisent pour acheminer les demandes ultérieures vers le même serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6ad50-120">X-BackEndOverrideCookie — A cookie that is included in the initial subscription response and contains a cookie that the load balancer and Client Access server use to route subsequent requests to the same Mailbox server.</span></span>
    
## <a name="how-do-i-maintain-affinity-by-using-the-ews-managed-api-or-ews"></a><span data-ttu-id="6ad50-121">Comment puis-je conserver les affinités à l’aide de l’API managée EWS ou EWS ?</span><span class="sxs-lookup"><span data-stu-id="6ad50-121">How do I maintain affinity by using the EWS Managed API or EWS?</span></span>
<span data-ttu-id="6ad50-122"><a name="bk_howdoimaintain"> </a></span><span class="sxs-lookup"><span data-stu-id="6ad50-122"><a name="bk_howdoimaintain"> </a></span></span>

<span data-ttu-id="6ad50-123">Vous pouvez utiliser les mêmes étapes pour conserver l’affinité pour les abonnements à plusieurs boîtes aux lettres et leurs serveurs de boîtes aux lettres, que vous utilisiez des notifications de diffusion en continu, d’extraction ou de transmission, et que vous cibliez ou non un serveur Exchange local ou Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="6ad50-123">You can use the same steps to maintain affinity for multiple mailbox subscriptions and their Mailbox servers, regardless of whether you are using streaming, pull, or push notifications, and regardless of whether you're targeting an Exchange on-premises server or Exchange Online.</span></span>
  
1. <span data-ttu-id="6ad50-124">Pour chaque boîte aux lettres, [appelez Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) et obtenez les paramètres utilisateur GroupingInformation et ExternalEwsUrl.</span><span class="sxs-lookup"><span data-stu-id="6ad50-124">For each mailbox, [call Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) and get the GroupingInformation and ExternalEwsUrl user settings.</span></span> <span data-ttu-id="6ad50-125">Pour la découverte automatique SOAP, vous utilisez l’élément [Setting](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) et pour la découverte automatique POX, vous utilisez l’élément [GroupingInformation](https://msdn.microsoft.com/library/2d8a007f-d79c-43c8-90e3-2c6d883f3a7c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6ad50-125">For SOAP Autodiscover, you use the [Setting](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) element, and for POX Autodiscover, you use the [GroupingInformation](https://msdn.microsoft.com/library/2d8a007f-d79c-43c8-90e3-2c6d883f3a7c%28Office.15%29.aspx) element.</span></span> 
    
2. <span data-ttu-id="6ad50-126">En utilisant les paramètres GroupingInformation et ExternalEwsUrl des réponses de découverte automatique, placez les boîtes aux lettres avec la même valeur concaténée ExternalEwsUrl et GroupingInformation dans le même groupe.</span><span class="sxs-lookup"><span data-stu-id="6ad50-126">Using the GroupingInformation and ExternalEwsUrl settings from the Autodiscover responses, place mailboxes with the same ExternalEwsUrl and GroupingInformation concatenated value in the same group.</span></span> <span data-ttu-id="6ad50-127">Si des groupes possèdent plus de 200 boîtes aux lettres, Rompez-les davantage afin que chaque groupe ne contienne pas plus de 200 boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6ad50-127">If any groups have more than 200 mailboxes, break the groups down further so that each group has no more than 200 mailboxes.</span></span>
    
3. <span data-ttu-id="6ad50-128">Créez et utilisez un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=EXCHG.80%29.aspx) pour le reste de la procédure.</span><span class="sxs-lookup"><span data-stu-id="6ad50-128">Create and use one [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=EXCHG.80%29.aspx) object for the rest of the procedure.</span></span> <span data-ttu-id="6ad50-129">Lorsque vous utilisez le même objet **ExchangeService** , les cookies et les en-têtes (lorsqu’ils sont définis) sont automatiquement gérés.</span><span class="sxs-lookup"><span data-stu-id="6ad50-129">When you use the same **ExchangeService** object, cookies and headers (when they are set) are automatically maintained.</span></span> <span data-ttu-id="6ad50-130">Notez que si vous n’avez pas l’intention de regrouper des abonnements de diffusion en continu dans une seule connexion, vous pouvez créer un objet **ExchangeService** différent pour chaque utilisateur emprunté.</span><span class="sxs-lookup"><span data-stu-id="6ad50-130">Note that if you do not intend to group streaming subscriptions into a single connection, you are free to create a different **ExchangeService** object for each impersonated user.</span></span> 
    
4. <span data-ttu-id="6ad50-131">[Envoyer une](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) demande d’abonnement pour l’utilisateur dont le nom d’utilisateur apparaît en premier lorsque tous les utilisateurs du groupe sont triés par ordre alphabétique (nous faisons référence à cet utilisateur comme l’utilisateur de la boîte aux lettres d’ancrage).</span><span class="sxs-lookup"><span data-stu-id="6ad50-131">[Send a subscription](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) request for the user whose user name appears first when all users in the group are sorted alphabetically (we'll refer to this user as the anchor mailbox user).</span></span> <span data-ttu-id="6ad50-132">Procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="6ad50-132">Do the following:</span></span> 
    
  - <span data-ttu-id="6ad50-133">Incluez l’en-tête X-AnchorMailbox avec une valeur définie sur l’adresse SMTP de l’utilisateur de la boîte aux lettres d’ancrage.</span><span class="sxs-lookup"><span data-stu-id="6ad50-133">Include the X-AnchorMailbox header with a value set to the SMTP address of the anchor mailbox user.</span></span>
    
  - <span data-ttu-id="6ad50-134">Incluez l’en-tête X-PreferServerAffinity avec une valeur définie sur true.</span><span class="sxs-lookup"><span data-stu-id="6ad50-134">Include the X-PreferServerAffinity header with a value set to true.</span></span>
    
  - <span data-ttu-id="6ad50-135">Utilisez le rôle [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) (type [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ).</span><span class="sxs-lookup"><span data-stu-id="6ad50-135">Use the [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) role (the [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) type).</span></span> 
    
5. <span data-ttu-id="6ad50-136">Dans la réponse de l’abonnement, obtenez la valeur X-BackEndOverrideCookie.</span><span class="sxs-lookup"><span data-stu-id="6ad50-136">In the subscription response, get the X-BackEndOverrideCookie value.</span></span> <span data-ttu-id="6ad50-137">Incluez cette valeur dans chacune des demandes d’abonnements suivantes pour les utilisateurs de ce groupe.</span><span class="sxs-lookup"><span data-stu-id="6ad50-137">Include this value in each of the subsequent subscription requests for users in this group.</span></span>
    
6. <span data-ttu-id="6ad50-138">Pour chaque utilisateur supplémentaire dans le groupe, envoyez une demande d’abonnement et procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="6ad50-138">For each additional user in the group, send a subscription request and do the following:</span></span>
    
  - <span data-ttu-id="6ad50-139">Incluez l’en-tête X-AnchorMailbox avec une valeur définie sur l’adresse SMTP de l’utilisateur de la boîte aux lettres d’ancrage du groupe.</span><span class="sxs-lookup"><span data-stu-id="6ad50-139">Include the X-AnchorMailbox header with a value set to the SMTP address of the anchor mailbox user for the group.</span></span>
    
  - <span data-ttu-id="6ad50-140">Incluez l’en-tête X-PreferServerAffinity avec une valeur définie sur true.</span><span class="sxs-lookup"><span data-stu-id="6ad50-140">Include the X-PreferServerAffinity header with a value set to true.</span></span>
    
  - <span data-ttu-id="6ad50-141">Incluez la X-BackEndOverrideCookie qui a été renvoyée dans la réponse de l’utilisateur de la boîte aux lettres d’ancrage.</span><span class="sxs-lookup"><span data-stu-id="6ad50-141">Include the X-BackEndOverrideCookie that was returned in the anchor mailbox user's subscription response.</span></span>
    
  - <span data-ttu-id="6ad50-142">Utilisez le rôle [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) (type [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ).</span><span class="sxs-lookup"><span data-stu-id="6ad50-142">Use the [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) role (the [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) type).</span></span> 
    
    <span data-ttu-id="6ad50-143">Notez que le serveur utilise les valeurs X-PreferServerAffinity et X-BackendOverrideCookie pour effectuer le routage vers le serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6ad50-143">Note that the server uses the X-PreferServerAffinity and X-BackendOverrideCookie values together to perform the routing to the mailbox server.</span></span> <span data-ttu-id="6ad50-144">L’en-tête X-AnchorMailbox est également requis, mais est ignoré par le serveur si les deux autres valeurs sont valides.</span><span class="sxs-lookup"><span data-stu-id="6ad50-144">The X-AnchorMailbox header is also required, but is ignored by the server if the other two values are valid.</span></span> <span data-ttu-id="6ad50-145">Si X-AnchorMailbox et X-PreferServerAffinity sont dans une requête et que X-BackendOverrideCookie n’est pas inclus, la valeur X-AnchorMailbox est utilisée pour acheminer les demandes.</span><span class="sxs-lookup"><span data-stu-id="6ad50-145">If X-AnchorMailbox and X-PreferServerAffinity are in a request and X-BackendOverrideCookie is not included, the X-AnchorMailbox value is used to route the requests.</span></span>
    
    <span data-ttu-id="6ad50-146">Étant donné que les valeurs X-PreferServerAffinity et X-BackendOverrideCookie effectuent le routage, si la boîte aux lettres d’ancrage ne passe pas à un autre groupe ou serveur, la logique ne change pas, car X-BackendOverrideCookie achemine la demande vers le serveur approprié pour le groupe.</span><span class="sxs-lookup"><span data-stu-id="6ad50-146">Because the X-PreferServerAffinity and X-BackendOverrideCookie values perform the routing, if the anchor mailbox ever moves to another group or server, the logic does not change because the X-BackendOverrideCookie will route the request to the correct server for the group.</span></span>
    
7. <span data-ttu-id="6ad50-147">Envoyez une seule demande [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) ou [GetEvents](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) pour le groupe, puis procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="6ad50-147">Send a single [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) or [GetEvents](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) requests for the group, and do the following:</span></span> 
    
  - <span data-ttu-id="6ad50-148">Incluez les valeurs [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) renvoyées dans chacune des réponses d’abonnement individuelles pour les boîtes aux lettres du groupe.</span><span class="sxs-lookup"><span data-stu-id="6ad50-148">Include the [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) values returned in each of the individual subscription responses for mailboxes in the group.</span></span> 
    
  - <span data-ttu-id="6ad50-149">Si plus de 200 abonnements existent pour le groupe, créez plusieurs demandes.</span><span class="sxs-lookup"><span data-stu-id="6ad50-149">If more than 200 subscriptions exist for the group, create multiple requests.</span></span> <span data-ttu-id="6ad50-150">Le nombre maximal de valeurs [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) à inclure dans une demande est de 200.</span><span class="sxs-lookup"><span data-stu-id="6ad50-150">The maximum number of [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) values to include in a request is 200.</span></span> 
    
  - <span data-ttu-id="6ad50-151">Si vous avez besoin de plus de connexions que celles disponibles pour la boîte aux lettres cible, utilisez le compte de service pour emprunter l’identité de la boîte aux lettres d’ancrage du groupe ; Sinon, n’utilisez pas l’emprunt d’identité.</span><span class="sxs-lookup"><span data-stu-id="6ad50-151">If you need more connections than are available to the target mailbox, use the service account to impersonate the anchor mailbox for the group; otherwise, do not use impersonation.</span></span> <span data-ttu-id="6ad50-152">Idéalement, vous souhaitez emprunter l’identité d’une boîte aux lettres unique par demande [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) ou [GetEvents](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) afin de ne pas rencontrer de limites de limitation.</span><span class="sxs-lookup"><span data-stu-id="6ad50-152">Ideally, you want to impersonate a unique mailbox per [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) or [GetEvents](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) request so that you never encounter throttling limits.</span></span> 
    
  - <span data-ttu-id="6ad50-153">Utilisez ApplicationImpersonation si vous avez besoin de [plus de connexions que celles disponibles pour la boîte aux lettres cible](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling); Sinon, n’utilisez pas ApplicationImpersonation.</span><span class="sxs-lookup"><span data-stu-id="6ad50-153">Use ApplicationImpersonation if you need [more connections than are available to the target mailbox](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling); otherwise, do not use ApplicationImpersonation.</span></span>
    
  - <span data-ttu-id="6ad50-154">Incluez l’en-tête X-PreferServerAffinity et définissez-le sur true.</span><span class="sxs-lookup"><span data-stu-id="6ad50-154">Include the X-PreferServerAffinity header and set it to true.</span></span> <span data-ttu-id="6ad50-155">Cette valeur est incluse automatiquement si vous utilisez l’objet **ExchangeService** que vous avez créé à l’étape 2.</span><span class="sxs-lookup"><span data-stu-id="6ad50-155">This value is automatically included if you are using the **ExchangeService** object that you created in step 2.</span></span> 
    
  - <span data-ttu-id="6ad50-156">Incluez X-BackEndOverrideCookie pour le groupe (X-BackEndOverrideCookie qui a été renvoyé dans la réponse d’abonnement de l’utilisateur de la boîte aux lettres d’ancrage).</span><span class="sxs-lookup"><span data-stu-id="6ad50-156">Include the X-BackEndOverrideCookie for the group (the X-BackEndOverrideCookie that was returned in the anchor mailbox user's subscription response).</span></span> <span data-ttu-id="6ad50-157">Cette valeur est incluse automatiquement si vous utilisez l’objet **ExchangeService** que vous avez créé à l’étape 2.</span><span class="sxs-lookup"><span data-stu-id="6ad50-157">This value is automatically included if you are using the **ExchangeService** object that you created in step 2.</span></span> 
    
8. <span data-ttu-id="6ad50-158">Transmettez les événements renvoyés à un thread distinct pour traitement.</span><span class="sxs-lookup"><span data-stu-id="6ad50-158">Pass the returned events to a separate thread for processing.</span></span>
    
## <a name="what-throttling-values-do-i-need-to-take-into-consideration"></a><span data-ttu-id="6ad50-159">Quelles valeurs de limitation dois-je prendre en considération ?</span><span class="sxs-lookup"><span data-stu-id="6ad50-159">What throttling values do I need to take into consideration?</span></span>
<span data-ttu-id="6ad50-160"><a name="bk_throttling"> </a></span><span class="sxs-lookup"><span data-stu-id="6ad50-160"><a name="bk_throttling"> </a></span></span>

<span data-ttu-id="6ad50-161">Lorsque vous planifiez l’implémentation de vos notifications, vous devez prendre deux valeurs en considération : le nombre de connexions et le nombre d’abonnements.</span><span class="sxs-lookup"><span data-stu-id="6ad50-161">As you plan your notification implementation, you'll want to take two values into consideration: the number of connections, and the number of subscriptions.</span></span> <span data-ttu-id="6ad50-162">Le tableau suivant répertorie les valeurs par défaut pour chaque paramètre de [limitation](ews-throttling-in-exchange.md) et la façon dont les paramètres sont utilisés.</span><span class="sxs-lookup"><span data-stu-id="6ad50-162">The following table lists the default values for each [throttling](ews-throttling-in-exchange.md) setting and how the settings are used.</span></span> <span data-ttu-id="6ad50-163">Pour chaque valeur, le budget est alloué à la boîte aux lettres cible.</span><span class="sxs-lookup"><span data-stu-id="6ad50-163">For each value, the budget is allocated to the target mailbox.</span></span> <span data-ttu-id="6ad50-164">Pour cette raison, l’utilisation de l’emprunt d’identité pour obtenir des connexions supplémentaires est une étape requise dans de nombreux scénarios.</span><span class="sxs-lookup"><span data-stu-id="6ad50-164">For this reason, using impersonation to gain additional connections is a required step in many scenarios.</span></span> 
  
<span data-ttu-id="6ad50-165">**Tableau 1. Valeurs de limitation par défaut**</span><span class="sxs-lookup"><span data-stu-id="6ad50-165">**Table 1. Default throttling values**</span></span>

|<span data-ttu-id="6ad50-166">**Domaine de réflexion**</span><span class="sxs-lookup"><span data-stu-id="6ad50-166">**Area of consideration**</span></span>|<span data-ttu-id="6ad50-167">**Paramètre de limitation**</span><span class="sxs-lookup"><span data-stu-id="6ad50-167">**Throttling setting**</span></span>|<span data-ttu-id="6ad50-168">**Valeur par défaut**</span><span class="sxs-lookup"><span data-stu-id="6ad50-168">**Default value**</span></span>|<span data-ttu-id="6ad50-169">**Description**</span><span class="sxs-lookup"><span data-stu-id="6ad50-169">**Description**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="6ad50-170">Connexions de diffusion en continu</span><span class="sxs-lookup"><span data-stu-id="6ad50-170">Streaming connections</span></span>  <br/> |<span data-ttu-id="6ad50-171">Limite de blocage par défaut</span><span class="sxs-lookup"><span data-stu-id="6ad50-171">Default hanging connection limit</span></span>  <br/> |<span data-ttu-id="6ad50-172">10 pour Exchange Online</span><span class="sxs-lookup"><span data-stu-id="6ad50-172">10 for Exchange Online</span></span>  <br/> <span data-ttu-id="6ad50-173">3 pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="6ad50-173">3 for Exchange 2013</span></span>  <br/> |<span data-ttu-id="6ad50-174">Nombre maximal de connexions de diffusion en continu simultanées qu’un compte peut ouvrir simultanément sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="6ad50-174">The maximum number of concurrent streaming connections that an account can have open on the server at one time.</span></span> <span data-ttu-id="6ad50-175">Pour travailler dans cette limite, utilisez un compte de service avec le rôle ApplicationImpersonation attribué pour les boîtes aux lettres cibles et empruntez l’identité du premier utilisateur dans chaque groupe d’ID d’abonnement lors de l’obtention d’événements en flux.</span><span class="sxs-lookup"><span data-stu-id="6ad50-175">To work within this limit, use a service account with the ApplicationImpersonation role assigned for the target mailboxes, and impersonate the first user in each subscription ID group when getting streamed events.</span></span>  <br/> |
|<span data-ttu-id="6ad50-176">Connexions d’extraction ou de transmission par émission</span><span class="sxs-lookup"><span data-stu-id="6ad50-176">Pull or push connections</span></span>  <br/> |<span data-ttu-id="6ad50-177">EWSMaxConcurrency</span><span class="sxs-lookup"><span data-stu-id="6ad50-177">EWSMaxConcurrency</span></span>  <br/> |<span data-ttu-id="6ad50-178">vingt</span><span class="sxs-lookup"><span data-stu-id="6ad50-178">27</span></span>  <br/> |<span data-ttu-id="6ad50-179">Nombre maximal de connexions d’extraction ou de transmission simultanées (demandes reçues mais pas encore satisfaites) qu’un compte peut ouvrir simultanément sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="6ad50-179">The maximum number of concurrent pull or push connections (requests that have been received but not yet responded to) that an account can have open on the server at one time.</span></span>  <br/> |
|<span data-ttu-id="6ad50-180">Abonnements</span><span class="sxs-lookup"><span data-stu-id="6ad50-180">Subscriptions</span></span>  <br/> |<span data-ttu-id="6ad50-181">EWSMaxSubscriptions</span><span class="sxs-lookup"><span data-stu-id="6ad50-181">EWSMaxSubscriptions</span></span>  <br/> |<span data-ttu-id="6ad50-182">20 pour Exchange Online</span><span class="sxs-lookup"><span data-stu-id="6ad50-182">20 for Exchange Online</span></span>  <br/> <span data-ttu-id="6ad50-183">5000 pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="6ad50-183">5000 for Exchange 2013</span></span>  <br/> |<span data-ttu-id="6ad50-184">Nombre maximal d’abonnements non expirés qu’un compte peut avoir à la fois.</span><span class="sxs-lookup"><span data-stu-id="6ad50-184">The maximum number of nonexpired subscriptions that an account can have at one time.</span></span> <span data-ttu-id="6ad50-185">Cette valeur est décrémentée lors de la création de l’abonnement sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="6ad50-185">This value is decremented when the subscription is created on the server.</span></span>  <br/> |
   
<span data-ttu-id="6ad50-186">L’exemple suivant montre comment les budgets sont gérés entre n’importe quelle boîte aux lettres cible et le compte de service auquel le rôle [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) est attribué pour les boîtes aux lettres cibles.</span><span class="sxs-lookup"><span data-stu-id="6ad50-186">The following example shows how budgets are handled between any target mailbox and the service account that has the [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) role assigned for the target mailboxes.</span></span> 
  
- <span data-ttu-id="6ad50-187">ServiceAccount1 (SA1) emprunte un grand nombre d’utilisateurs (M1, m2, m3, etc.) et crée des abonnements pour chaque boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6ad50-187">ServiceAccount1 (sa1) impersonates many users (m1, m2, m3, and so on) and creates subscriptions for each mailbox.</span></span> <span data-ttu-id="6ad50-188">Notez que lorsque les abonnements sont créés, le propriétaire de l’abonnement est SA1, donc lorsque SA1 ouvre une connexion avec les abonnements, EWS applique que les abonnements appartiennent à SA1.</span><span class="sxs-lookup"><span data-stu-id="6ad50-188">Note that when the subscriptions are created, the subscription owner is sa1, so when sa1 opens a connection with the subscriptions, EWS enforces that the subscriptions are owned by sa1.</span></span>
    
- <span data-ttu-id="6ad50-189">SA1 peut ouvrir la connexion de l’une des manières suivantes :</span><span class="sxs-lookup"><span data-stu-id="6ad50-189">Sa1 can open the connection in the following ways:</span></span>
    
1. <span data-ttu-id="6ad50-190">Sans emprunt d’identité, la connexion est donc facturée par rapport à SA1.</span><span class="sxs-lookup"><span data-stu-id="6ad50-190">Without impersonation, so the connection is charged against sa1.</span></span>
    
2. <span data-ttu-id="6ad50-191">En empruntant l’identité de l’un des utilisateurs (M1, par exemple) de sorte que la connexion soit facturée par rapport à une copie du budget m1's.</span><span class="sxs-lookup"><span data-stu-id="6ad50-191">By impersonating any of the users — m1 for example — so that the connection is charged against a copy of m1's budget.</span></span> <span data-ttu-id="6ad50-192">(M1 elle-même peut ouvrir dix connexions à l’aide d’Exchange Online, et tous les comptes de service qui empruntent l’identité M1 peuvent ouvrir dix connexions à l’aide du budget copié.)</span><span class="sxs-lookup"><span data-stu-id="6ad50-192">(M1 itself can open ten connections by using Exchange Online, and all service accounts impersonating m1 can open ten connections by using the copied budget.)</span></span>
    
- <span data-ttu-id="6ad50-193">Si la limite de connexion est atteinte, les solutions de contournement suivantes sont disponibles :</span><span class="sxs-lookup"><span data-stu-id="6ad50-193">If the connection limit is hit, the following workarounds are available:</span></span>
    
  - <span data-ttu-id="6ad50-194">Si l’option 1 est utilisée, l’administrateur peut créer plusieurs comptes de service pour emprunter l’identité d’utilisateurs supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="6ad50-194">If option 1 is used, the administrator can create multiple service accounts to impersonate additional users.</span></span>
    
  - <span data-ttu-id="6ad50-195">Si l’option 2 est utilisée, le code peut emprunter l’identité d’un autre utilisateur (m2 par exemple).</span><span class="sxs-lookup"><span data-stu-id="6ad50-195">If option 2 is used, the code can impersonate another user — m2 for example.</span></span>
    
## <a name="example-maintaining-affinity-between-a-group-of-subscriptions-and-the-mailbox-server"></a><span data-ttu-id="6ad50-196">Exemple : conservation de l’affinité entre un groupe d’abonnements et le serveur de boîtes aux lettres</span><span class="sxs-lookup"><span data-stu-id="6ad50-196">Example: Maintaining affinity between a group of subscriptions and the Mailbox server</span></span>
<span data-ttu-id="6ad50-197"><a name="bk_ce"> </a></span><span class="sxs-lookup"><span data-stu-id="6ad50-197"><a name="bk_ce"> </a></span></span>

<span data-ttu-id="6ad50-198">OK, voyons-le en action.</span><span class="sxs-lookup"><span data-stu-id="6ad50-198">Okay, let's see it in action.</span></span> <span data-ttu-id="6ad50-199">L’exemple de code suivant montre comment regrouper des utilisateurs et utiliser les en-têtes X-AnchorMailbox et X-PreferServerAffinity et le cookie X-BackendOverrideCookie pour maintenir l’affinité avec le serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6ad50-199">The following code example shows you how to group users and use the X-AnchorMailbox and X-PreferServerAffinity headers and the X-BackendOverrideCookie cookie to maintain affinity with the Mailbox server.</span></span> <span data-ttu-id="6ad50-200">Étant donné que les en-têtes et le cookie ont une importance essentielle dans la histoire de l’affinité, cet exemple se concentre sur les requêtes et les réponses XML EWS.</span><span class="sxs-lookup"><span data-stu-id="6ad50-200">Because the headers and the cookie are of primary importance in the affinity story, this example focuses on the EWS XML requests and responses.</span></span> <span data-ttu-id="6ad50-201">Pour utiliser l’API managée EWS afin de créer le corps des demandes et des réponses d’abonnement, consultez la rubrique [transmettre des notifications sur les événements de boîte aux lettres à l’aide d’EWS dans Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md) et les [notifications pull sur les événements de boîte aux lettres à l’aide d’EWS dans Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="6ad50-201">To use the EWS Managed API to create the body of the subscription requests and responses, see [Stream notifications about mailbox events by using EWS in Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md) and [Pull notifications about mailbox events by using EWS in Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="6ad50-202">Cette section comprend des étapes supplémentaires en particulier pour conserver l’affinité et ajouter les en-têtes à vos demandes.</span><span class="sxs-lookup"><span data-stu-id="6ad50-202">This section includes additional steps particular to maintaining affinity and adding the headers to your requests.</span></span>
  
<span data-ttu-id="6ad50-203">Cet exemple est doté de quatre utilisateurs : alfred@contoso.com, alisa@contoso.com, ronnie@contoso.com et sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="6ad50-203">This example has four users: alfred@contoso.com, alisa@contoso.com, ronnie@contoso.com, and sadie@contoso.com.</span></span> <span data-ttu-id="6ad50-204">La figure suivante illustre les [paramètres de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) GroupingInformation et ExternalEwsUrl pour les utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="6ad50-204">The following figure shows the GroupingInformation and ExternalEwsUrl [Autodiscover settings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) for the users.</span></span> 
  
<span data-ttu-id="6ad50-205">**Figure 1. Paramètres de découverte automatique utilisés pour regrouper des boîtes aux lettres**</span><span class="sxs-lookup"><span data-stu-id="6ad50-205">**Figure 1. Autodiscover settings used to group mailboxes**</span></span>

![Table illustrant les valeurs GroupingInformation et ExternalEwsUrl pour chacun des utilisateurs.](media/Exchange2013_NotificationAffinityAutoDResults.png)
  
<span data-ttu-id="6ad50-207">À l’aide des paramètres des réponses de découverte automatique, les boîtes aux lettres sont regroupées par la valeur concaténée des paramètres GroupingInformation et ExternalEwsUrl.</span><span class="sxs-lookup"><span data-stu-id="6ad50-207">Using the settings from the Autodiscover responses, the mailboxes are grouped by the concatenated value of the GroupingInformation and ExternalEwsUrl settings.</span></span> <span data-ttu-id="6ad50-208">Dans cet exemple, Alfred et Sadie ont les mêmes valeurs, de sorte qu’elles se trouvent dans un groupe et que Alisa et Ronnie partagent les mêmes valeurs, ils sont donc dans un autre groupe.</span><span class="sxs-lookup"><span data-stu-id="6ad50-208">In this example, Alfred and Sadie have the same values, so they are in one group, and Alisa and Ronnie share the same values, so they are in another group.</span></span>
  
<span data-ttu-id="6ad50-209">**Figure 2. Création de groupes de boîtes aux lettres**</span><span class="sxs-lookup"><span data-stu-id="6ad50-209">**Figure 2. Creating mailbox groups**</span></span>

![Tableau illustrant la création des groupes de boîtes aux lettres à l’aide des paramètres de découverte automatique.](media/Exchange2013_NotificationAffinityGrouping.png)
  
<span data-ttu-id="6ad50-211">Dans le cadre de cet exemple, nous allons nous concentrer sur le groupe A. Nous allons utiliser les mêmes étapes pour le groupe B, mais utiliser une valeur X-AnchorMailbox différente pour ce groupe.</span><span class="sxs-lookup"><span data-stu-id="6ad50-211">For the purpose of this example, we'll focus on Group A. We would use the same steps for group B, but use a different X-AnchorMailbox value for that group.</span></span>
  
<span data-ttu-id="6ad50-212">À l’aide de [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx), créez la demande d’abonnement pour la boîte aux lettres d’ancrage (Alfred@contoso.com), avec l’en-tête x-AnchorMailbox défini sur l’adresse de messagerie et une valeur d’en-tête x-PreferServerAffinity de true.</span><span class="sxs-lookup"><span data-stu-id="6ad50-212">Using [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx), create the subscription request for the anchor mailbox (alfred@contoso.com), with the X-AnchorMailbox header set to the their email address and an X-PreferServerAffinity header value of true.</span></span> <span data-ttu-id="6ad50-213">La définition de ces deux valeurs d’en-tête déclenche le serveur pour créer une X-BackEndOverrideCookie pour la réponse.</span><span class="sxs-lookup"><span data-stu-id="6ad50-213">Setting these two header values will trigger the server to create an X-BackEndOverrideCookie for the response.</span></span>
  
<span data-ttu-id="6ad50-214">Si vous utilisez l’API managée EWS, utilisez la méthode[Add](https://msdn.microsoft.com/library/cy7xta5e) [HttpHeaders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice_members%28v=exchg.80%29.aspx)pour ajouter les deux en-têtes à votre demande d’abonnement, comme illustré.</span><span class="sxs-lookup"><span data-stu-id="6ad50-214">If you're using the EWS Managed API, use the [HttpHeaders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice_members%28v=exchg.80%29.aspx)[Add](https://msdn.microsoft.com/library/cy7xta5e) method to add the two headers to your subscription request, as shown.</span></span> 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", Mailbox.SMTPAddress);
service.HttpHeaders.Add("X-PreferServerAffinity", "true");
```

<span data-ttu-id="6ad50-215">Ainsi, la demande d’abonnement à Alfred se présente comme suit.</span><span class="sxs-lookup"><span data-stu-id="6ad50-215">So Alfred's subscription request looks like this.</span></span>
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>alfred@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:Subscribe>
      <m:StreamingSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox" />
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
        </t:EventTypes>
      </m:StreamingSubscriptionRequest>
    </m:Subscribe>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="6ad50-216">Le message XML suivant est la réponse à la demande d’abonnement à Alfred, qui inclut X-BackEndOverrideCookie.</span><span class="sxs-lookup"><span data-stu-id="6ad50-216">The following XML message is the response to Alfred's subscription request, and it includes the X-BackEndOverrideCookie.</span></span> <span data-ttu-id="6ad50-217">Renvoyez ce cookie pour toutes les demandes suivantes pour les utilisateurs de ce groupe.</span><span class="sxs-lookup"><span data-stu-id="6ad50-217">Resend this cookie for all subsequent requests for users in this group.</span></span> <span data-ttu-id="6ad50-218">Notez que la réponse contient également des cookies supplémentaires, tels que le cookie exchangecookie utilisé par Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="6ad50-218">Notice that the response also contains additional cookies, such as the exchangecookie cookie used by Exchange 2010.</span></span> <span data-ttu-id="6ad50-219">Exchange Online, Exchange Online dans le cadre d’Office 365 et versions d’Exchange à partir d’Exchange 2013, ignorez exchangecookie s’il est inclus dans les demandes d’abonnement ultérieures.</span><span class="sxs-lookup"><span data-stu-id="6ad50-219">Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013, ignore exchangecookie if it is included in subsequent subscription requests.</span></span>
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=ddb8c383aef34c7694132aa679744feb; expires=Thu, 25-Sep-2014 18:42:45 GMT; path=/;
    HttpOnly
Set-Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295; path=/; secure; HttpOnly
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
    expires=Wed, 25-Sep-2013 18:52:49 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAAUeGk+7JFdSaFM8/NI/gQQpVdgZX6H0Ag=</m:SubscriptionId>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </m:SubscribeResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="6ad50-220">À l’aide de X-BackEndOverrideCookie à partir de la réponse de Alfred et de l’en-tête X-AnchorMailbox, la demande d’abonnement est créée pour Sadie, l’autre membre de la demande d’abonnement de groupe A. Sadie ressemble à ceci.</span><span class="sxs-lookup"><span data-stu-id="6ad50-220">Using the X-BackEndOverrideCookie from Alfred's response and the X-AnchorMailbox header, the subscription request is created for Sadie, the other member of Group A. Sadie's subscription request looks like this.</span></span>
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@contoso.com </t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:Subscribe>
      <m:StreamingSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox" />
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
        </t:EventTypes>
      </m:StreamingSubscriptionRequest>
    </m:Subscribe>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="6ad50-221">La réponse d’abonnement de Sadie ressemble à ceci.</span><span class="sxs-lookup"><span data-stu-id="6ad50-221">Sadie's subscription response looks like this.</span></span> <span data-ttu-id="6ad50-222">Notez qu’il n’inclut pas X-BackEndOverrideCookie.</span><span class="sxs-lookup"><span data-stu-id="6ad50-222">Note that it does not include the X-BackEndOverrideCookie.</span></span> <span data-ttu-id="6ad50-223">Le client est responsable de la mise en cache de cette valeur pour les demandes ultérieures.</span><span class="sxs-lookup"><span data-stu-id="6ad50-223">The client is responsible for caching that value for future requests.</span></span>
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=640ea858f69d47ff8cce8b44c337f6d9; path=/
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
   expires= Wed, 25-Sep-2013 18:53:06 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAB4EQOy2pfrQJfM3hzs/nZJIZssan6H0Ag=</m:SubscriptionId>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </m:SubscribeResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="6ad50-224">À l’aide des valeurs [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) des réponses d’abonnement, une demande d’opération [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) a été créée pour tous les abonnements dans le groupe.</span><span class="sxs-lookup"><span data-stu-id="6ad50-224">Using the [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) values from the subscription responses, a [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) operation request was created for all the subscriptions in the group.</span></span> <span data-ttu-id="6ad50-225">Étant donné qu’il y a moins de 200 abonnements dans ce groupe, ils sont tous envoyés dans une demande.</span><span class="sxs-lookup"><span data-stu-id="6ad50-225">Because there are less than 200 subscriptions in this group, they are all sent in one request.</span></span> <span data-ttu-id="6ad50-226">L’en-tête X-PreferServerAffinity est défini sur true et l’X-BackEndOverrideCookie est inclus.</span><span class="sxs-lookup"><span data-stu-id="6ad50-226">The X-PreferServerAffinity header is set to true and the X-BackEndOverrideCookie is included.</span></span> 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:GetStreamingEvents>
      <m:SubscriptionIds>
        <t:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAB4EQOy2pfrQJfM3hzs/nZJIZssan6H0Ag=</t:SubscriptionId>
        <t:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAAUeGk+7JFdSaFM8/NI/gQQpVdgZX6H0Ag=</t:SubscriptionId>
      </m:SubscriptionIds>
      <m:ConnectionTimeout>10</m:ConnectionTimeout>
    </m:GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="6ad50-227">Les événements renvoyés sont ensuite transmis à un thread distinct pour traitement.</span><span class="sxs-lookup"><span data-stu-id="6ad50-227">The returned events are then passed to a separate thread for processing.</span></span>
  
## <a name="how-has-affinity-changed"></a><span data-ttu-id="6ad50-228">Quelles sont les modifications apportées à l’affinité ?</span><span class="sxs-lookup"><span data-stu-id="6ad50-228">How has affinity changed?</span></span>
<span data-ttu-id="6ad50-229"><a name="bk_howchanged"> </a></span><span class="sxs-lookup"><span data-stu-id="6ad50-229"><a name="bk_howchanged"> </a></span></span>

<span data-ttu-id="6ad50-230">Dans Exchange 2010, les abonnements sont conservés sur le serveur d’accès au client, comme illustré dans la figure 3.</span><span class="sxs-lookup"><span data-stu-id="6ad50-230">In Exchange 2010, subscriptions are maintained on the Client Access server, as shown in Figure 3.</span></span> <span data-ttu-id="6ad50-231">Dans les versions d’Exchange ultérieures à Exchange 2010, les abonnements sont conservés sur le serveur de boîtes aux lettres, comme le montre la figure 4.</span><span class="sxs-lookup"><span data-stu-id="6ad50-231">In versions of Exchange later than Exchange 2010, subscriptions are maintained on the Mailbox server, as shown in Figure 4.</span></span>
  
<span data-ttu-id="6ad50-232">**Figure 3. Processus de conservation de l’affinité dans Exchange 2010**</span><span class="sxs-lookup"><span data-stu-id="6ad50-232">**Figure 3. Process for maintaining affinity in Exchange 2010**</span></span>

![Illustration présentant la façon dont la table d’abonnements actifs est conservée sur le serveur d’accès au client dans Exchange 2010.](media/Exchange2013_NoficationAffinity2010.png)
  
<span data-ttu-id="6ad50-234">**Figure 4. Processus de conservation de l’affinité dans Exchange Online et Exchange 2013**</span><span class="sxs-lookup"><span data-stu-id="6ad50-234">**Figure 4. Process for maintaining affinity in Exchange Online and Exchange 2013**</span></span>

![Illustration présentant la façon dont l’équilibrage de charge et le serveur d’accès au client acheminent les demandes vers le serveur de boîtes aux lettres qui conserve la table des abonnements actifs dans Exchange Server et Exchange Online.](media/Exchange2013_NoficationAffinity2013.png)
  
<span data-ttu-id="6ad50-236">Dans Exchange 2010, le client connaît uniquement l’adresse de l’équilibreur de charge et le exchangecookie renvoyé par le serveur s’assure que la demande est routée vers le serveur d’accès au client approprié.</span><span class="sxs-lookup"><span data-stu-id="6ad50-236">In Exchange 2010, the client only knows the address of the load balancer, and the exchangecookie that is returned by the server ensures that the request is routed to the right Client Access server.</span></span> <span data-ttu-id="6ad50-237">Toutefois, dans les versions ultérieures, les rôles du serveur d’accès au client et de l’équilibreur de charge doivent tous deux acheminer les demandes de manière appropriée avant qu’ils n’obtiennent le serveur de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6ad50-237">However, in later versions, the load balancer and the Client Access server roles both have to route the requests appropriately before they get to the Mailbox server.</span></span> <span data-ttu-id="6ad50-238">Pour ce faire, des informations supplémentaires sont requises, c’est pourquoi les nouveaux en-têtes et les cookies ont été introduits.</span><span class="sxs-lookup"><span data-stu-id="6ad50-238">To do that, additional information is required, which is why the new headers and cookie were introduced.</span></span> <span data-ttu-id="6ad50-239">L’article [abonnements aux notifications, les événements de boîte aux lettres et EWS dans Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) explique comment les abonnements sont gérés dans Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="6ad50-239">The article [Notification subscriptions, mailbox events, and EWS in Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) explains how subscriptions are maintained in Exchange 2013.</span></span> 
  
<span data-ttu-id="6ad50-240">Vous pouvez remarquer que le exchangecookie utilisé par Exchange 2010 est toujours renvoyé par les versions ultérieures.</span><span class="sxs-lookup"><span data-stu-id="6ad50-240">You might notice that the exchangecookie that Exchange 2010 uses is still returned by later versions.</span></span> <span data-ttu-id="6ad50-241">Il n’y a aucun dommage à inclure ce cookie dans les requêtes, mais les versions ultérieures d’Exchange l’ignorent.</span><span class="sxs-lookup"><span data-stu-id="6ad50-241">There's no harm in including this cookie in requests, but later versions of Exchange ignore it.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="6ad50-242">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6ad50-242">See also</span></span>

- [<span data-ttu-id="6ad50-243">Abonnements à des notifications, événements de boîte aux lettres et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6ad50-243">Notification subscriptions, mailbox events, and EWS in Exchange</span></span>](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [<span data-ttu-id="6ad50-244">Notifications de flux concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6ad50-244">Stream notifications about mailbox events by using EWS in Exchange</span></span>](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [<span data-ttu-id="6ad50-245">Notifications de type pull concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6ad50-245">Pull notifications about mailbox events by using EWS in Exchange</span></span>](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [<span data-ttu-id="6ad50-246">Gestion des erreurs liées à la notification dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6ad50-246">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
- [<span data-ttu-id="6ad50-247">Modifications apportées à la gestion de l’affinité pour les abonnements EWS...</span><span class="sxs-lookup"><span data-stu-id="6ad50-247">Changes in Managing Affinity for EWS Subscriptions…</span></span>](https://blogs.msdn.com/b/mstehle/archive/2013/04/17/changes-in-managing-affinity-for-ews-subscriptions.aspx)
- [<span data-ttu-id="6ad50-248">Limitation EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6ad50-248">EWS throttling in Exchange</span></span>](ews-throttling-in-exchange.md)
    

