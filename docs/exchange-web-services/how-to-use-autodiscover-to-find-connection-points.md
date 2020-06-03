---
title: Utilisation de la découverte automatique pour trouver des points de connexion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 03896542-549b-4c45-973c-98f9025ea26c
description: Découvrez comment utiliser le service de découverte automatique pour diriger votre application cliente vers le serveur Exchange approprié.
localization_priority: Priority
ms.openlocfilehash: c1895fa0d2cce489467a726614e9457052624ef6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527592"
---
# <a name="use-autodiscover-to-find-connection-points"></a>Utilisation de la découverte automatique pour trouver des points de connexion

Découvrez comment utiliser le service de découverte automatique pour diriger votre application cliente vers le serveur Exchange approprié.
  
Le service de découverte automatique Exchange fournit à votre application cliente des paramètres de configuration pour les comptes de messagerie hébergés sur Exchange Online, Exchange Online dans le cadre d’Office 365 ou un serveur Exchange exécutant une version d’Exchange à partir d’Exchange 2013. Le service de découverte automatique est un service Web qui fournit des paramètres de configuration. Le service de découverte automatique est un service Web qui fournit des informations de configuration Exchange Server à votre application cliente. Les applications clientes utilisent la découverte automatique pour déterminer le point de terminaison du service de découverte automatique pour une boîte aux lettres spécifique. Cet article explique comment suivre les réponses d’un serveur Exchange pour trouver le point de terminaison correct. 
  
Pour plus d’informations sur la façon d’obtenir les paramètres de configuration des adresses de messagerie, consultez la rubrique [obtenir les paramètres utilisateur à partir d’Exchange à l’aide de la découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) et [obtenir les paramètres de domaine à partir d’un serveur Exchange](how-to-get-domain-settings-from-an-exchange-server.md).
  
> [!NOTE]
> Le processus de recherche du point de terminaison correct fait partie de la demande pour les paramètres de l’utilisateur ou du domaine. Le service de découverte automatique utilise une série de réponses de redirection pour envoyer l’application cliente au point de terminaison approprié pour une adresse de messagerie. 
  
Vous pouvez utiliser l’une des technologies de développement Exchange suivantes pour accéder au service de découverte automatique :

- API managée des services web Exchange (EWS)
    
- EWS
    
Si vous utilisez EWS, recourez aux méthodes suivantes pour extraire des paramètres utilisateur :
    
- Service de découverte automatique basé sur SOAP
    
- Service de découverte automatique XML (POX)
    
- Proxy généré automatiquement à partir du service de détection automatique SOAP ou XML
    
Pour plus d'informations sur ces méthodes, reportez-vous à la section [Découverte automatique pour Exchange](autodiscover-for-exchange.md).

Pour plus d’informations sur ces technologies de développement Exchange, voir [Explorer l’API managée EWS, EWS et les services Web dans Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md). 

L’API managée EWS fournit une interface basée sur des objets pour récupérer les paramètres de l’utilisateur. Si votre application cliente utilise du code managé, nous vous recommandons de choisir l’API managée EWS. L’interface API managée EWS optimisée pour un modèle d’objet simple présente des performances supérieures au proxy de service web généré automatiquement par défaut. 
  
Si vous utilisez EWS, nous vous conseillons d’opter pour le service de découverte automatique SOAP, car il prend en charge un ensemble de fonctionnalités plus riche que le service de découverte automatique POX.
  
## <a name="prerequisites-for-finding-an-endpoint"></a>Conditions préalables à la recherche d’un point de terminaison
<a name="bk_Prereq"> </a>

Pour pouvoir créer une application cliente qui utilise le service de découverte automatique, vous devez avoir accès à ce qui suit :
  
- Exchange Online ou un serveur qui exécute une version d’Exchange à partir d’Exchange 2007 SP1. Si vous utilisez le service de découverte automatique basé sur SOAP, Exchange Online ou une version d’Exchange commençant par Exchange 2010.
    
- Un serveur Exchange qui est configuré pour accepter les connexions depuis votre application cliente. Pour plus d'informations sur la configuration de votre serveur Exchange, reportez-vous à la rubrique [Contrôle de l'accès aux applications de client pour EWS dans Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
- Un compte autorisé à utiliser EWS. Pour plus d'informations sur la configuration d'un compte, reportez-vous à la rubrique [Contrôle de l'accès aux applications de client pour EWS dans Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
> [!NOTE]
> Si vous utilisez l’API managée EWS, vous devez fournir un rappel de validation de certificat dans certains cas. Vous aurez peut-être également besoin d’un rappel de validation de certificat avec certaines bibliothèques proxy générées, telles que celles créées par Visual Studio. Pour plus d'informations, reportez-vous à la rubrique [Valider un certificat de serveur pour l'API managée EWS](how-to-validate-a-server-certificate-for-the-ews-managed-api.md). 
  
### <a name="core-concepts-for-finding-an-endpoint"></a>Concepts de base pour trouver un point de terminaison
<a name="bk_Core"> </a>

Avant d’utiliser la découverte automatique pour trouver un point de terminaison, vous devez être familiarisé avec les concepts présentés dans le tableau suivant.
  
