---
title: Utiliser la découverte automatique pour rechercher les points de connexion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 03896542-549b-4c45-973c-98f9025ea26c
description: Découvrez comment utiliser le service de découverte automatique pour diriger votre application cliente vers le serveur Exchange approprié.
ms.openlocfilehash: 653fcd1c094c23c3e89e903b7194b96720802b51
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754953"
---
# <a name="use-autodiscover-to-find-connection-points"></a>Utiliser la découverte automatique pour rechercher les points de connexion

Découvrez comment utiliser le service de découverte automatique pour diriger votre application cliente vers le serveur Exchange approprié.
  
Le service de découverte automatique Exchange fournit à votre application client avec les paramètres de configuration de comptes de messagerie qui sont hébergées sur Exchange Online, Exchange Online dans le cadre d’Office 365 ou un serveur Exchange qui exécute une version d’Exchange commençant par Exchange 2013. Le service de découverte automatique est un service web qui fournit des paramètres de configuration. Le service de découverte automatique est un service web qui fournit des informations de configuration Exchange server pour votre application cliente. Applications clientes utilisent la découverte automatique pour déterminer le point de terminaison du service de découverte automatique pour une boîte aux lettres spécifique. Cet article explique comment suivre les réponses à partir d’un serveur Exchange pour rechercher le point de terminaison correct. 
  
Pour plus d’informations sur la façon d’obtenir des paramètres de configuration d’adresse de messagerie, voir [obtenir les paramètres utilisateur à partir d’Exchange à l’aide de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) et [obtenir les paramètres de domaine à partir d’un serveur Exchange](how-to-get-domain-settings-from-an-exchange-server.md).
  
> [!NOTE]
> Le processus pour rechercher le point de terminaison correct fait partie de la demande de l’utilisateur ou les paramètres de domaine. Le service de découverte automatique utilise une série de réponses de redirection pour envoyer l’application cliente au point de terminaison correct pour une adresse de messagerie. 
  
Vous pouvez utiliser une des technologies de développement Exchange suivantes pour accéder au service de découverte automatique :
  
> [!NOTE]
> Pour plus d’informations sur ces technologies de développement Exchange, voir [Explorer l’API managée EWS, EWS et des services web Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md). 
  
- API managée des services web Exchange (EWS)
    
- EWS
    
    Si vous utilisez EWS, recourez aux méthodes suivantes pour extraire des paramètres utilisateur :
    
  - Service de découverte automatique basé sur SOAP
    
  - Service de découverte automatique XML (POX)
    
  - Proxy généré automatiquement à partir du service de détection automatique SOAP ou XML
    
    Pour plus d'informations sur ces méthodes, reportez-vous à la section [Découverte automatique pour Exchange](autodiscover-for-exchange.md).
    
L'API managée EWS fournit une interface basée sur des objets pour récupérer les paramètres de l'utilisateur. Si votre application cliente utilise du code managé, nous vous recommandons de choisir l'API managée EWS. L'interface API managée EWS optimisée pour un modèle d'objet simple présente des performances supérieures au proxy de service web généré automatiquement par défaut. 
  
Si vous utilisez EWS, nous vous conseillons d'opter pour le service de découverte automatique SOAP, car il prend en charge un ensemble de fonctionnalités plus riche que le service de découverte automatique POX.
  
## <a name="prerequisites-for-finding-an-endpoint"></a>Conditions préalables pour la recherche d’un point de terminaison
<a name="bk_Prereq"> </a>

Avant de pouvoir créer une application cliente qui utilise le service de découverte automatique, vous devez avoir accès à ce qui suit :
  
- Exchange Online ou un serveur qui exécute une version d’Exchange de démarrer avec Exchange 2007 SP1. Si vous utilisez le service Autodiscover basés sur SOAP, Exchange Online ou une version d’Exchange commençant par Exchange 2010.
    
