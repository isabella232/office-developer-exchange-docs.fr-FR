---
title: Acheminer les demandes de hiérarchie de dossiers publics
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ec35df8e-4d75-4aa1-8b9c-ae1db7e05772
description: Toutes les demandes d’informations de dossier public nécessitant des connaissances de la hiérarchie de dossiers publics, telles que le transfert, la mise à jour, la suppression ou la recherche de dossiers publics, doivent être routées vers la boîte aux lettres de hiérarchie de dossiers publics par défaut pour l’utilisateur donné. Pour acheminer les demandes vers cette boîte aux lettres, vous devez définir les en-têtes X-AnchorMailbox et X-PublicFolderMailbox sur des valeurs spécifiques renvoyées par le service de découverte automatique.
ms.openlocfilehash: 2773aa3ab29868c69d1fb088deb6c8a96dfb9ecc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455705"
---
# <a name="route-public-folder-hierarchy-requests"></a>Acheminer les demandes de hiérarchie de dossiers publics

Toutes les demandes d’informations de dossier public nécessitant des connaissances de la hiérarchie de dossiers publics, telles que le transfert, la mise à jour, la suppression ou la recherche de dossiers publics, doivent être routées vers la boîte aux lettres de hiérarchie de dossiers publics par défaut pour l’utilisateur donné. Pour acheminer les demandes vers cette boîte aux lettres, vous devez définir les en-têtes **x-AnchorMailbox** et **x-PublicFolderMailbox** sur des valeurs spécifiques renvoyées par le service de découverte automatique. 
  
**Vue d’ensemble des dossiers publics**

