---
title: Outils et ressources pour la résolution des problèmes des applications EWS pour Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ee7fcd05-35d7-47bf-bac4-e719c49c11fe
description: Trouvez des ressources pour vous aider à résoudre les problèmes des applications EWS API managées.
ms.openlocfilehash: d8d8ea736ca3b896642ad06f5987caeba8d8d059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755073"
---
# <a name="tools-and-resources-for-troubleshooting-ews-applications-for-exchange"></a><span data-ttu-id="b7c05-103">Outils et ressources pour la résolution des problèmes des applications EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="b7c05-103">Tools and resources for troubleshooting EWS applications for Exchange</span></span>

<span data-ttu-id="b7c05-104">Trouvez des ressources pour vous aider à résoudre les problèmes des applications EWS API managées.</span><span class="sxs-lookup"><span data-stu-id="b7c05-104">Find resources to help you troubleshoot your EWS Managed API or EWS application.</span></span>
  
<span data-ttu-id="b7c05-105">Éléments ne se déroule pas comme prévu.</span><span class="sxs-lookup"><span data-stu-id="b7c05-105">Things don't always go as planned.</span></span> <span data-ttu-id="b7c05-106">Parfois EWS demande échoue ou fournir des résultats inattendus.</span><span class="sxs-lookup"><span data-stu-id="b7c05-106">Sometimes EWS requests fail, or provide unexpected results.</span></span> <span data-ttu-id="b7c05-107">Cela peut être frustrant, surtout si la raison n’est pas évidente.</span><span class="sxs-lookup"><span data-stu-id="b7c05-107">This can be frustrating, especially if the reason isn't obvious.</span></span> <span data-ttu-id="b7c05-108">J’espère que cela vous arrivera jamais, mais dans ce cas, cet article fournit des informations sur les outils et les ressources que vous pouvez utiliser pour aider à résoudre le problème.</span><span class="sxs-lookup"><span data-stu-id="b7c05-108">Hopefully this never happens to you, but if it does, this article provides information about tools and resources that you can use to help troubleshoot your problem.</span></span>
  
> [!NOTE]
> <span data-ttu-id="b7c05-109">Cet article fournit des conseils de résolution des problèmes généraux et les sources des informations de dépannage.</span><span class="sxs-lookup"><span data-stu-id="b7c05-109">This article provides general troubleshooting advice and sources for troubleshooting information.</span></span> <span data-ttu-id="b7c05-110">Malheureusement il n’est pas possible d’attribuer des étapes de dépannage détaillées.</span><span class="sxs-lookup"><span data-stu-id="b7c05-110">Unfortunately it isn't possible to give detailed troubleshooting steps.</span></span> <span data-ttu-id="b7c05-111">Pour obtenir une assistance dépannage votre erreur spécifique, voir les [étapes suivantes](#bk_NextSteps).</span><span class="sxs-lookup"><span data-stu-id="b7c05-111">For assistance troubleshooting your specific error, see [Next steps](#bk_NextSteps).</span></span> 
  
## <a name="examine-the-soap-requests-and-responses"></a><span data-ttu-id="b7c05-112">Examiner les demandes et réponses SOAP</span><span class="sxs-lookup"><span data-stu-id="b7c05-112">Examine the SOAP requests and responses</span></span>

<span data-ttu-id="b7c05-113">Lorsque les choses ne fonctionnent pas correctement, il est très utile pour être en mesure de voir ce qui se passe.</span><span class="sxs-lookup"><span data-stu-id="b7c05-113">When things aren't working correctly, it really helps to be able to see what's going on.</span></span> <span data-ttu-id="b7c05-114">La première ligne de la recherche lorsque vous recherchez un problème avec EWS ou l’API managée EWS consiste à examiner les demandes de l’envoi de votre application sur le réseau et les réponses que le serveur envoie précédent.</span><span class="sxs-lookup"><span data-stu-id="b7c05-114">The first line of inquiry when investigating a problem with EWS or the EWS Managed API is to examine the requests that your application is sending over the network and the responses that the server is sending back.</span></span>
  
