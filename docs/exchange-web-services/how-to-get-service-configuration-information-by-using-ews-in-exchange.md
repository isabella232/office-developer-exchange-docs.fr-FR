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
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a>Obtenir des informations de configuration de service à l’aide de EWS dans Exchange

Découvrez comment obtenir des informations de configuration de service de messagerie unifiée, déplacer de stratégie, les conseils de messagerie et les règles de protection d’EWS dans Exchange.
  
Votre application EWS fonctionne avec la messagerie unifiée (MU), déplacer de stratégie, les conseils de messagerie ou les règles de protection ? Dans ce cas, votre application vous devrez appeler l' [opération GetServiceConfiguration](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) pour obtenir les informations de configuration de service qui lui sont nécessaires. L’opération **GetServiceConfiguration** renvoie des informations de configuration spécifiques à chacune de ces fonctionnalités EWS. 
  
> [!NOTE]
> L’API managée EWS n’implémente pas cette fonctionnalité. 
  
**Le tableau 1. Informations de configuration qui renvoie l’opération GetServiceConfiguration**

|Fonctionnalité EWS|Opération GetServiceConfiguration renvoie...|
|:-----|:-----|
|MESSAGERIE UNIFIÉE  <br/> | <ul><li>Une valeur qui indique si la messagerie unifiée est activée.</li><li>Une valeur qui indique si l’option Lire sur le téléphone est activée.</li><li>La lire sur la chaîne de numérotation téléphonique.</li></ul> |
|Déplacer de stratégie  <br/> | <ul><li>Stratégie est déplacée pour l’affichage de votre client.</li></ul> |
|Conseils de messagerie  <br/> | <ul><li>Une valeur qui indique si les conseils de la messagerie sont activées.</li><li>Le nombre maximal de destinataires par demande.</li><li>La taille maximale des messages.</li><li>Le seuil de large public.</li><li>Une valeur qui indique si le nombre de destinataires externes est affiché.</li><li>Liste des domaines internes.</li><li>Une valeur qui indique si les conseils de stratégie sont activés.</li><li>Le seuil de délimiter large public pour indiquer si votre messagerie est considéré comme un grand nombre de destinataires.  </li></ul>|
|Règles de protection  <br/> | <ul><li>Programme d’installation des règles de protection de votre client.</li><li>Une liste des domaines internes à votre organisation.  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a>Exemple de code : obtenir des informations de configuration de service pour des conseils de messagerie à l’aide de EWS

L’exemple de code suivant utilise l' [opération GetServiceConfiguration](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) pour demander des informations de configuration de service pour des conseils de messagerie. Vous pouvez demander des informations de configuration de service supplémentaires en ajoutant des éléments de [nom de configuration](http://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) avec des valeurs différentes. 
  
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

## <a name="next-steps"></a>Étapes suivantes

Une fois que vous demandez les informations de configuration de service, utilisez la [classe XmlDocument](http://msdn.microsoft.com/en-us/library/system.xml.xmldocument.aspx) pour charger la réponse XML de sorte que vous pouvez analyser. Ensuite, en fonction de votre scénario, vous pouvez effectuer une des options suivantes : 
  
- Utilisez l' [opération GetMailTips](http://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) pour obtenir des conseils pour les applications clientes à afficher aux utilisateurs de la messagerie. 
    
- Si la messagerie unifiée est activée, [Découvrez comment lire des éléments de boîte aux lettres](http://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) sur votre téléphone. 
    
## <a name="see-also"></a>Voir aussi

- [Options de configuration pour EWS dans Exchange](configuration-options-for-ews-in-exchange.md)    
- [La configuration de vos applications EWS](setting-up-your-ews-application.md)    
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    

