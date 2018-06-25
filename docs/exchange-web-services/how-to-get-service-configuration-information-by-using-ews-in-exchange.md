---
title: Obtenir des informations de configuration de service à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9379740a-96e1-490d-a229-0f9937c548d2
description: Découvrez comment obtenir des informations de configuration de service de messagerie unifiée, déplacer de stratégie, les conseils de messagerie et les règles de protection d’EWS dans Exchange.
ms.openlocfilehash: e84a563bb094a2fe03e08f8e1a81b2b054d45850
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754835"
---
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a><span data-ttu-id="a1035-103">Obtenir des informations de configuration de service à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a1035-103">Get service configuration information by using EWS in Exchange</span></span>

<span data-ttu-id="a1035-104">Découvrez comment obtenir des informations de configuration de service de messagerie unifiée, déplacer de stratégie, les conseils de messagerie et les règles de protection d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1035-104">Find out how to get service configuration information for UM, policy nudges, mail tips, and protection rules from EWS in Exchange.</span></span>
  
<span data-ttu-id="a1035-105">Votre application EWS fonctionne avec la messagerie unifiée (MU), déplacer de stratégie, les conseils de messagerie ou les règles de protection ?</span><span class="sxs-lookup"><span data-stu-id="a1035-105">Does your EWS application work with Unified Messaging (UM), policy nudges, mail tips, or protection rules?</span></span> <span data-ttu-id="a1035-106">Dans ce cas, votre application vous devrez appeler l' [opération GetServiceConfiguration](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) pour obtenir les informations de configuration de service qui lui sont nécessaires.</span><span class="sxs-lookup"><span data-stu-id="a1035-106">If so, your application will need to call the [GetServiceConfiguration operation](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) to get the service configuration information that it needs.</span></span> <span data-ttu-id="a1035-107">L’opération **GetServiceConfiguration** renvoie des informations de configuration spécifiques à chacune de ces fonctionnalités EWS.</span><span class="sxs-lookup"><span data-stu-id="a1035-107">The **GetServiceConfiguration** operation returns configuration information that is specific to each of these EWS features.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a1035-108">L’API managée EWS n’implémente pas cette fonctionnalité.</span><span class="sxs-lookup"><span data-stu-id="a1035-108">The EWS Managed API does not implement this functionality.</span></span> 
  
<span data-ttu-id="a1035-109">**Le tableau 1. Informations de configuration qui renvoie l’opération GetServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="a1035-109">**Table 1. Configuration information that the GetServiceConfiguration operation returns**</span></span>