<span data-ttu-id="b7c05-115">L’API managée EWS facilite examen demandes et réponses SOAP avec son [intégré dans la fonctionnalité de suivi](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md).</span><span class="sxs-lookup"><span data-stu-id="b7c05-115">The EWS Managed API makes examining SOAP requests and responses easy with its [built in tracing functionality](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md).</span></span> <span data-ttu-id="b7c05-116">Si vous utilisez EWS, vous pouvez ou n’aurez pas accès à une fonctionnalité similaire suivi, en fonction de quel plateforme ou les classes qui vous permet d’envoyer vos demandes.</span><span class="sxs-lookup"><span data-stu-id="b7c05-116">If you are using EWS, you might or might not have access to similar tracing functionality, depending on what platform or classes you use to send your requests.</span></span> <span data-ttu-id="b7c05-117">Toutefois, vous pouvez toujours utiliser un outil de suivi réseau comme [Moniteur réseau](http://www.microsoft.com/en-us/download/details.aspx?id=4865) ou [Fiddler](http://www.telerik.com/fiddler) examiner le trafic réseau et d’afficher les charges de demande et de réponse.</span><span class="sxs-lookup"><span data-stu-id="b7c05-117">However, you can always use a network tracing tool like [Network Monitor](http://www.microsoft.com/en-us/download/details.aspx?id=4865) or [Fiddler](http://www.telerik.com/fiddler) to examine the network traffic and view the request and response payloads.</span></span> 
  
<span data-ttu-id="b7c05-118">En outre, vous pouvez [instrument vos requêtes client](instrumenting-client-requests-for-ews-and-rest-in-exchange.md) afin d’améliorer les informations disponibles dans les demandes et réponses.</span><span class="sxs-lookup"><span data-stu-id="b7c05-118">Additionally, you can [instrument your client requests](instrumenting-client-requests-for-ews-and-rest-in-exchange.md) to enhance the information available in requests and responses.</span></span> 
  
<span data-ttu-id="b7c05-119">Une fois que vous avez les demandes et les réponses, posez-vous les éléments suivants : font elles semblent correctes ?</span><span class="sxs-lookup"><span data-stu-id="b7c05-119">After you have the requests and responses, ask yourself the following: Do they look correct?</span></span> <span data-ttu-id="b7c05-120">Sont les valeurs que votre application envoie attendue ?</span><span class="sxs-lookup"><span data-stu-id="b7c05-120">Are the values that your application is sending expected?</span></span> <span data-ttu-id="b7c05-121">Les réponses ont sens ?</span><span class="sxs-lookup"><span data-stu-id="b7c05-121">Do the responses make sense?</span></span>
  
## <a name="examine-error-codes"></a><span data-ttu-id="b7c05-122">Examinez les codes d’erreur</span><span class="sxs-lookup"><span data-stu-id="b7c05-122">Examine error codes</span></span>

<span data-ttu-id="b7c05-123">Le code d’erreur peuvent-ils parfois permettent de localiser le problème, même si au premier coup de œil cela ne semble pas pertinent.</span><span class="sxs-lookup"><span data-stu-id="b7c05-123">Sometimes the error code can go a long way toward pinpointing the problem, even if at first glance it doesn't seem to make sense.</span></span> <span data-ttu-id="b7c05-124">L’erreur indique que votre client est [limitée](ews-throttling-in-exchange.md)?</span><span class="sxs-lookup"><span data-stu-id="b7c05-124">Does the error indicate that your client is being [throttled](ews-throttling-in-exchange.md)?</span></span> <span data-ttu-id="b7c05-125">Un appel à la découverte automatique pour [Actualiser les informations de configuration](how-to-refresh-configuration-information-by-using-autodiscover.md) est peut-être dans l’ordre ?</span><span class="sxs-lookup"><span data-stu-id="b7c05-125">Perhaps a call to Autodiscover to [refresh configuration information](how-to-refresh-configuration-information-by-using-autodiscover.md) is in order?</span></span> 
  
<span data-ttu-id="b7c05-126">Pour plus d’informations sur la gestion des erreurs spécifiques, voir les articles suivants :</span><span class="sxs-lookup"><span data-stu-id="b7c05-126">For more information about handling specific errors, see the following articles:</span></span>
  
- [<span data-ttu-id="b7c05-127">Gestion des messages d'erreur de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="b7c05-127">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
- [<span data-ttu-id="b7c05-128">Gestion des erreurs liées à la notification dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7c05-128">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="b7c05-129">Gestion des erreurs liées à la synchronisation dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7c05-129">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="b7c05-130">Gestion des erreurs liées aux suppression dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7c05-130">Handling deletion-related errors in EWS in Exchange</span></span>](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="verify-versions"></a><span data-ttu-id="b7c05-131">Vérifier les versions</span><span class="sxs-lookup"><span data-stu-id="b7c05-131">Verify versions</span></span>

<span data-ttu-id="b7c05-132">Il existe un nombre de différents composants impliqués dans les opérations EWS et les versions de ces composants peuvent influer sur les résultats.</span><span class="sxs-lookup"><span data-stu-id="b7c05-132">There are a number of different components involved in EWS operations, and the versions of those components can influence the results.</span></span>
  
<span data-ttu-id="b7c05-133">**Le tableau 1. Composants de versions susceptibles d’affecter les processus EWS**</span><span class="sxs-lookup"><span data-stu-id="b7c05-133">**Table 1. Versioned components that can affect EWS processes**</span></span>

|<span data-ttu-id="b7c05-134">**Composant**</span><span class="sxs-lookup"><span data-stu-id="b7c05-134">**Component**</span></span>|<span data-ttu-id="b7c05-135">**API managée par EWS**</span><span class="sxs-lookup"><span data-stu-id="b7c05-135">**EWS Managed API**</span></span>|<span data-ttu-id="b7c05-136">**EWS**</span><span class="sxs-lookup"><span data-stu-id="b7c05-136">**EWS**</span></span>|<span data-ttu-id="b7c05-137">**Remarques**</span><span class="sxs-lookup"><span data-stu-id="b7c05-137">**Notes**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="b7c05-138">Version du serveur demandée</span><span class="sxs-lookup"><span data-stu-id="b7c05-138">Requested server version</span></span>  <br/> |<span data-ttu-id="b7c05-139">Propriété [ExchangeServiceBase.RequestedServerVersion](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="b7c05-139">[ExchangeServiceBase.RequestedServerVersion](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="b7c05-140">Élément [RequestServerVersion](http://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="b7c05-140">[RequestServerVersion](http://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx) element</span></span>  <br/> |<span data-ttu-id="b7c05-141">Cette valeur contrôle la version du schéma EWS est utilisée pour traiter la demande EWS.</span><span class="sxs-lookup"><span data-stu-id="b7c05-141">This value controls which version of the EWS schema is used to process the EWS request.</span></span> <span data-ttu-id="b7c05-142">Assurez-vous que la version du schéma spécifiée dans ce champ est significatif pour la demande vous envoyez.</span><span class="sxs-lookup"><span data-stu-id="b7c05-142">Make sure that the schema version specified here makes sense for the request you are sending.</span></span> <span data-ttu-id="b7c05-143">Certaines propriétés et opérations ne sont pas disponibles dans les versions antérieures du schéma.</span><span class="sxs-lookup"><span data-stu-id="b7c05-143">Some properties and operations are not available in earlier versions of the schema.</span></span>  <br/> |
|<span data-ttu-id="b7c05-144">La version du serveur</span><span class="sxs-lookup"><span data-stu-id="b7c05-144">The server version</span></span>  <br/> |<span data-ttu-id="b7c05-145">Propriété [ExchangeServiceBase.ServerInfo](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservicebase.serverinfo%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="b7c05-145">[ExchangeServiceBase.ServerInfo](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservicebase.serverinfo%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="b7c05-146">Élément [ServerVersionInfo](http://msdn.microsoft.com/library/c04a6872-ca27-432b-aac2-36b023d0afc6%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="b7c05-146">[ServerVersionInfo](http://msdn.microsoft.com/library/c04a6872-ca27-432b-aac2-36b023d0afc6%28Office.15%29.aspx) element</span></span>  <br/> |<span data-ttu-id="b7c05-147">Cette valeur est retournée par le serveur dans les réponses EWS et indique la version du serveur qui a traité la réponse.</span><span class="sxs-lookup"><span data-stu-id="b7c05-147">This value is returned by the server in EWS responses, and indicates the version of the server that processed the response.</span></span> <span data-ttu-id="b7c05-148">Assurez-vous que cette valeur est ce que vous attendez.</span><span class="sxs-lookup"><span data-stu-id="b7c05-148">Make sure this value is what you expect.</span></span> <span data-ttu-id="b7c05-149">Si possible, assurez-vous que le serveur Exchange exécute la mise à jour les plus récent pour votre version majeure d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="b7c05-149">If possible, make sure that the Exchange server is running the most recent update for your major version of Exchange.</span></span>  <br/> |
|<span data-ttu-id="b7c05-150">La version de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="b7c05-150">The EWS Managed API version</span></span>  <br/> |<span data-ttu-id="b7c05-151">La propriété version de produit du fichier Microsoft.Exchange.WebServices.dll.</span><span class="sxs-lookup"><span data-stu-id="b7c05-151">The Product version property of the Microsoft.Exchange.WebServices.dll file.</span></span>  <br/> |<span data-ttu-id="b7c05-152">Not applicable</span><span class="sxs-lookup"><span data-stu-id="b7c05-152">Not applicable</span></span>  <br/> |<span data-ttu-id="b7c05-153">Si vous utilisez l’API managée EWS, assurez-vous que vous utilisez [la version la plus récente](http://aka.ms/ews-managed-api-readme).</span><span class="sxs-lookup"><span data-stu-id="b7c05-153">If you're using the EWS Managed API, make sure that you are using [the most recent version](http://aka.ms/ews-managed-api-readme).</span></span>  <br/> |
   
## <a name="verify-access"></a><span data-ttu-id="b7c05-154">Vérifier l’accès</span><span class="sxs-lookup"><span data-stu-id="b7c05-154">Verify access</span></span>

<span data-ttu-id="b7c05-155">EWS est activée par défaut, mais [peut être modifié par défaut](how-to-control-access-to-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="b7c05-155">EWS is enabled by default, but [defaults can be changed](how-to-control-access-to-ews-in-exchange.md).</span></span> <span data-ttu-id="b7c05-156">Utilisez l’applet de commande [Get-OrganizationConfig](http://technet.microsoft.com/en-us/library/bb124754.aspx) pour vous assurer que EWS est activée sur le serveur et l’applet de commande [Get-CASMailbox](http://technet.microsoft.com/en-us/library/aa997571.aspx) pour vous assurer que EWS est activé pour la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b7c05-156">Use the [Get-OrganizationConfig](http://technet.microsoft.com/en-us/library/bb124754.aspx) cmdlet to make sure that EWS is enabled on the server, and the [Get-CASMailbox](http://technet.microsoft.com/en-us/library/aa997571.aspx) cmdlet to make sure that EWS is enabled for the user's mailbox.</span></span> <span data-ttu-id="b7c05-157">Vérifiez également les deux réponses de l’applet de commande pour un EWS autorisent ou bloquent la liste et vous assurer que votre application n’est pas bloquée à partir de l’aide de EWS.</span><span class="sxs-lookup"><span data-stu-id="b7c05-157">Also check both cmdlet responses for an EWS allow or block list, and make sure that your application isn't blocked from using EWS.</span></span> 
  
<span data-ttu-id="b7c05-158">Vous devez également vérifier que les [paramètres d’authentification par défaut](http://technet.microsoft.com/en-us/library/gg247612%28v=exchg.150%29.aspx) dans le répertoire virtuel EWS n’ont pas été modifiés.</span><span class="sxs-lookup"><span data-stu-id="b7c05-158">You should also verify that the [default authentication settings](http://technet.microsoft.com/en-us/library/gg247612%28v=exchg.150%29.aspx) on the EWS virtual directory have not been modified.</span></span> 
  
## <a name="try-another-ews-client"></a><span data-ttu-id="b7c05-159">Essayer un autre client EWS</span><span class="sxs-lookup"><span data-stu-id="b7c05-159">Try another EWS client</span></span>

<span data-ttu-id="b7c05-160">Il est parfois utile essayer la même requête à partir d’un autre client et comparer les résultats.</span><span class="sxs-lookup"><span data-stu-id="b7c05-160">Sometimes it is helpful to try the same request from another client and compare results.</span></span> <span data-ttu-id="b7c05-161">Si un autre client obtient des résultats différents, quelle est la différence ?</span><span class="sxs-lookup"><span data-stu-id="b7c05-161">If another client gets different results, what is different?</span></span> <span data-ttu-id="b7c05-162">Déterminer quelle est la différence entre une demande réussie et une demande ayant échouée peut aider à expliquer pourquoi une requête particulière est défectueux.</span><span class="sxs-lookup"><span data-stu-id="b7c05-162">Figuring out what is different between a successful request and a failed request can help explain why a particular request is failing.</span></span>
  
<span data-ttu-id="b7c05-163">Si vous pouvez écrire certainement un autre client pour le test, vous n’avez pas besoin !</span><span class="sxs-lookup"><span data-stu-id="b7c05-163">While you can certainly write another client to test with, you don't have to!</span></span> <span data-ttu-id="b7c05-164">[EWSEditor](http://ewseditor.codeplex.com/) est un exemple de client qui utilise les API managées EWS.</span><span class="sxs-lookup"><span data-stu-id="b7c05-164">[EWSEditor](http://ewseditor.codeplex.com/) is a sample client that uses the EWS Managed API and EWS.</span></span> <span data-ttu-id="b7c05-165">Vous pouvez télécharger le client (y compris le code source) et l’utiliser pour essayer les mêmes requêtes sont défectueux dans votre application.</span><span class="sxs-lookup"><span data-stu-id="b7c05-165">You can download the client (including the source code) and use it to try the same requests that are failing in your application.</span></span> 
  
## <a name="examine-iis-logs"></a><span data-ttu-id="b7c05-166">Examiner les journaux IIS</span><span class="sxs-lookup"><span data-stu-id="b7c05-166">Examine IIS logs</span></span>

<span data-ttu-id="b7c05-167">Si vous avez accès au serveur Exchange, la fonctionnalité de journalisation fournie par Internet Information Services (IIS) sur les serveurs d’accès au Client peut fournir plus d’informations sur les échecs.</span><span class="sxs-lookup"><span data-stu-id="b7c05-167">If you have access to the Exchange server, the logging functionality provided by Internet Information Services (IIS) on the Client Access servers can provide more information about failures.</span></span> <span data-ttu-id="b7c05-168">Toutefois, n’oubliez pas que les journaux IIS ne seront utiles si vous recevez une erreur HTTP.</span><span class="sxs-lookup"><span data-stu-id="b7c05-168">However, keep in mind that IIS logs will only be helpful if you are receiving an HTTP error.</span></span>
  
<span data-ttu-id="b7c05-169">IIS fournit deux méthodes de journalisation différentes : [échecs de demandes de suivi](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)et de [journalisation IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis) .</span><span class="sxs-lookup"><span data-stu-id="b7c05-169">IIS provides two different logging methods: [IIS logging](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis) and [failed requests tracing](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis).</span></span> <span data-ttu-id="b7c05-170">Pour travailler avec les journaux IIS, vous pouvez utiliser [Log Parser Studio](http://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx), qui comprend un nombre de requêtes EWS intégrées.</span><span class="sxs-lookup"><span data-stu-id="b7c05-170">To work with IIS logs, you can use [Log Parser Studio](http://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx), which includes a number of built-in EWS queries.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="b7c05-171">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="b7c05-171">Next steps</span></span>
<span data-ttu-id="b7c05-172"><a name="bk_NextSteps"> </a></span><span class="sxs-lookup"><span data-stu-id="b7c05-172"></span></span>

<span data-ttu-id="b7c05-173">Maintenant que vous avez appris à utiliser les outils et les ressources que vous pouvez utiliser pour résoudre les problèmes, vous devrez comprendre les informations fournies par ces outils.</span><span class="sxs-lookup"><span data-stu-id="b7c05-173">Now that you've learned about the tools and resources that you can use to troubleshoot, you might need help understanding the information provided by those tools.</span></span> <span data-ttu-id="b7c05-174">Certaines options pour obtenir de l’aide sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="b7c05-174">The following are some options for getting help:</span></span>
  
- <span data-ttu-id="b7c05-175">[Forum de développement d’Exchange Server sur MSDN](http://social.msdn.microsoft.com/Forums/en-US/home?category=exchangeserver) : poser une question de la Communauté de développement MSDN Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="b7c05-175">[Exchange Server Development forum on MSDN](http://social.msdn.microsoft.com/Forums/en-US/home?category=exchangeserver) — Ask a question of the MSDN Exchange Server development community.</span></span> 
    
- <span data-ttu-id="b7c05-176">[StackOverflow](http://stackoverflow.com/tags/ews) : poser une question de la Communauté StackOverflow.</span><span class="sxs-lookup"><span data-stu-id="b7c05-176">[StackOverflow](http://stackoverflow.com/tags/ews) — Ask a question of the StackOverflow community.</span></span> <span data-ttu-id="b7c05-177">Veillez à ajouter une balise à votre publication avec « ews ».</span><span class="sxs-lookup"><span data-stu-id="b7c05-177">Be sure to tag your post with "ews".</span></span> 
    
- <span data-ttu-id="b7c05-178">[Prise en charge de Microsoft](http://support.microsoft.com/ph/730/en-us) , contactez le support technique Microsoft pour obtenir une assistance.</span><span class="sxs-lookup"><span data-stu-id="b7c05-178">[Microsoft Support](http://support.microsoft.com/ph/730/en-us) — Contact a Microsoft support professional for assistance.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="b7c05-179">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b7c05-179">See also</span></span>


<span data-ttu-id="b7c05-180">Voir les articles suivants :</span><span class="sxs-lookup"><span data-stu-id="b7c05-180">See the following articles:</span></span>
  
- [<span data-ttu-id="b7c05-181">Développer des clients de service web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="b7c05-181">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="b7c05-182">Suivi des demandes et réponses pour dépanner les applications de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="b7c05-182">Trace requests and responses to troubleshoot EWS Managed API applications</span></span>](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    
- [<span data-ttu-id="b7c05-183">L'instrumentation des demandes du client pour EWS et reste dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7c05-183">Instrumenting client requests for EWS and REST in Exchange</span></span>](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)
    
- [<span data-ttu-id="b7c05-184">Limitation EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7c05-184">EWS throttling in Exchange</span></span>](ews-throttling-in-exchange.md)
    
- [<span data-ttu-id="b7c05-185">Actualiser les informations de configuration à l’aide de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="b7c05-185">Refresh configuration information by using Autodiscover</span></span>](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [<span data-ttu-id="b7c05-186">Gestion des messages d'erreur de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="b7c05-186">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
- [<span data-ttu-id="b7c05-187">Gestion des erreurs liées à la notification dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7c05-187">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="b7c05-188">Gestion des erreurs liées à la synchronisation dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7c05-188">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="b7c05-189">Gestion des erreurs liées aux suppression dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b7c05-189">Handling deletion-related errors in EWS in Exchange</span></span>](handling-deletion-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="b7c05-190">Configuration de l’enregistrement dans IIS</span><span class="sxs-lookup"><span data-stu-id="b7c05-190">Configuring Logging in IIS</span></span>](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis)
    
- [<span data-ttu-id="b7c05-191">Dépannage des échecs de demandes à l’aide de suivi dans IIS 7</span><span class="sxs-lookup"><span data-stu-id="b7c05-191">Troubleshooting Failed Requests Using Tracing in IIS 7</span></span>](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)
    
- [<span data-ttu-id="b7c05-192">Présentation : Log Parser Studio</span><span class="sxs-lookup"><span data-stu-id="b7c05-192">Introducing: Log Parser Studio</span></span>](http://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx)
    
- [<span data-ttu-id="b7c05-193">Paramètres par défaut des répertoires virtuels Exchange</span><span class="sxs-lookup"><span data-stu-id="b7c05-193">Default Settings for Exchange Virtual Directories</span></span>](http://technet.microsoft.com/en-us/library/gg247612%28v=exchg.150%29.aspx)
    
<span data-ttu-id="b7c05-194">Télécharger les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="b7c05-194">Download the following:</span></span>
  
- [<span data-ttu-id="b7c05-195">Moniteur réseau Microsoft 3.4</span><span class="sxs-lookup"><span data-stu-id="b7c05-195">Microsoft Network Monitor 3.4</span></span>](http://www.microsoft.com/en-us/download/details.aspx?id=4865)
    
- [<span data-ttu-id="b7c05-196">Fiddler</span><span class="sxs-lookup"><span data-stu-id="b7c05-196">Fiddler</span></span>](http://www.telerik.com/fiddler)
    
- [<span data-ttu-id="b7c05-197">EWSEditor</span><span class="sxs-lookup"><span data-stu-id="b7c05-197">EWSEditor</span></span>](http://ewseditor.codeplex.com/)
    
- [<span data-ttu-id="b7c05-198">API gérée Exchange Web Services</span><span class="sxs-lookup"><span data-stu-id="b7c05-198">Exchange Web Services Managed API</span></span>](http://go.microsoft.com/fwlink/?LinkID=255472)
    
