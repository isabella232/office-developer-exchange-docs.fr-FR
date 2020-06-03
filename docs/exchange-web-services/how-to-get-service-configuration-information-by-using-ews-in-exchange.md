---
title: Obtenir des informations de configuration de service à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9379740a-96e1-490d-a229-0f9937c548d2
description: Découvrez comment obtenir des informations de configuration de service pour la messagerie unifiée, les Wizz, les conseils de messagerie et les règles de protection d’EWS dans Exchange.
ms.openlocfilehash: 7546d9524f1e004eda2bdc55687fb44beafa44af
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528005"
---
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a><span data-ttu-id="3ea9b-103">Obtenir des informations de configuration de service à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3ea9b-103">Get service configuration information by using EWS in Exchange</span></span>

<span data-ttu-id="3ea9b-104">Découvrez comment obtenir des informations de configuration de service pour la messagerie unifiée, les Wizz, les conseils de messagerie et les règles de protection d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-104">Find out how to get service configuration information for UM, policy nudges, mail tips, and protection rules from EWS in Exchange.</span></span>
  
<span data-ttu-id="3ea9b-105">Votre application EWS fonctionne-t-elle avec la messagerie unifiée, les Wizz, les conseils de messagerie ou les règles de protection ?</span><span class="sxs-lookup"><span data-stu-id="3ea9b-105">Does your EWS application work with Unified Messaging (UM), policy nudges, mail tips, or protection rules?</span></span> <span data-ttu-id="3ea9b-106">Si c’est le cas, votre application devra appeler l' [opération GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) pour obtenir les informations de configuration de service dont elle a besoin.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-106">If so, your application will need to call the [GetServiceConfiguration operation](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) to get the service configuration information that it needs.</span></span> <span data-ttu-id="3ea9b-107">L’opération **GetServiceConfiguration** renvoie les informations de configuration propres à chacune de ces fonctionnalités EWS.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-107">The **GetServiceConfiguration** operation returns configuration information that is specific to each of these EWS features.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="3ea9b-108">L’API managée EWS n’implémente pas cette fonctionnalité.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-108">The EWS Managed API does not implement this functionality.</span></span> 
  
<span data-ttu-id="3ea9b-109">**Tableau 1. Informations de configuration renvoyées par l’opération GetServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="3ea9b-109">**Table 1. Configuration information that the GetServiceConfiguration operation returns**</span></span>

|<span data-ttu-id="3ea9b-110">Fonctionnalité EWS</span><span class="sxs-lookup"><span data-stu-id="3ea9b-110">EWS feature</span></span>|<span data-ttu-id="3ea9b-111">L’opération GetServiceConfiguration renvoie...</span><span class="sxs-lookup"><span data-stu-id="3ea9b-111">GetServiceConfiguration operation returns…</span></span>|
|:-----|:-----|
|<span data-ttu-id="3ea9b-112">MESSAGERIE</span><span class="sxs-lookup"><span data-stu-id="3ea9b-112">UM</span></span>  <br/> | <ul><li><span data-ttu-id="3ea9b-113">Valeur qui indique si la messagerie unifiée est activée.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-113">A value that indicates whether UM is enabled.</span></span></li><li><span data-ttu-id="3ea9b-114">Valeur qui indique si la fonction émettre au téléphone est activée.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-114">A value that indicates whether play on phone is enabled.</span></span></li><li><span data-ttu-id="3ea9b-115">Chaîne de numérotation lire sur le téléphone.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-115">The play on phone dial string.</span></span></li></ul> |
|<span data-ttu-id="3ea9b-116">Wizz de stratégie</span><span class="sxs-lookup"><span data-stu-id="3ea9b-116">Policy nudges</span></span>  <br/> | <ul><li><span data-ttu-id="3ea9b-117">Les stratégies sont déplacées pour être affichées dans votre client.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-117">Policy nudges for display in your client.</span></span></li></ul> |
|<span data-ttu-id="3ea9b-118">Infos-courrier</span><span class="sxs-lookup"><span data-stu-id="3ea9b-118">Mail tips</span></span>  <br/> | <ul><li><span data-ttu-id="3ea9b-119">Valeur qui indique si les conseils de messagerie sont activés.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-119">A value that indicates whether mail tips are enabled.</span></span></li><li><span data-ttu-id="3ea9b-120">Nombre maximal de destinataires par demande.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-120">The maximum number of recipients per request.</span></span></li><li><span data-ttu-id="3ea9b-121">Taille maximale des messages.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-121">The maximum message size.</span></span></li><li><span data-ttu-id="3ea9b-122">Le seuil d’audience élevée.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-122">The large audience threshold.</span></span></li><li><span data-ttu-id="3ea9b-123">Valeur qui indique si le nombre de destinataires externes est affiché.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-123">A value that indicates whether the number of external recipients is shown.</span></span></li><li><span data-ttu-id="3ea9b-124">Liste des domaines internes.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-124">A list of internal domains.</span></span></li><li><span data-ttu-id="3ea9b-125">Valeur qui indique si les conseils de stratégie sont activés.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-125">A value that indicates whether policy tips are enabled.</span></span></li><li><span data-ttu-id="3ea9b-126">Seuil de capitalisation de grande audience pour indiquer si votre courrier est considéré comme un grand nombre de destinataires.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-126">The large audience cap threshold for indicating whether your mail is considered to have a large number of recipients.</span></span>  </li></ul>|
|<span data-ttu-id="3ea9b-127">Règles de protection</span><span class="sxs-lookup"><span data-stu-id="3ea9b-127">Protection rules</span></span>  <br/> | <ul><li><span data-ttu-id="3ea9b-128">Configuration des règles de protection pour votre client.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-128">Protection rules setup for your client.</span></span></li><li><span data-ttu-id="3ea9b-129">Liste de domaines internes à votre organisation.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-129">A list of domains that are internal to your organization.</span></span>  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a><span data-ttu-id="3ea9b-130">Exemple de code : obtenir les informations de configuration de service pour les conseils de messagerie à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="3ea9b-130">Code example: Get service configuration information for mail tips by using EWS</span></span>