|**Concept**|**Description**|
|:-----|:-----|
|[Découverte automatique pour Exchange](autodiscover-for-exchange.md) <br/> |Fournit une vue d’ensemble du fonctionnement du service de découverte automatique.  <br/> |
   
Si vous utilisez l'API managée EWS, vous gérez votre connexion à EWS à l'aide de la classe [Microsoft.Exchange.WebServices.Data.ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) dans l'espace de noms [Microsoft.Exchange.WebServices.Data](https://msdn.microsoft.com/library/dd633907%28v=exchg.80%29.aspx). Pour utiliser les exemples de code de l’API managée EWS dans cet article, vous devez référencer les espaces de noms suivants dans votre code : 
  
- **System.Net**
    
- **Microsoft.Exchange.WebServices.Data.ExchangeService**
    
## <a name="find-the-correct-endpoint-by-using-the-ews-managed-api"></a>Trouver le point de terminaison correct à l’aide de l’API managée EWS
<a name="bk_Managed"> </a>

Si vous utilisez l’API managée EWS, les appels au service de découverte automatique sont gérés par la classe **ExchangeService** . Pour déterminer le point de terminaison approprié pour un compte de messagerie, vous appelez la méthode **AutodiscoverUrl** sur un objet **[ExchangeService]** . L’exemple de code suivant montre comment définir le point de terminaison du service Web EWS pour une adresse de messagerie dans le fichier Exchange. asmx sur le serveur d’accès au client approprié à l’aide de l’API managée EWS. 
  
```cs
NetworkCredential credentials = new NetworkCredential(securelyStoredEmail, securelyStoredPassword);
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2013);
service.Credentials = credentials;
service.AutodiscoverUrl("User1@contoso.com");
```

## <a name="find-the-correct-endpoint-by-using-ews"></a>Trouver le point de terminaison correct à l’aide d’EWS
<a name="bk_SOAP"> </a>

Le service de découverte automatique SOAP peut utiliser une série de demandes et de réponses pour diriger votre application vers le point de terminaison correct pour EWS. Pour plus d’informations sur le processus permettant de déterminer le point de terminaison correct pour un compte de messagerie, consultez la rubrique [découverte automatique pour Exchange](autodiscover-for-exchange.md). Les exemples XML suivants montrent la série de demandes et de réponses que vous pouvez vous attendre lors de la création d’une demande de découverte automatique SOAP pour trouver le point de terminaison approprié.
  
### <a name="soap-autodiscover-endpoint-request"></a>Demande de point de terminaison de découverte automatique SOAP

L’exemple suivant montre une requête XML qui est envoyée au service de découverte automatique pour trouver le point de terminaison correct.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://mail.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

### <a name="soap-autodiscover-redirection-response"></a>Réponse de redirection de la découverte automatique SOAP

Le service de découverte automatique peut répondre avec une des deux réponses de redirection : une redirection HTTP 302 ou une réponse de redirection SOAP. Si la réponse du serveur Exchange est une redirection HTTP 302, l’application cliente doit vérifier que l’adresse de redirection est acceptable, puis suivre la réponse de redirection.
  
> [!IMPORTANT]
> Pour obtenir les critères de validation d’une réponse de redirection, consultez la rubrique [découverte automatique pour Exchange](autodiscover-for-exchange.md). 
  
Si le service de découverte automatique renvoie une réponse de redirection, indiquée par l’élément [ErrorCode](https://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) de l’élément **UserResponse** , votre application cliente doit utiliser l’élément **RedirectTarget** pour créer une nouvelle demande de paramètres qui est envoyée au serveur spécifié dans la réponse de redirection. L’exemple suivant montre une réponse de redirection du serveur. 
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>682</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

Après une redirection, le client utilise l’URL de redirection pour préparer une autre demande. Le code suivant illustre un exemple de la requête que vous créez à partir de la réponse de redirection.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

Lorsque l’application cliente a été dirigée vers le point de terminaison approprié pour le service de découverte automatique, le serveur envoie une réponse avec l’élément [ErrorCode](https://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) de l’élément **UserResponse** défini sur **NOERROR** et contenant les paramètres utilisateur demandés. Seuls les paramètres utilisateur demandés, **InternalEwsUrl** et **ExternalEwsUrl**, sont renvoyés. L’exemple suivant montre la réponse du serveur. 
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
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
    <GetUserSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

La recherche du point de terminaison en suivant le processus de découverte automatique renvoie les paramètres de domaine ou d’utilisateur demandés. Pour plus d’informations sur la demande de paramètres spécifiques, consultez les articles suivants :
  
- [Obtenir des paramètres de domaine à partir d’un serveur Exchange](how-to-get-domain-settings-from-an-exchange-server.md)    
- [Obtenir les paramètres de l'utilisateur Exchange à l'aide de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a>Voir aussi

- [Configuration de votre application EWS](setting-up-your-ews-application.md)   
- [Découverte automatique pour Exchange](autodiscover-for-exchange.md)    
- [Référence de service web de découverte automatique pour Exchange](https://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)    
- [Référence EWS pour Exchange](https://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    

