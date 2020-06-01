---
title: Obtenir des paramètres de domaine à partir du serveur Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 2f9acb81-5135-4f72-94e8-65c235d725e6
description: Découvrez comment obtenir les paramètres de domaine à partir d’un serveur Exchange à l’aide du service de découverte automatique.
localization_priority: Priority
ms.openlocfilehash: e77810089b77f614f6bca064b2e5cf6bde2bff7c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455806"
---
# <a name="get-domain-settings-from-an-exchange-server"></a>Obtenir des paramètres de domaine à partir du serveur Exchange

Découvrez comment obtenir les paramètres de domaine à partir d’un serveur Exchange à l’aide du service de découverte automatique.
  
Vous pouvez récupérer les informations de configuration d’un domaine de messagerie en utilisant le service de découverte automatique. Le service de découverte automatique fournit à votre application un processus de connexion au point de terminaison de service correct pour un domaine spécifique.
  
Vous pouvez utiliser l’une des technologies de développement suivantes pour accéder au service de découverte automatique :
  
- API managée des services web Exchange (EWS)
    
- EWS
    
    Si vous utilisez EWS, recourez aux méthodes suivantes pour extraire des paramètres utilisateur :
    
  - Service de découverte automatique basé sur SOAP
    
  - Service de découverte automatique XML (POX)
    
  - Proxy généré automatiquement à partir du service de détection automatique SOAP ou XML
    
    Pour plus d'informations sur ces méthodes, reportez-vous à la section [Découverte automatique pour Exchange](autodiscover-for-exchange.md).
    
L’API managée EWS fournit une interface basée sur des objets pour récupérer les paramètres de l’utilisateur. Si votre application cliente utilise du code managé, nous vous recommandons de choisir l’API managée EWS. L’interface API managée EWS optimisée pour un modèle d’objet simple présente des performances supérieures au proxy de service web généré automatiquement par défaut. 
  
Si vous utilisez EWS, nous vous conseillons d’opter pour le service de découverte automatique SOAP, car il prend en charge un ensemble de fonctionnalités plus riche que le service de découverte automatique POX.
  
Le service de découverte automatique renvoie uniquement les paramètres de configuration requis. Le tableau suivant répertorie les paramètres de configuration de domaine que le service de découverte automatique peut renvoyer.
  
**Tableau 1 : Paramètres de configuration de domaine**

|**Paramètre de configuration**|**Description**|
|:-----|:-----|
|ExternalEwsUrl  <br/> |URL EWS externe.  <br/> |
|ExternalEwsVersion  <br/> |Version du serveur Exchange qui héberge l’URL EWS.  <br/> |
   
## <a name="prerequisites-for-getting-domain-settings"></a>Conditions préalables requises pour l’obtention de paramètres du domaine
<a name="bk_Prereq"> </a>

Avant de créer une application qui se connecte au service de découverte automatique pour obtenir les paramètres de domaine, vérifiez que vous avez accès à ce qui suit :
  
- Exchange Online, Exchange Online dans le cadre d’Office 365 ou un serveur qui exécute une version d’Exchange égale ou supérieure à Exchange 2007. Si vous utilisez le service de découverte automatique basé sur SOAP EWS, un serveur qui exécute une version d’Exchange égale ou supérieure à Exchange 2010.
    
- Un serveur Exchange qui est configuré pour accepter les connexions depuis votre application cliente. Pour plus d'informations sur la configuration de votre serveur Exchange, reportez-vous à la rubrique [Contrôle de l'accès aux applications de client pour EWS dans Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
- Un compte autorisé à utiliser EWS. Pour plus d'informations sur la configuration d'un compte, reportez-vous à la rubrique [Contrôle de l'accès aux applications de client pour EWS dans Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
> [!NOTE]
> Si vous utilisez l’API managée EWS, vous devez fournir un rappel de validation de certificat dans certains cas. Vous aurez peut-être également besoin d’un rappel de validation de certificat avec certaines bibliothèques proxy générées, telles que celles créées par Visual Studio. Pour plus d'informations, reportez-vous à la rubrique [Valider un certificat de serveur pour l'API managée EWS](how-to-validate-a-server-certificate-for-the-ews-managed-api.md). 
  
### <a name="core-concepts-for-getting-domain-settings"></a>Les concepts de base pour obtenir des paramètres de domaine
<a name="bk_Core"> </a>

Avant d’utiliser la découverte automatique pour obtenir des paramètres de domaine, vous devez être familiarisé avec les concepts répertoriés dans le tableau suivant.
  
|**Concept**|**Description**|
|:-----|:-----|
|[Découverte automatique pour Exchange](autodiscover-for-exchange.md) <br/> |Fournit une vue d’ensemble du fonctionnement du service de découverte automatique.  <br/> |
|[Utiliser la découverte automatique pour trouver des points de connexion](how-to-use-autodiscover-to-find-connection-points.md) <br/> |Décrit le processus utilisé par le service de découverte automatique pour rediriger votre application client vers le point de terminaison de service correct.  <br/> |
   
