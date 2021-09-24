---
title: Obtenir des informations de configuration de service à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 9379740a-96e1-490d-a229-0f9937c548d2
description: Découvrez comment obtenir des informations de configuration de service pour la messagerie unée, les conseils de stratégie, les conseils de messagerie et les règles de protection d’EWS dans Exchange.
ms.openlocfilehash: 30d4058104726c79f473a88a09398689675b988d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513170"
---
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a>Obtenir des informations de configuration de service à l’aide d’EWS dans Exchange

Découvrez comment obtenir des informations de configuration de service pour la messagerie unée, les conseils de stratégie, les conseils de messagerie et les règles de protection d’EWS dans Exchange.
  
Votre application EWS fonctionne-t-elle avec la messagerie unifiée, les changements de stratégie, les conseils de messagerie ou les règles de protection ? Si c’est le cas, votre application devra appeler l’opération [GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) pour obtenir les informations de configuration de service dont elle a besoin. **L’opération GetServiceConfiguration** renvoie des informations de configuration spécifiques à chacune de ces fonctionnalités EWS. 
  
> [!NOTE]
> L’API managée EWS n’implémente pas cette fonctionnalité. 
  
**Tableau 1. Informations de configuration que renvoie l’opération GetServiceConfiguration**

|Fonctionnalité EWS|L’opération GetServiceConfiguration renvoie...|
|:-----|:-----|
|UM  <br/> | <ul><li>Valeur qui indique si la um est activée.</li><li>Valeur qui indique si la lecture sur le téléphone est activée.</li><li>Chaîne de numérotation de lecture sur téléphone.</li></ul> |
|Changements de stratégie  <br/> | <ul><li>La stratégie doit être affichée dans votre client.</li></ul> |
|Infos-courrier  <br/> | <ul><li>Valeur qui indique si les infos-courrier sont activées.</li><li>Nombre maximal de destinataires par demande.</li><li>Taille maximale du message.</li><li>Seuil de large public.</li><li>Valeur qui indique si le nombre de destinataires externes est affiché.</li><li>Liste des domaines internes.</li><li>Valeur qui indique si les conseils de stratégie sont activés.</li><li>Seuil de large audience limite pour indiquer si votre courrier électronique est considéré comme étant un grand nombre de destinataires.  </li></ul>|
|Règles de protection  <br/> | <ul><li>Configuration des règles de protection pour votre client.</li><li>Liste des domaines internes à votre organisation.  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a>Exemple de code : obtenir des informations de configuration de service pour les conseils de messagerie à l’aide d’EWS

L’exemple de code suivant utilise [l’opération GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) pour demander des informations de configuration de service pour les conseils de messagerie. Vous pouvez demander des informations de configuration de service supplémentaires en ajoutant d’autres [éléments ConfigurationName](https://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) avec des valeurs différentes. 
  
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

Après avoir demandé des informations de configuration de service, utilisez la classe [XmlDocument](https://msdn.microsoft.com/library/system.xml.xmldocument.aspx) pour charger le XML de réponse afin de pouvoir l’utiliser. Ensuite, en fonction de votre scénario, vous pouvez faire l’une des choses suivantes : 
  
- Utilisez [l’opération GetMailTips pour](https://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) obtenir des conseils de messagerie pour les applications clientes à afficher aux utilisateurs. 
    
- Si la messagerie un utilisateur est activée, découvrez comment lire des éléments de boîte [aux lettres](https://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) sur votre téléphone. 
    
## <a name="see-also"></a>Voir aussi

- [Options de configuration pour EWS dans Exchange](configuration-options-for-ews-in-exchange.md)    
- [La configuration de vos applications EWS](setting-up-your-ews-application.md)    
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    