|<span data-ttu-id="a1035-110">Fonctionnalité EWS</span><span class="sxs-lookup"><span data-stu-id="a1035-110">EWS feature</span></span>|<span data-ttu-id="a1035-111">Opération GetServiceConfiguration renvoie...</span><span class="sxs-lookup"><span data-stu-id="a1035-111">GetServiceConfiguration operation returns…</span></span>|
|:-----|:-----|
|<span data-ttu-id="a1035-112">MESSAGERIE UNIFIÉE</span><span class="sxs-lookup"><span data-stu-id="a1035-112">UM</span></span>  <br/> | <ul><li><span data-ttu-id="a1035-113">Une valeur qui indique si la messagerie unifiée est activée.</span><span class="sxs-lookup"><span data-stu-id="a1035-113">A value that indicates whether UM is enabled.</span></span></li><li><span data-ttu-id="a1035-114">Une valeur qui indique si l’option Lire sur le téléphone est activée.</span><span class="sxs-lookup"><span data-stu-id="a1035-114">A value that indicates whether play on phone is enabled.</span></span></li><li><span data-ttu-id="a1035-115">La lire sur la chaîne de numérotation téléphonique.</span><span class="sxs-lookup"><span data-stu-id="a1035-115">The play on phone dial string.</span></span></li></ul> |
|<span data-ttu-id="a1035-116">Déplacer de stratégie</span><span class="sxs-lookup"><span data-stu-id="a1035-116">Policy nudges</span></span>  <br/> | <ul><li><span data-ttu-id="a1035-117">Stratégie est déplacée pour l’affichage de votre client.</span><span class="sxs-lookup"><span data-stu-id="a1035-117">Policy nudges for display in your client.</span></span></li></ul> |
|<span data-ttu-id="a1035-118">Conseils de messagerie</span><span class="sxs-lookup"><span data-stu-id="a1035-118">Mail tips</span></span>  <br/> | <ul><li><span data-ttu-id="a1035-119">Une valeur qui indique si les conseils de la messagerie sont activées.</span><span class="sxs-lookup"><span data-stu-id="a1035-119">A value that indicates whether mail tips are enabled.</span></span></li><li><span data-ttu-id="a1035-120">Le nombre maximal de destinataires par demande.</span><span class="sxs-lookup"><span data-stu-id="a1035-120">The maximum number of recipients per request.</span></span></li><li><span data-ttu-id="a1035-121">La taille maximale des messages.</span><span class="sxs-lookup"><span data-stu-id="a1035-121">The maximum message size.</span></span></li><li><span data-ttu-id="a1035-122">Le seuil de large public.</span><span class="sxs-lookup"><span data-stu-id="a1035-122">The large audience threshold.</span></span></li><li><span data-ttu-id="a1035-123">Une valeur qui indique si le nombre de destinataires externes est affiché.</span><span class="sxs-lookup"><span data-stu-id="a1035-123">A value that indicates whether the number of external recipients is shown.</span></span></li><li><span data-ttu-id="a1035-124">Liste des domaines internes.</span><span class="sxs-lookup"><span data-stu-id="a1035-124">A list of internal domains.</span></span></li><li><span data-ttu-id="a1035-125">Une valeur qui indique si les conseils de stratégie sont activés.</span><span class="sxs-lookup"><span data-stu-id="a1035-125">A value that indicates whether policy tips are enabled.</span></span></li><li><span data-ttu-id="a1035-126">Le seuil de délimiter large public pour indiquer si votre messagerie est considéré comme un grand nombre de destinataires.</span><span class="sxs-lookup"><span data-stu-id="a1035-126">The large audience cap threshold for indicating whether your mail is considered to have a large number of recipients.</span></span>  </li></ul>|
|<span data-ttu-id="a1035-127">Règles de protection</span><span class="sxs-lookup"><span data-stu-id="a1035-127">Protection rules</span></span>  <br/> | <ul><li><span data-ttu-id="a1035-128">Programme d’installation des règles de protection de votre client.</span><span class="sxs-lookup"><span data-stu-id="a1035-128">Protection rules setup for your client.</span></span></li><li><span data-ttu-id="a1035-129">Une liste des domaines internes à votre organisation.</span><span class="sxs-lookup"><span data-stu-id="a1035-129">A list of domains that are internal to your organization.</span></span>  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a><span data-ttu-id="a1035-130">Exemple de code : obtenir des informations de configuration de service pour des conseils de messagerie à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="a1035-130">Code example: Get service configuration information for mail tips by using EWS</span></span>

<span data-ttu-id="a1035-131">L’exemple de code suivant utilise l' [opération GetServiceConfiguration](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) pour demander des informations de configuration de service pour des conseils de messagerie.</span><span class="sxs-lookup"><span data-stu-id="a1035-131">The following code example uses the [GetServiceConfiguration operation](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) to request service configuration information for mail tips.</span></span> <span data-ttu-id="a1035-132">Vous pouvez demander des informations de configuration de service supplémentaires en ajoutant des éléments de [nom de configuration](http://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) avec des valeurs différentes.</span><span class="sxs-lookup"><span data-stu-id="a1035-132">You can request additional service configuration information by adding more [ConfigurationName](http://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) elements with different values.</span></span> 
  
