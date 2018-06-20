---
title: Acheminer les requêtes de hiérarchie de dossiers publics
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ec35df8e-4d75-4aa1-8b9c-ae1db7e05772
description: Toutes les demandes pour les informations de dossier public qui requièrent la connaissance de la hiérarchie de dossiers publics, telles que le déplacement, mise à jour, suppression ou de trouver des dossiers publics, doivent être acheminés vers la boîte aux lettres de hiérarchie des dossiers publics par défaut pour l’utilisateur donné. Pour router les demandes pour cette boîte aux lettres, vous devez définir les en-têtes X-AnchorMailbox et X-PublicFolderMailbox à des valeurs spécifiques renvoyées par le service de découverte automatique.
ms.openlocfilehash: 983431864729edbb040a7206dae416d10bfb2b7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754942"
---
# <a name="route-public-folder-hierarchy-requests"></a>Acheminer les requêtes de hiérarchie de dossiers publics

Toutes les demandes pour les informations de dossier public qui requièrent la connaissance de la hiérarchie de dossiers publics, telles que le déplacement, mise à jour, suppression ou de trouver des dossiers publics, doivent être acheminés vers la boîte aux lettres de hiérarchie des dossiers publics par défaut pour l’utilisateur donné. Pour router les demandes pour cette boîte aux lettres, vous devez définir les en-têtes **X-AnchorMailbox** et **X-PublicFolderMailbox** à des valeurs spécifiques renvoyées par le service de découverte automatique. 
  
**Vue d’ensemble des dossiers publics**