|En-tête|De quoi ai-je besoin ?|Comment puis-je l’obtenir ?|
|:-----|:-----|:-----|
|**X-AnchorMailbox** <br/> |Valeur [PublicFolderInformation](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) d’une réponse SOAP de découverte automatique [GetUserSettings](https://msdn.microsoft.com/library/office/dd877096%28v=exchg.150%29.aspx) , qui devient la valeur de l’en-tête **X-AnchorMailbox** .<br/><br/> ![TODO](media/Ex15_PF_PFH_Anchor.png)| 1. envoyez une demande **GetUserSetting** avec l’adresse SMTP de la boîte aux lettres de l’utilisateur.<br/><br/>2. mettre en cache la valeur de l’élément **PublicFolderInformation** renvoyé par le service de découverte automatique. Cela peut être mis en cache à partir d’un appel de découverte automatique existant dans votre code ou d’un nouvel [appel GetUserSettings d’API managée EWS](#bk_getpfinfoewsma) ou d’une [requête SOAP GetUserSettings](#bk_getpfinfoews).  <br/><br/>3. Utilisez l’élément **PublicFolderInformation** pour renseigner la valeur de l’en-tête **X-AnchorMailbox** . La valeur de l’élément **PublicFolderInformation** est une adresse SMTP.  <br/> |
|**X-PublicFolderMailbox** <br/> |Valeur de [serveur](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) d’une [réponse de découverte automatique pox](https://msdn.microsoft.com/library/bb204082%28v=exchg.150%29.aspx)qui devient la valeur de l’en-tête **X-PublicFolderMailbox** .<br/><br/> ![TODO](media/Ex15_PF_PFH_PFMailbox.png)|1. [appelez le service de découverte automatique pox](#bk_makeautodrequest) à l’aide de l’adresse de messagerie **X-AnchorMailbox** .  <br/><br/>2. Utilisez l’élément **serveur** renvoyé par le service de découverte automatique pour renseigner la valeur de l’en-tête **X-PublicFolderMailbox** . La valeur de **X-PublicFolderMailbox** est une adresse SMTP où le nom d’utilisateur est un GUID.  <br/> |

<br/>

Une fois que vous avez déterminé les valeurs d’en-tête, incluez-les [lorsque vous effectuez des demandes de hiérarchie de dossiers publics](#bk_setheadervalues).
  
Les étapes décrites dans cet article sont spécifiques aux demandes de hiérarchie de dossiers publics. Pour déterminer si votre requête est une hiérarchie de dossiers publics ou une demande de contenu, consultez la rubrique [Routing Public Folder requests](public-folder-access-with-ews-in-exchange.md#bk_routing).
  
## <a name="determine-the-value-of-the-x-anchormailbox-header-by-using-the-ews-managed-api"></a>Déterminer la valeur de l’en-tête X-AnchorMailbox à l’aide de l’API managée EWS
<a name="bk_getpfinfoewsma"> </a>

Pour récupérer la valeur [PublicFolderInformation (POX)](https://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) à l’aide de l’API managée EWS, vous pouvez mettre en cache la valeur de l’élément **PublicFolderInformation** qu’un appel existant au service de découverte automatique renvoie ou effectuer un nouvel appel. 
  
Si vous effectuez un nouvel appel, vous pouvez [obtenir les paramètres utilisateur à l’aide de l’API managée EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)[obtenir les paramètres utilisateur à l’aide de l’API managée EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed) pour votre code, puis appeler l’exemple de méthode **GetUserSettings** à l’aide du code suivant, qui récupère uniquement la valeur de l’élément **PublicFolderInformation** . Incluez l’adresse SMTP de l’utilisateur de boîte aux lettres en tant que paramètre d’entrée. 
  
```cs
GetUserSettingsResponse userResponse = GetUserSettings(adservice, "sonyaf@contoso.com", 3, UserSettingName.PublicFolderInformation);
Console.WriteLine("X-AnchorMailbox value for public folder hierarchy requests: {0}", userResponse.Settings[UserSettingName.PublicFolderInformation]);
```

Après avoir exécuté le code, les informations suivantes s’affichent dans la console :
  
`X-AnchorMailbox for public folder hierarchy requests: SharedPublicFolder@contoso.com`

Maintenant que vous avez la valeur **PublicFolderInformation** , incluez-la comme valeur pour l’en-tête X-AnchorMailbox dans toutes les demandes de hiérarchie de dossiers publics. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="determine-the-value-of-the-x-anchormailbox-header-using-soap"></a>Déterminer la valeur de l’en-tête X-AnchorMailbox à l’aide de SOAP
<a name="bk_getpfinfoews"> </a>

L’exemple de code suivant montre comment récupérer la valeur **PublicFolderInformation** à l’aide de l’opération SOAP [GetUserSettings](https://msdn.microsoft.com/library/dd877096%28v=exchg.150%29.aspx) . L’utilisateur de boîte aux lettres est spécifié dans l’élément [Mailbox](https://msdn.microsoft.com/library/dd877076%28v=exchg.150%29.aspx) et l’élément [RequestedSettings](https://msdn.microsoft.com/library/office/dd877107%28v=exchg.150%29.aspx) limite la réponse à la valeur [PublicFolderInformation](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2007_SP1</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://pod51042.outlook.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>sonyaf@contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>PublicFolderInformation</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>
```

La réponse inclut la valeur **PublicFolderInformation** . 
  
```XML
<UserSetting i:type="StringSetting">
    <Name>PublicFolderInformation</Name>
    <Value>SharedPublicFolder@contoso.com</Value>
</UserSetting>
```

Maintenant que vous avez la valeur **PublicFolderInformation** , incluez-la comme valeur pour l’en-tête X-AnchorMailbox dans toutes les demandes de hiérarchie de dossiers publics. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="make-an-autodiscover-request-to-determine-the-x-publicfolderinformation-value"></a>Effectuer une demande de découverte automatique pour déterminer la valeur X-PublicFolderInformation
<a name="bk_makeautodrequest"> </a>

Effectuez une demande de découverte automatique à l’aide de l’adresse SMTP **PublicFolderInformation** , qui est maintenant utilisée en tant que valeur **X-AnchorMailbox** . Utilisez l’exemple de code [Exchange 2013 : Get User Settings with Autodiscover](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) pour appeler le service de découverte automatique, car il simplifie le processus de découverte automatique pour vous. Cet exemple de code utilise les arguments de ligne de commande présentés dans le tableau suivant pour appeler le service de découverte automatique POX sur l’adresse SMTP **PublicFolderInformation** . 
  
|**Argument de ligne de commande**|**Description**|
|:-----|:-----|
|emailAddress  <br/> |L’adresse SMTP **PublicFolderInformation** .  <br/> |
|-skipSOAP  <br/> | Utilisez les requêtes de découverte automatique POX pour ce scénario.  <br/> |
|-authEmailAddress auth  <br/> |L’adresse de messagerie de l’utilisateur de la boîte aux lettres, qui est utilisée pour l’authentification. Vous serez invité à entrer le mot de passe de l’utilisateur de boîte aux lettres lors de l’exécution de l’exemple.  <br/> |
   
Par exemple, quand SharedPublicFolder@contoso.com est l’adresse SMTP de l’élément **PublicFolderInformation** et sonyaf@contoso.com est l’utilisateur de boîte aux lettres, les arguments de ligne de commande doivent ressembler à ce qui suit. 
  
`SharedPublicFolder@contoso.com -skipSOAP -auth sonyaf@contoso.com`

Lorsque vous exécutez l’exemple de code **Exchange 2013 : Get User Settings with Autodiscover** , la dernière réponse de découverte automatique doit réussir et inclure tous les paramètres utilisateur associés au GUID de la boîte aux lettres. La valeur de [serveur](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) associée à l’élément de[type](https://msdn.microsoft.com/library/office/bb204223%28v=exchg.150%29.aspx) de [protocole](https://msdn.microsoft.com/library/bb204278%28v=exchg.150%29.aspx)Exch est la valeur d’en-tête **X-PublicFolderInformation** . 
  
```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    …
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <Protocol>
        <Type>EXCH</Type>
        <Server>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</Server>

```

Par ailleurs, si vous ne souhaitez pas utiliser l’exemple **Exchange 2013 : Get User Settings with Autodiscover** , vous pouvez obtenir la valeur du **serveur** en [générant une liste de points de terminaison de découverte automatique](how-to-generate-a-list-of-autodiscover-endpoints.md), puis en envoyant la demande de découverte automatique pox suivante à chaque URL jusqu’à ce que vous obteniez une réponse réussie. SharedPublicFolder@contoso.com est la valeur de l’en-tête **X-PublicFolderMailbox** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>SharedPublicFolder@contoso.com</EMailAddress>
    <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

Pour plus d’informations sur le processus de découverte automatique, voir [Autodiscover pour Exchange](autodiscover-for-exchange.md), [générer une liste des points de terminaison de découverte automatique](how-to-generate-a-list-of-autodiscover-endpoints.md)et [obtenir les paramètres utilisateur à partir d’Exchange à l’aide de la découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a>Définir les valeurs des en-têtes X-AnchorMailbox et X-PublicFolderMailbox
<a name="bk_setheadervalues"> </a>

En utilisant la valeur de l’adresse SMTP **PublicFolderInformation** acquise dans [determine la valeur de l’en-tête x-AnchorMailbox à l’aide de l’API managée EWS](#bk_getpfinfoewsma) ou en [déterminant la valeur de l’en-tête x-ANCHORMAILBOX à l’aide de SOAP](#bk_getpfinfoews) **, ainsi que** la valeur du **serveur** acquise dans la **demande de** [découverte automatique pour déterminer la valeur x-PublicFolderInformation](#bk_makeautodrequest) 
  
Par exemple, étant donné une adresse SMTP **PublicFolderInformation** de SharedPublicFolder@contoso.com et une valeur de **serveur** de 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com, incluez les en-têtes suivants lors de l’appel aux méthodes ou opérations suivantes. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com` <br/>
`X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com`

**Appels de dossier public nécessitant les en-têtes X-AnchorMailbox et X-PublicFolder**

|**Méthodes d'API managée EWS**|**Opérations EWS**|
|:-----|:-----|
|[Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [Folder. Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [MoveFolder](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
Pour ajouter ces en-têtes à l’aide de l’API managée EWS, utilisez la méthode [HttpHeaders. Add](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) . 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "SharedPublicFolder@contoso.com");service.HttpHeaders.Add("X-PublicFolderMailbox", "1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com");
```

Par exemple, le code suivant montre une requête [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) avec l’en-tête **x-AnchorMailbox** et **x-PublicFolderMailbox** défini sur les valeurs récupérées dans les exemples de cet article. 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
User-Agent: SoapSender1.0
X-AnchorMailbox: SharedPublicFolder@contoso.com
X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com
Host: outlook.office365.com
Content-Length: 1174
Expect: 100-continue
Connection: Keep-Alive
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:IsEqualTo>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:FieldURIOrConstant>
            <t:Constant Value="My Public Contacts" />
          </t:FieldURIOrConstant>
        </t:IsEqualTo>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:FolderId Id="AQEuAAADy/LIWjRCp0GFb0W6aGPbwwEARg5aCLUc8k6wLfl1c0a/2AAAAwIAAAA=" ChangeKey="AQAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/XB" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi

- [Accéder aux dossiers publics avec EWS dans Exchange](public-folder-access-with-ews-in-exchange.md)    
- [Acheminer les demandes de contenu de dossier public](how-to-route-public-folder-content-requests.md)    
- [Obtenir les paramètres utilisateur à l’aide de l’API managée EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)
    