```cs
private static void GetServiceConfiguration(ExchangeService service, NetworkCredential creds)
{ 
  // XML for the GetServiceConfiguration request SOAP envelope for mail tips configuration information.
  const string getServiceConfigurationRequest = 
    "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
    "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\"\n" +
    "               xmlns:m=\"http://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
    "               xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\" \n" +
    "               xmlns:soap=\"http://schemas.xmlsoap.org/soap/envelope/\"\n" +
    "               xmlns:xs=\"http://www.w3.org/2001/XMLSchema\">\n" +
    "  <soap:Header>\n" +
    "    <t:RequestServerVersion Version=\"Exchange2013\" />\n" +
    "  </soap:Header>\n" +
    "  <soap:Body>\n" +
    "    <m:GetServiceConfiguration>\n" +
    "      <m:ActingAs>\n" +
    "        <t:EmailAddress>user1@contoso.com</t:EmailAddress>\n" +
    "        <t:RoutingType>SMTP</t:RoutingType>\n" +
    "      </m:ActingAs>\n" +
    "      <m:RequestedConfiguration>\n" +
    "        <m:ConfigurationName>MailTips</m:ConfigurationName>\n" +
    "      </m:RequestedConfiguration>\n" +
    "    </m:GetServiceConfiguration>\n" +
    "  </soap:Body>\n" +
    "</soap:Envelope>";
  // Encoded GetServiceConfiguration operation request.
  byte[] payload = System.Text.Encoding.UTF8.GetBytes(getServiceConfigurationRequest);
  try
  {
    HttpWebRequest request = (HttpWebRequest)WebRequest.Create(service.Url);
    request.AllowAutoRedirect = false;
    request.Credentials = creds;
    request.Method = "POST";
    request.ContentType = "text/xml";
    Stream requestStream = request.GetRequestStream();
    requestStream.Write(payload, 0, payload.Length);
    requestStream.Close();
    HttpWebResponse response = (HttpWebResponse)request.GetResponse();
    if (response.StatusCode == HttpStatusCode.OK)
    {
      Stream responseStream = response.GetResponseStream();
      StreamReader reader = new StreamReader(responseStream);
      string responseFromServer = reader.ReadToEnd();
      Console.WriteLine("You will need to parse this response to get the configuration information:\n\n" + responseFromServer);
      reader.Close();
      responseStream.Close();
    }
    else
      throw new WebException(response.StatusDescription);
          
  }
  catch (WebException e)
  {
    Console.WriteLine(e.Message);
  }
}

```

## <a name="next-steps"></a><span data-ttu-id="a1035-133">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="a1035-133">Next steps</span></span>

<span data-ttu-id="a1035-134">Une fois que vous demandez les informations de configuration de service, utilisez la [classe XmlDocument](http://msdn.microsoft.com/en-us/library/system.xml.xmldocument.aspx) pour charger la réponse XML de sorte que vous pouvez analyser.</span><span class="sxs-lookup"><span data-stu-id="a1035-134">After you request service configuration information, use the [XmlDocument class](http://msdn.microsoft.com/en-us/library/system.xml.xmldocument.aspx) to load the response XML so that you can parse it.</span></span> <span data-ttu-id="a1035-135">Ensuite, en fonction de votre scénario, vous pouvez effectuer une des options suivantes :</span><span class="sxs-lookup"><span data-stu-id="a1035-135">Then, depending on your scenario, you can do one of the following:</span></span> 
  
- <span data-ttu-id="a1035-136">Utilisez l' [opération GetMailTips](http://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) pour obtenir des conseils pour les applications clientes à afficher aux utilisateurs de la messagerie.</span><span class="sxs-lookup"><span data-stu-id="a1035-136">Use the [GetMailTips operation](http://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) to get mail tips for client applications to display to users.</span></span> 
    
- <span data-ttu-id="a1035-137">Si la messagerie unifiée est activée, [Découvrez comment lire des éléments de boîte aux lettres](http://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) sur votre téléphone.</span><span class="sxs-lookup"><span data-stu-id="a1035-137">If UM is enabled, [learn about how to play mailbox items](http://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) over your phone.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="a1035-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a1035-138">See also</span></span>

- [<span data-ttu-id="a1035-139">Options de configuration pour EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a1035-139">Configuration options for EWS in Exchange</span></span>](configuration-options-for-ews-in-exchange.md)    
- [<span data-ttu-id="a1035-140">La configuration de vos applications EWS</span><span class="sxs-lookup"><span data-stu-id="a1035-140">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)    
- [<span data-ttu-id="a1035-141">Développer des clients de service web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="a1035-141">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

