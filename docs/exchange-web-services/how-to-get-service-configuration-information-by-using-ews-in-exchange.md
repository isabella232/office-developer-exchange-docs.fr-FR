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
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a>Obtenir des informations de configuration de service à l’aide d’EWS dans Exchange

Découvrez comment obtenir des informations de configuration de service pour la messagerie unifiée, les Wizz, les conseils de messagerie et les règles de protection d’EWS dans Exchange.
  
Votre application EWS fonctionne-t-elle avec la messagerie unifiée, les Wizz, les conseils de messagerie ou les règles de protection ? Si c’est le cas, votre application devra appeler l' [opération GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) pour obtenir les informations de configuration de service dont elle a besoin. L’opération **GetServiceConfiguration** renvoie les informations de configuration propres à chacune de ces fonctionnalités EWS. 
  
> [!NOTE]
> L’API managée EWS n’implémente pas cette fonctionnalité. 
  
**Tableau 1. Informations de configuration renvoyées par l’opération GetServiceConfiguration**

|Fonctionnalité EWS|L’opération GetServiceConfiguration renvoie...|
|:-----|:-----|
|MESSAGERIE  <br/> | <ul><li>Valeur qui indique si la messagerie unifiée est activée.</li><li>Valeur qui indique si la fonction émettre au téléphone est activée.</li><li>Chaîne de numérotation lire sur le téléphone.</li></ul> |
|Wizz de stratégie  <br/> | <ul><li>Les stratégies sont déplacées pour être affichées dans votre client.</li></ul> |
|Infos-courrier  <br/> | <ul><li>Valeur qui indique si les conseils de messagerie sont activés.</li><li>Nombre maximal de destinataires par demande.</li><li>Taille maximale des messages.</li><li>Le seuil d’audience élevée.</li><li>Valeur qui indique si le nombre de destinataires externes est affiché.</li><li>Liste des domaines internes.</li><li>Valeur qui indique si les conseils de stratégie sont activés.</li><li>Seuil de capitalisation de grande audience pour indiquer si votre courrier est considéré comme un grand nombre de destinataires.  </li></ul>|
|Règles de protection  <br/> | <ul><li>Configuration des règles de protection pour votre client.</li><li>Liste de domaines internes à votre organisation.  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a>Exemple de code : obtenir les informations de configuration de service pour les conseils de messagerie à l’aide d’EWS

L’exemple de code suivant utilise l' [opération GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) pour demander des informations de configuration de service pour les conseils de messagerie. Vous pouvez demander des informations de configuration de service supplémentaires en ajoutant des éléments [ConfigurationName](https://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) ayant des valeurs différentes. 
  
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

## <a name="next-steps"></a>Étapes suivantes

Une fois que vous avez demandé des informations de configuration de service, utilisez la [classe XmlDocument](https://msdn.microsoft.com/library/system.xml.xmldocument.aspx) pour charger le code XML de réponse afin de pouvoir l’analyser. Ensuite, en fonction de votre scénario, vous pouvez effectuer l’une des opérations suivantes : 
  
- Utilisez l' [opération GetMailTips](https://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) pour obtenir des conseils de messagerie pour les applications clientes à afficher aux utilisateurs. 
    
- Si la messagerie unifiée est activée, [Découvrez comment lire des éléments de boîte aux lettres](https://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) sur votre téléphone. 
    
## <a name="see-also"></a>Voir aussi

- [Options de configuration pour EWS dans Exchange](configuration-options-for-ews-in-exchange.md)    
- [Configuration de votre application EWS](setting-up-your-ews-application.md)    
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    