- Un serveur Exchange qui est configuré pour accepter les connexions depuis votre application cliente. Pour plus d'informations sur la configuration de votre serveur Exchange, reportez-vous à la rubrique [Contrôle de l'accès aux applications de client pour EWS dans Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
- Un compte autorisé à utiliser EWS. Pour plus d'informations sur la configuration d'un compte, reportez-vous à la rubrique [Contrôle de l'accès aux applications de client pour EWS dans Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
> [!NOTE]
> [!REMARQUE] Si vous utilisez l'API managée EWS, vous devez fournir un rappel de validation de certificat dans certains cas. Vous aurez peut-être également besoin d'un rappel de validation de certificat avec certaines bibliothèques proxy générées, telles que celles qui sont créées par Visual Studio. Pour plus d’informations, voir [valider un certificat de serveur pour l’API managée EWS](how-to-validate-a-server-certificate-for-the-ews-managed-api.md). 
  
### <a name="core-concepts-for-finding-an-endpoint"></a>Concepts de base pour la recherche d’un point de terminaison
<a name="bk_Core"> </a>

Avant d’utiliser la découverte automatique pour trouver un point de terminaison, vous devez connaître avec les concepts figurant dans le tableau suivant.
  
|**Concept**|**Description**|
|:-----|:-----|
|[Découverte automatique pour Exchange](autodiscover-for-exchange.md) <br/> |Fournit une vue d'ensemble du fonctionnement du service de découverte automatique.  <br/> |
   
Si vous utilisez l'API managée EWS, vous gérez votre connexion à EWS à l'aide de la classe [Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) dans l'espace de noms [Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/en-us/library/dd633907%28v=exchg.80%29.aspx). Pour utiliser les exemples de code d’API managées dans cet article, vous devez faire référence les espaces de noms suivants dans votre code : 
  
- **System.Net**
    
- **Microsoft.Exchange.WebServices.Data.ExchangeService**
    
## <a name="find-the-correct-endpoint-by-using-the-ews-managed-api"></a>Rechercher le point de terminaison correct à l’aide de l’API managée EWS
<a name="bk_Managed"> </a>

Si vous utilisez l’API managée EWS, les appels vers le service de découverte automatique sont gérés par la classe **ExchangeService** . Pour déterminer le point de terminaison correct pour un compte de messagerie, vous appelez la méthode **AutodiscoverUrl** sur un objet **[ExchangeService]** . L’exemple de code suivant montre comment définir le point de terminaison EWS web services pour une adresse de messagerie au fichier Exchange.asmx sur le serveur d’accès au Client approprié à l’aide de l’API managée EWS. 
  
```cs
NetworkCredential credentials = new NetworkCredential(securelyStoredEmail, securelyStoredPassword);
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2013);
service.Credentials = credentials;
service.AutodiscoverUrl("User1@contoso.com");
```

## <a name="find-the-correct-endpoint-by-using-ews"></a>Rechercher le point de terminaison correct à l’aide de EWS
<a name="bk_SOAP"> </a>

Le service de découverte automatique SOAP peut utiliser une série de demandes et réponses pour diriger votre application au point de terminaison correct pour EWS. Pour plus d’informations sur la façon de déterminer le point de terminaison correct pour un compte de messagerie, voir [service de découverte automatique pour Exchange](autodiscover-for-exchange.md). Les exemples de code XML suivants montrent la série de demandes et réponses que vous pouvez vous attendre lors d’une demande SOAP Autodiscover pour rechercher le point de terminaison correct.
  
### <a name="soap-autodiscover-endpoint-request"></a>Demande de point de terminaison SOAP découverte automatique

L’exemple suivant montre une requête XML qui est envoyée au service de découverte automatique pour rechercher le point de terminaison correct.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://mail.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>User1@Contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>InternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsUrl</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

### <a name="soap-autodiscover-redirection-response"></a>Réponse de redirection SOAP découverte automatique

Le service de découverte automatique peut répondre avec une des deux réponses de redirection : une redirection HTTP 302, ou une réponse de redirection SOAP. Si la réponse du serveur Exchange est une redirection HTTP 302, l’application cliente doit valider que l’adresse de la redirection est acceptable et suivez la réponse de redirection.
  
> [! Remarque sur la sécurité] pour les critères de validation d’une réponse de redirection, voir [découverte automatique pour Exchange](autodiscover-for-exchange.md). 
  
Si le service de découverte automatique renvoie une réponse de redirection indiquée par l’élément [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) de l’élément de **réponse utilisateur** , votre application cliente doit utiliser l’élément **RedirectTarget** pour construire une nouvelle demande de paramètres qui est envoyé au serveur spécifié dans la réponse de redirection. L’exemple suivant montre une réponse de redirection à partir du serveur. 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>682</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>RedirectAddress</ErrorCode>
            <ErrorMessage>Redirection address.</ErrorMessage>
            <RedirectTarget>User1@mail.Contoso.com</RedirectTarget>
            <UserSettingErrors />
            <UserSettings />
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>

```

Après une redirection, le client utilise l’URL de redirection pour préparer une autre requête. Le code suivant montre un exemple de la demande que vous créez à partir de la réponse de redirection.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>User1@mail.Contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>InternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsUrl</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

Lors de l’application cliente a été demandée au point de terminaison correct pour le service de découverte automatique, le serveur envoie une réponse à l’élément [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) de l’élément de **réponse utilisateur** définie sur **NoError** et contenant les informations demandées paramètres utilisateur. Les paramètres utilisateur demandé uniquement, **InternalEwsUrl** et **ExternalEwsUrl**, sont renvoyés. L’exemple suivant montre la réponse du serveur. 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>160</h:MajorBuildNumber>
      <h:MinorBuildNumber>4</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>NoError</ErrorCode>
            <ErrorMessage>No error.</ErrorMessage>
            <RedirectTarget i:nil="true" />
            <UserSettingErrors />
            <UserSettings>
              <UserSetting i:type="StringSetting">
                <Name>InternalEwsUrl</Name>
                <Value>https://server.Contoso.com/ews/exchange.asmx</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ExternalEwsUrl</Name>
                <Value>https://server.Contoso.com/ews/exchange.asmx</Value>
              </UserSetting>
            </UserSettings>
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a>Étapes suivantes
<a name="bk_Next"> </a>

Recherche le point de terminaison en suivant le processus de découverte automatique renvoie le domaine demandé ou les paramètres utilisateur. Pour plus d’informations sur la création d’une demande pour des paramètres spécifiques, consultez les articles suivants :
  
- [Obtenir les paramètres de domaine à partir d’un serveur Exchange](how-to-get-domain-settings-from-an-exchange-server.md)
    
- [Obtenir les paramètres de l’utilisateur Exchange à l’aide de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a>Voir aussi


- [La configuration de vos applications EWS](setting-up-your-ews-application.md)
    
- [Découverte automatique pour Exchange](autodiscover-for-exchange.md)
    
- [Référence de service web de découverte automatique pour Exchange](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)
    
- [Référence EWS pour Exchange](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    