|En-tête|Que dois-je ?|Comment l’obtenir ?|
|:-----|:-----|:-----|
|**X-AnchorMailbox** <br/> |La valeur [PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx) à partir d’une réponse SOAP de découverte automatique [GetUserSettings](http://msdn.microsoft.com/en-us/library/office/dd877096%28v=exchg.150%29.aspx) , qui devient la valeur de l’en-tête **X-AnchorMailbox** .<br/><br/> ![TÂCHES](media/Ex15_PF_PFH_Anchor.png)| 1. envoyer une demande de **GetUserSetting** avec l’adresse SMTP de la boîte aux lettres de l’utilisateur.<br/><br/>2. mettre en cache la valeur de l’élément **PublicFolderInformation** qui renvoie le service de découverte automatique. Cela peut être mis en cache à partir d’un appel de la découverte automatique existant dans votre code, ou un nouvel [appel GetUserSettings des API gérée EWS](#bk_getpfinfoewsma) ou une [demande SOAP GetUserSettings](#bk_getpfinfoews).  <br/><br/>3. Utilisez l’élément **PublicFolderInformation** pour remplir la valeur de l’en-tête **X-AnchorMailbox** . La valeur de l’élément **PublicFolderInformation** est une adresse SMTP.  <br/> |
|**X-PublicFolderMailbox** <br/> |La valeur de [serveur](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx) à partir d’une [réponse de découverte automatique variole](http://msdn.microsoft.com/en-us/library/bb204082%28v=exchg.150%29.aspx), qui devient la valeur de l’en-tête **X-PublicFolderMailbox** .<br/><br/> ![TÂCHES](media/Ex15_PF_PFH_PFMailbox.png)|1. le service [d’appel de la découverte automatique variole](#bk_makeautodrequest) à l’aide de l’adresse de messagerie **X-AnchorMailbox** .  <br/><br/>2. Utilisez l’élément de **serveur** renvoyé par le service de découverte automatique pour remplir la valeur de l’en-tête **X-PublicFolderMailbox** . La valeur de la **X-PublicFolderMailbox** est une adresse SMTP où le nom d’utilisateur est un GUID.  <br/> |

<br/>

Une fois que vous avez déterminé les valeurs d’en-tête, ajoutez-les [lorsque vous effectuez des demandes de hiérarchie de dossiers publics](#bk_setheadervalues).
  
Les étapes décrites dans cet article sont spécifiques aux demandes de hiérarchie de dossiers publics. Pour déterminer si votre demande est une hiérarchie de dossiers publics ou d’une requête de contenu, voir les [demandes de dossiers publics de routage](public-folder-access-with-ews-in-exchange.md#bk_routing).
  
## <a name="determine-the-value-of-the-x-anchormailbox-header-by-using-the-ews-managed-api"></a>Déterminer la valeur de l’en-tête X-AnchorMailbox à l’aide de l’API managée EWS
<a name="bk_getpfinfoewsma"> </a>

Pour récupérer la valeur [PublicFolderInformation (POX)](http://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) à l’aide de l’API managée EWS, vous pouvez mettre en cache la valeur de l’élément **PublicFolderInformation** qui renvoie un appel existant pour le service de découverte automatique ou effectuer un nouvel appel. 
  
Si vous créez un nouvel appel, vous pouvez [obtenir les paramètres utilisateur à l’aide de l’API managée EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)[obtenir les paramètres utilisateur à l’aide de l’API managée EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed) votre code et puis appelez le **GetUserSettings** exemple de méthode en utilisant le code suivant, extrait seule la valeur de l’élément **PublicFolderInformation** . Inclure l’adresse SMTP de l’utilisateur de boîte aux lettres comme paramètre d’entrée. 
  
```cs
GetUserSettingsResponse userResponse = GetUserSettings(adservice, "sonyaf@contoso.com", 3, UserSettingName.PublicFolderInformation);
Console.WriteLine("X-AnchorMailbox value for public folder hierarchy requests: {0}", userResponse.Settings[UserSettingName.PublicFolderInformation]);
```

Après avoir exécuté le code, les informations suivantes s’affiche sur la console :
  
`X-AnchorMailbox for public folder hierarchy requests: SharedPublicFolder@contoso.com`

Maintenant que vous disposez de la valeur **PublicFolderInformation** , inclure en tant que la valeur de l’en-tête X-AnchorMailbox dans toutes les demandes de hiérarchie de dossiers publics. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="determine-the-value-of-the-x-anchormailbox-header-using-soap"></a>Déterminer la valeur de l’en-tête X-AnchorMailbox utilisant SOAP
<a name="bk_getpfinfoews"> </a>

L’exemple de code suivant montre comment récupérer la valeur **PublicFolderInformation** à l’aide de l’opération SOAP [GetUserSettings](http://msdn.microsoft.com/en-us/library/dd877096%28v=exchg.150%29.aspx) . L’utilisateur de boîte aux lettres est spécifié dans l’élément de [boîte aux lettres](http://msdn.microsoft.com/en-us/library/dd877076%28v=exchg.150%29.aspx) , et l’élément [RequestedSettings](http://msdn.microsoft.com/en-us/library/office/dd877107%28v=exchg.150%29.aspx) limite la réponse à la valeur [PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2007_SP1</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://pod51042.outlook.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
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

Maintenant que vous disposez de la valeur **PublicFolderInformation** , inclure en tant que la valeur de l’en-tête X-AnchorMailbox dans toutes les demandes de hiérarchie de dossiers publics. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="make-an-autodiscover-request-to-determine-the-x-publicfolderinformation-value"></a>Effectuer une requête de découverte automatique pour déterminer la valeur X-PublicFolderInformation
<a name="bk_makeautodrequest"> </a>

Effectuer une requête de découverte automatique à l’aide de l’adresse SMTP **PublicFolderInformation** , qui est désormais utilisée comme valeur **X-AnchorMailbox** . Utiliser le [Exchange 2013 : obtenir les paramètres utilisateur avec Autodiscover](http://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) exemple de code pour appeler le service de découverte automatique, car elle rationalise le processus de découverte automatique pour vous. Cet exemple de code utilise les arguments de ligne de commande répertoriées dans le tableau suivant pour appeler le service de découverte automatique variole sur l’adresse SMTP **PublicFolderInformation** . 
  
|**Argument de ligne de commande**|**Description**|
|:-----|:-----|
|emailAddress  <br/> |L’adresse **PublicFolderInformation** SMTP.  <br/> |
|-skipSOAP  <br/> | Utilisez les demandes de découverte automatique variole pour ce scénario.  <br/> |
|authEmailAddress - auth  <br/> |Adresse de messagerie de l’utilisateur de boîte aux lettres, qui est utilisé pour l’authentification. Vous serez invité à entrer le mot de passe de l’utilisateur de boîte aux lettres lorsque vous exécutez l’exemple.  <br/> |
   
Par exemple, lorsque SharedPublicFolder@contoso.com est l’adresse SMTP de l’élément **PublicFolderInformation** et sonyaf@contoso.com est l’utilisateur de boîte aux lettres, les arguments de ligne de commande doivent se présenter comme suit. 
  
`SharedPublicFolder@contoso.com -skipSOAP -auth sonyaf@contoso.com`

Lorsque vous exécutez le **Exchange 2013 : obtenir les paramètres utilisateur avec Autodiscover** exemple, la dernière réponse de découverte automatique doit être réussie et inclure tous les paramètres d’utilisateur associés à la boîte aux lettres GUID. La valeur du [serveur](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx) associée à l’élément de [protocole](http://msdn.microsoft.com/en-us/library/bb204278%28v=exchg.150%29.aspx)EXCH[Type](http://msdn.microsoft.com/en-us/library/office/bb204223%28v=exchg.150%29.aspx) est la valeur de l’en-tête **X-PublicFolderInformation** . 
  
```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    …
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <Protocol>
        <Type>EXCH</Type>
        <Server>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</Server>

```

Sinon, si vous ne souhaitez pas utiliser le **Exchange 2013 : obtenir les paramètres utilisateur avec Autodiscover** exemple, vous pouvez obtenir la valeur du **serveur** en [générant une liste des points de terminaison de découverte automatique](how-to-generate-a-list-of-autodiscover-endpoints.md), puis l’envoi de la découverte automatique de variole suivantes demander à chaque URL jusqu'à ce que vous recevez une réponse positive. SharedPublicFolder@contoso.com est la valeur de l’en-tête **X-PublicFolderMailbox** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>SharedPublicFolder@contoso.com</EMailAddress>
    <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

Pour plus d’informations sur le processus de découverte automatique, consultez la rubrique [Autodiscover pour Exchange](autodiscover-for-exchange.md), [Générer une liste des points de terminaison de découverte automatique](how-to-generate-a-list-of-autodiscover-endpoints.md)et [obtenir les paramètres utilisateur à partir d’Exchange à l’aide de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a>Définissez les valeurs des en-têtes X-AnchorMailbox et X-PublicFolderMailbox
<a name="bk_setheadervalues"> </a>

À l’aide de la valeur de l’adresse **PublicFolderInformation** SMTP pour [déterminer la valeur de l’en-tête X-AnchorMailbox à l’aide de l’API managée EWS](#bk_getpfinfoewsma) ou [déterminer la valeur de l’en-tête X-AnchorMailbox en utilisant SOAP](#bk_getpfinfoews) et le serveur ** **de valeur acquise dans [créer une demande de découverte automatique pour déterminer la valeur X-PublicFolderInformation](#bk_makeautodrequest), définissez les valeurs d’en-tête **X-AnchorMailbox** et **X-PublicFolderMailbox** dans votre requête de contenu de dossier public. 
  
Par exemple, si une adresse **PublicFolderInformation** SMTP SharedPublicFolder@contoso.com et la valeur **Server** 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com, inclure les en-têtes suivants lors d’appels à ce qui suit méthodes ou opérations. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com` <br/>
`X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com`

**Appels de dossier public qui nécessitent les en-têtes X-AnchorMailbox et X-PublicFolder**

|**Méthodes d'API managée EWS**|**Opérations EWS**|
|:-----|:-----|
|[Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [Folder.Move](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [MoveFolder](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
Pour ajouter ces en-têtes à l’aide de l’API managée EWS, utilisez la méthode [HttpHeaders.Add](http://msdn.microsoft.com/en-us/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) . 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "SharedPublicFolder@contoso.com");service.HttpHeaders.Add("X-PublicFolderMailbox", "1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com");
```

Par exemple, le code suivant montre une demande [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) avec l’en-tête **X-AnchorMailbox** et **X-PublicFolderMailbox** les valeurs récupérées dans les exemples de cet article. 
  
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
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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
- [Router les demandes de contenu de dossier public](how-to-route-public-folder-content-requests.md)    
- [Obtenir les paramètres de l’utilisateur à l’aide de l’API managée EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)
    