Si vous utilisez l'API managée EWS, vous gérez votre connexion à EWS à l'aide de la classe [Microsoft.Exchange.WebServices.Data.ExchangeService](https://msdn.microsoft.com/library/exchange/dd635811%28v=exchg.80%29.aspx) dans l'espace de noms [Microsoft.Exchange.WebServices.Data](https://msdn.microsoft.com/library/exchange/dd633907%28v=exchg.80%29.aspx). Les exemples de code de cette section supposent que vous référencez les espaces de noms suivants dans votre code : 
  
- **System.Net**
    
- **Microsoft.Exchange.WebServices.Data.ExchangeService**
    
## <a name="get-domain-settings-by-using-the-ews-managed-api"></a>Obtenir les paramètres de domaine à l’aide de l’API managée EWS
<a name="bk_Managed"> </a>

Si vous utilisez l'API managée EWS, vous pouvez recourir à la méthode [Microsoft.Exchange.WebServices.Data.AutodiscoverSettings.GetUserSettings](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) de l'objet [Microsoft.Exchange.WebServices.Data.AutodiscoverService](https://msdn.microsoft.com/library/exchange/dd634321%28v=exchg.80%29.aspx) pour générer la requête qui récupère les informations de configuration pour un domaine, comme illustré dans l'exemple suivant. Dans cet exemple, seuls certains des paramètres de domaine possibles sont demandés, et seuls les paramètres demandés sont renvoyés à partir du serveur. 
  
```cs
AutodiscoverService autodiscoverService = new AutodiscoverService("domain.contoso.com");
autodiscoverService.Credentials = new NetworkCredential("User1", "password", "domain.contoso.com");
// Submit a request and get the settings. The response contains only the
// settings that are requested, if they exist.
GetDomainSettingsResponse domainresponse = autodiscoverService.GetDomainSettings(
    "domain",
    ExchangeVersion.Exchang2013,
    DomainSettingName.ExternalEwsUrl,
    DomainSettingName.ExternalEwsVersion);
```

Vous pouvez analyser la collection retournée pour accéder à chaque paire clé/valeur. L’exemple suivant montre comment analyser chaque élément retourné et affiche le nom et la valeur de chaque paire clé/valeur.
  
```cs
// Display each retrieved value. The settings are part of a key/value pair.
foreach (KeyValuePair<DomainSettingName, Object> domainsetting in domainresponse.Settings)
{
    Console.WriteLine(domainsetting.Key.ToString() + ": " + domainsetting.Value.ToString());
}
```

Vous pouvez également obtenir la valeur d'un paramètre spécifique. Dans l'exemple suivant, le paramètre **ExternalEwsUrl** doit être affiché. 
  
```cs
// Display a specific setting, such as ExternalEwsUrl.
Console.WriteLine(domainresponse.Settings[DomainSettingName.ExternalEwsUrl]);
```

## <a name="get-user-settings-by-using-ews-soap-autodiscover"></a>Obtenir les paramètres de l’utilisateur à l’aide de la découverte automatique SOAP EWS
<a name="bk_SOAP"> </a>

L’exemple suivant représente une demande XML SOAP destinée à extraire les deux paramètres de domaine auprès du service de découverte automatique.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetDomainSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetDomainSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Domains>
          <a:Domain>domain</a:Domain>
        </a:Domains>
        <a:RequestedSettings>
          <a:Setting>ExternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsVersion</a:Setting>
        </a:RequestedSettings>
        <a:RequestedVersion>Exchange2013</a:RequestedVersion>
      </a:Request>
    </a:GetDomainSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>
```

L’exemple suivant illustre la réponse XML renvoyée par le serveur après analyse de la demande du client.
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/
          Autodiscover/Autodiscover/GetDomainSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
          xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>160</h:MajorBuildNumber>
      <h:MinorBuildNumber>4</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetDomainSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <DomainResponses>
          <DomainResponse>
            <ErrorCode>NoError</ErrorCode>
            <ErrorMessage>No error.</ErrorMessage>
            <DomainSettingErrors />
            <DomainSettings>
              <DomainSetting i:type="DomainStringSetting">
                <Name>ExternalEwsUrl</Name>
                <Value>https://failover.exchange.microsoft.com/ews/exchange.asmx</Value>
              </DomainSetting>
              <DomainSetting i:type="DomainStringSetting">
                <Name>ExternalEwsVersion</Name>
                <Value>15.00.0085.000</Value>
              </DomainSetting>
            </DomainSettings>
            <RedirectTarget i:nil="true" />
          </DomainResponse>
        </DomainResponses>
      </Response>
    </GetDomainSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a>Étapes suivantes
<a name="bk_Next"> </a>

Les paramètres de domaine fournissent les informations de base dont votre client a besoin pour se connecter à EWS. Ces informations vous permettent de vous connecter à EWS. Vous pouvez également récupérer les paramètres de configuration supplémentaires pour un compte de messagerie à partir du serveur. Pour plus d’informations, consultez l’article suivant :
  
- [Obtenir les paramètres de l'utilisateur Exchange à l'aide de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a>Voir aussi


- [Configuration de votre application EWS](setting-up-your-ews-application.md)
    
- [Référence de service web de découverte automatique pour Exchange](https://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)
    
- [Référence EWS pour Exchange](https://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    