<span data-ttu-id="3ea9b-131">L’exemple de code suivant utilise l' [opération GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) pour demander des informations de configuration de service pour les conseils de messagerie.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-131">The following code example uses the [GetServiceConfiguration operation](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) to request service configuration information for mail tips.</span></span> <span data-ttu-id="3ea9b-132">Vous pouvez demander des informations de configuration de service supplémentaires en ajoutant des éléments [ConfigurationName](https://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) ayant des valeurs différentes.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-132">You can request additional service configuration information by adding more [ConfigurationName](https://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) elements with different values.</span></span> 
  
```cs
private static void GetServiceConfiguration(ExchangeService service, NetworkCredential creds)
{ 
  // XML for the GetServiceConfiguration request SOAP envelope for mail tips configuration information.
  const string getServiceConfigurationRequest = 
    "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
    "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\"\n" +
    "               xmlns:m=\"https://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
    "               xmlns:t=\"https://schemas.microsoft.com/exchange/services/2006/types\" \n" +
    "               xmlns:soap=\"https://schemas.xmlsoap.org/soap/envelope/\"\n" +
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

## <a name="next-steps"></a><span data-ttu-id="3ea9b-133">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="3ea9b-133">Next steps</span></span>

<span data-ttu-id="3ea9b-134">Une fois que vous avez demandé des informations de configuration de service, utilisez la [classe XmlDocument](https://msdn.microsoft.com/library/system.xml.xmldocument.aspx) pour charger le code XML de réponse afin de pouvoir l’analyser.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-134">After you request service configuration information, use the [XmlDocument class](https://msdn.microsoft.com/library/system.xml.xmldocument.aspx) to load the response XML so that you can parse it.</span></span> <span data-ttu-id="3ea9b-135">Ensuite, en fonction de votre scénario, vous pouvez effectuer l’une des opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="3ea9b-135">Then, depending on your scenario, you can do one of the following:</span></span> 
  
- <span data-ttu-id="3ea9b-136">Utilisez l' [opération GetMailTips](https://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) pour obtenir des conseils de messagerie pour les applications clientes à afficher aux utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-136">Use the [GetMailTips operation](https://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) to get mail tips for client applications to display to users.</span></span> 
    
- <span data-ttu-id="3ea9b-137">Si la messagerie unifiée est activée, [Découvrez comment lire des éléments de boîte aux lettres](https://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) sur votre téléphone.</span><span class="sxs-lookup"><span data-stu-id="3ea9b-137">If UM is enabled, [learn about how to play mailbox items](https://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) over your phone.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="3ea9b-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3ea9b-138">See also</span></span>

- [<span data-ttu-id="3ea9b-139">Options de configuration pour EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3ea9b-139">Configuration options for EWS in Exchange</span></span>](configuration-options-for-ews-in-exchange.md)    
- [<span data-ttu-id="3ea9b-140">Configuration de votre application EWS</span><span class="sxs-lookup"><span data-stu-id="3ea9b-140">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)    
- [<span data-ttu-id="3ea9b-141">Développer des clients de service web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="3ea9b-141">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

