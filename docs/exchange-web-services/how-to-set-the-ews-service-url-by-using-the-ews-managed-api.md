---
title: Définir l’URL du service EWS à l’aide de l’API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: cddf6525-1c04-484b-a911-56c2f0f1f7b6
description: Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Trouvez des informations sur la configuration de l'URL du service EWS dans votre application d'API managée EWS.
ms.openlocfilehash: e1a414f7c6f13bd61a58403c9d2be546c0226a69
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754935"
---
# <a name="set-the-ews-service-url-by-using-the-ews-managed-api"></a><span data-ttu-id="48186-103">Définir l’URL du service EWS à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="48186-103">Set the EWS service URL by using the EWS Managed API</span></span>

<span data-ttu-id="48186-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Trouvez des informations sur la configuration de l'URL du service EWS dans votre application d'API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="48186-104">Find information about how to set the EWS service URL in your EWS Managed API application.</span></span>
  
<span data-ttu-id="48186-p101">L'URL du service est l'adresse qu'Exchange utilise pour communiquer avec les services web Exchange (EWS). Une fois que votre application d'API managée EWS a cette adresse et qu'elle dispose d'un accès approprié pour [communiquer avec EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md), elle peut effectuer des appels vers la [classe ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx). L'URL du service pour un serveur Exchange local peut se présenter comme suit.</span><span class="sxs-lookup"><span data-stu-id="48186-p101">The service URL is the address that Exchange uses to communicate with Exchange Web Services (EWS). After your EWS Managed API application has this address, and has appropriate access to [communicate with EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md), it can make calls to the [ExchangeService class](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx). The service URL for an on-premises Exchange server might look like the following.</span></span> 
  
```HTML
https://computer.domain.contoso.com/EWS/Exchange.asmx
```

<span data-ttu-id="48186-p102">Vous pouvez définir l'URL EWS dans votre application de deux manières. Nous vous conseillons d'utiliser le [service de découverte automatique](http://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx) pour obtenir l'URL, car dans une vaste forêt de serveurs, l'URL peut changer si la boîte aux lettres est migrée vers un autre serveur. Toutefois, comme l'appel du service de découverte automatique peut prendre du temps et ralentir votre application, si vous devez effectuer plusieurs appels sur une courte période, vous devrez peut-être mettre en cache la valeur de l'URL obtenue grâce à la découverte automatique et définir manuellement l'URL du service EWS à l'aide de cette valeur mise en cache. Cela améliore les performances de votre application ; veillez simplement à utiliser la découverte automatique pour mettre à jour régulièrement la valeur mise en cache, au cas où la valeur soit modifiée sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="48186-p102">You can set the EWS URL in your application in a couple of ways. We recommend that you use the [Autodiscover service](http://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx) to get the URL because in a large forest of servers, the URL can change if the mailbox is migrated to another server. However, because calling Autodiscover can take some time and can slow down your application if you need to make multiple calls in a short period of time, you might want to cache the URL value you get from Autodiscover and manually set the EWS service URL with this cached value. This will improve the performance of your application; just make sure that you use Autodiscover to update your cached value periodically in case the value changes on the server.</span></span> 
  
## <a name="set-the-ews-service-url-by-using-the-autodiscover-service"></a><span data-ttu-id="48186-112">Définir l'URL du service EWS en utilisant le service de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="48186-112">Set the EWS service URL by using the Autodiscover service</span></span>
<span data-ttu-id="48186-113"><a name="bk_SetURLusingAutoDiscover"> </a></span><span class="sxs-lookup"><span data-stu-id="48186-113"></span></span>

<span data-ttu-id="48186-p103">La méthode [AutodiscoverUrl](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) utilise l'adresse électronique pour définir le point de terminaison [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) et elle permet à votre application d'utiliser toutes les méthodes incluses dans les classes proxy **ExchangeService**. L'exemple qui suit illustre l'utilisation de la méthode **AutodiscoverURL**.</span><span class="sxs-lookup"><span data-stu-id="48186-p103">The [AutodiscoverUrl](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) method uses the email address to set the [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) endpoint and enables your application to use any methods included in the **ExchangeService** proxy classes. The following example shows how to use the **AutodiscoverURL** method.</span></span> 
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.AutodiscoverUrl("User1@contoso.com");

```

## <a name="set-the-exchange-service-url-manually"></a><span data-ttu-id="48186-116">Définir manuellement l'URL du service Exchange</span><span class="sxs-lookup"><span data-stu-id="48186-116">Set the Exchange service URL manually</span></span>
<span data-ttu-id="48186-117"><a name="bk_SetURLmanually"> </a></span><span class="sxs-lookup"><span data-stu-id="48186-117"></span></span>

<span data-ttu-id="48186-p104">L'exemple qui suit illustre la définition de l'URL du service EWS à l'aide d'une valeur mise en cache. Avant cela, veillez à utiliser le service de découverte automatique pour obtenir l'URL EWS.</span><span class="sxs-lookup"><span data-stu-id="48186-p104">The following example shows you how to set the EWS service URL by using a cached value. Before you do this, make sure to use the Autodiscover service to get the EWS URL.</span></span>
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.Url = new Uri("https://computername.domain.contoso.com/EWS/Exchange.asmx");

```

## <a name="see-also"></a><span data-ttu-id="48186-120">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="48186-120">See also</span></span>

- [<span data-ttu-id="48186-121">Prise en main des applications clientes d'API managée EWS</span><span class="sxs-lookup"><span data-stu-id="48186-121">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)   
- [<span data-ttu-id="48186-122">La configuration de votre environnement de développement d'applications Exchange</span><span class="sxs-lookup"><span data-stu-id="48186-122">Setting up your Exchange application development environment</span></span>](setting-up-your-exchange-application-development-environment.md)   
- [<span data-ttu-id="48186-123">Contrôler l’accès à EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="48186-123">Control access to EWS in Exchange</span></span>](how-to-control-access-to-ews-in-exchange.md) 
- [<span data-ttu-id="48186-124">Communiquer avec EWS à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="48186-124">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)  
- [<span data-ttu-id="48186-125">Utiliser la découverte automatique pour rechercher les points de connexion</span><span class="sxs-lookup"><span data-stu-id="48186-125">Use Autodiscover to find connection points</span></span>](how-to-use-autodiscover-to-find-connection-points.md)
    

