---
title: Définir des autorisations de dossier pour un autre utilisateur à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 7eb81676-a780-4c56-b4f2-c4ed2697107d
description: Découvrez comment définir des niveaux d’autorisation sur un dossier à l’aide de l’API gérée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: 15288af0448a48c176529912604f628ae9bc2f19
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513086"
---
# <a name="set-folder-permissions-for-another-user-by-using-ews-in-exchange"></a>Définir des autorisations de dossier pour un autre utilisateur à l’aide d’EWS dans Exchange

Découvrez comment définir des niveaux d’autorisation sur un dossier à l’aide de l’API gérée EWS ou d’EWS dans Exchange.
  
Les autorisations au niveau du dossier permettent aux utilisateurs d’accéder à un ou plusieurs dossiers dans la boîte aux lettres d’un autre utilisateur. Les autorisations de dossier sont similaires à l’accès délégué, mais elles diffèrent des manières suivantes : 
  
- Les autorisations de dossier ne permettent pas à un utilisateur d'« envoyer de la part de » ou d'« envoyer en tant que » un autre utilisateur. Ils permettent uniquement l’accès aux dossiers. Les utilisateurs peuvent créer des éléments dans ces dossiers, mais ils ne peuvent pas les envoyer.
    
- Vous pouvez définir des autorisations de dossier sur n’importe quel dossier de la boîte aux lettres, mais vous pouvez uniquement ajouter un délégué aux dossiers Calendrier, Contacts, Boîte de réception, Journal, Notes et Tâches.
    
- Vous pouvez définir un certain nombre [d’autorisations sur un dossier spécifique.](#bk_folderperms) Lorsque vous ajoutez un délégué, vous pouvez attribuer l’un des cinq [niveaux d’autorisation uniquement.](delegate-access-and-ews-in-exchange.md#bk_delegateperms)
    
- Vous pouvez définir des autorisations de dossier pour les utilisateurs anonymes et par défaut. Vous pouvez uniquement accorder un accès délégué à un compte à messagerie.
    
Si vous connaissez les entrées de contrôle d’accès et les listes de contrôle d’accès discrétionnaire, vous savez qu’un utilisateur ne peut avoir qu’un seul ensemble d’autorisations pour chaque dossier. Si vous essayez d’ajouter un ensemble d’autorisations pour un utilisateur et qu’il a déjà un ensemble d’autorisations, vous obtenez une erreur. Lorsque vous ajoutez, supprimez ou mettez à jour des autorisations sur un dossier, vous obtenez le DACL actuel, ajoutez ou supprimez des ace, puis envoyez le DACL mis à jour. Vous ne pouvez pas ajouter plusieurs ace pour le même utilisateur. Lorsque vous mettez à jour les autorisations à l’aide de l’API gérée EWS, vous devez supprimer l’ACE actuel de l’utilisateur, puis ajouter son nouvel ACE à la collection. Si vous utilisez EWS, vous remplacez simplement l’ensemble d’aces précédent par les nouvelles.
  
Si vous a apporté plusieurs modifications d’autorisation à un dossier unique, vous pouvez effectuer des ajouts par lots, des suppressions ou des mises à jour. Notez simplement que vous ne pouvez pas effectuer de mises à jour utilisateur par lot sur plusieurs dossiers. Un appel est nécessaire pour obtenir les autorisations sur un dossier unique, et un deuxième appel est nécessaire pour mettre à jour les autorisations sur ce dossier. Lorsque vous ajoutez, supprimez ou mettez à jour des autorisations utilisateur, vous utilisez les mêmes deux opérations ou appels de méthode pour chaque tâche.
  
**Tableau 1. Méthodes d’API gérées EWS et opérations EWS pour la définition des autorisations de dossier**

|Si vous souhaitez...|Utilisez cette méthode d’API gérée EWS...|Utilisez cette opération EWS...|
|:-----|:-----|:-----|
|Activer, supprimer ou mettre à jour les autorisations de dossier  <br/> |[Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) suivi de [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) <br/> |[GetFolder suivi](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) de [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|Créer un dossier et définir des autorisations de dossier  <br/> |[Folder.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
   
## <a name="folder-permissions"></a>Autorisations d’accès aux dossiers
<a name="bk_folderperms"> </a>

Vous avez plusieurs options pour définir des autorisations de dossier sur un dossier spécifique. Vous pouvez définir un niveau d’autorisation sur un dossier pour chaque utilisateur, ce qui ajoute un ensemble d’autorisations individuelles prédéfinës au DACL, ou vous pouvez définir des autorisations individuelles sur un dossier, mais vous ne pouvez pas combiner et faire correspondre.
  
Les autorisations individuelles suivantes sont disponibles :
  
- Peut créer
- Peut créer des sous-foldeurs    
- Est propriétaire du dossier    
- Le dossier est-il visible ?    
- Est-ce qu’un contact de dossier    
- Modifier des éléments    
- Supprimer des éléments    
- Lire des éléments
    
En outre, les niveaux d’autorisation suivants sont disponibles, qui définissent un sous-ensemble d’autorisations et de valeurs individuelles, comme indiqué dans le tableau 2 :
  
- Aucun    
- Propriétaire    
- PublishingEditor    
- Éditeur    
- PublishingAuthor    
- Auteur    
- NoneditingAuthor    
- Relecteur    
- Collaborateur   
- Personnalisé : cette valeur ne peut pas être définie par l’application. Le serveur définit cette valeur si l’application inclut une collection personnalisée d’autorisations individuelles.    
- FreeBusyTimeOnly : cette fonction ne peut être définie que sur les dossiers de calendrier.   
- FreeBusyTimeAndSubjectAndLocation : cette fonction ne peut être définie que sur les dossiers de calendrier.
    
Le tableau suivant indique les autorisations individuelles qui sont appliquées par défaut en fonction du niveau d’autorisation.
  
**Tableau 2. Autorisations individuelles par niveau d’autorisation**

|Niveau d’autorisation|Peut créer des éléments|Peut créer des sous-dossiers|Est propriétaire du dossier|Le dossier est-il visible ?|Est-ce qu’un contact de dossier|Modifier des éléments|Supprimer des éléments|Peut lire des éléments|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Aucun  <br/> |Faux  <br/> |Faux  <br/> |Faux  <br/> |Faux  <br/> |Faux  <br/> |Aucun  <br/> |Aucun  <br/> |Aucun  <br/> |
|Propriétaire  <br/> |True  <br/> |True  <br/> |True  <br/> |True  <br/> |True  <br/> |Tous  <br/> |Tous  <br/> |FullDetails  <br/> |
|PublishingEditor  <br/> |True  <br/> |True  <br/> |False  <br/> |True  <br/> |Faux  <br/> |Tous  <br/> |Tous  <br/> |FullDetails  <br/> |
|Éditeur  <br/> |Vrai  <br/> |Faux  <br/> |False  <br/> |True  <br/> |Faux  <br/> |Tous  <br/> |Tous  <br/> |FullDetails  <br/> |
|PublishingAuthor  <br/> |True  <br/> |True  <br/> |False  <br/> |True  <br/> |Faux  <br/> |Owned  <br/> |Owned  <br/> |FullDetails  <br/> |
|Auteur  <br/> |Vrai  <br/> |Faux  <br/> |False  <br/> |True  <br/> |Faux  <br/> |Owned  <br/> |Owned  <br/> |FullDetails  <br/> |
|NoneditingAuthor  <br/> |Vrai  <br/> |Faux  <br/> |False  <br/> |True  <br/> |Faux  <br/> |Aucun  <br/> |Owned  <br/> |FullDetails  <br/> |
|Relecteur  <br/> |Faux  <br/> |Faux  <br/> |False  <br/> |True  <br/> |Faux  <br/> |Aucun  <br/> |Aucun  <br/> |FullDetails  <br/> |
|Collaborateur  <br/> |Vrai  <br/> |Faux  <br/> |False  <br/> |True  <br/> |Faux  <br/> |Aucun  <br/> |Aucun  <br/> |Aucun  <br/> |
   
Si vous spécifiez un niveau d’autorisation non personnalisé dans la demande d’autorisations au niveau du dossier, vous n’avez pas besoin de spécifier les paramètres d’autorisation individuels. Si vous spécifiez une autorisation individuelle lorsque vous définissez un niveau d’autorisation, une erreur **ErrorInvalidPermissionSettings** est renvoyée dans la réponse. 
  
## <a name="adding-folder-permissions-by-using-the-ews-managed-api"></a>Ajout d’autorisations de dossier à l’aide de l’API gérée EWS
<a name="bk_enableewsma"> </a>

L’exemple de code suivant montre comment utiliser l’API gérée EWS pour : 
  
- Créez un [objet FolderPermission](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) pour le nouvel utilisateur. 
    
- Obtenez les autorisations actuelles pour un dossier à l’aide de [la méthode Bind.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) 
    
- Ajoutez les **nouveaux FolderPermissions à** la [propriété Folder.Permissions.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) 
    
- Appelez la [méthode Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) pour enregistrer les nouvelles autorisations sur le serveur. 
    
Cet exemple suppose que **le service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le propriétaire de la boîte aux lettres et que l’utilisateur a été authentifié sur Exchange serveur. 
  
```cs
static void EnableFolderPermissions(ExchangeService service)
{
    // Create a property set to use for folder binding.
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.Permissions);
    // Specify the SMTP address of the new user and the folder permissions level.
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
    
    // Bind to the folder and get the current permissions. 
    // This call results in a GetFolder call to EWS.
    Folder sentItemsFolder = Folder.Bind(service, WellKnownFolderName.SentItems, propSet);
 
    // Add the permissions for the new user to the Sent Items DACL.
    sentItemsFolder.Permissions.Add(fldperm);
    // This call results in a UpdateFolder call to EWS.
    sentItemsFolder.Update();
}
```

La ligne de code suivante spécifie le niveau d’autorisation.
  
```cs
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
```

Si vous souhaitez utiliser le niveau d’autorisation personnalisé, utilisez ce code à la place.
  
```cs
FolderPermission fldperm = new FolderPermission();
fldperm.UserId = "sadie@Contoso1000.onmicrosoft.com";
fldperm.CanCreateItems = true;
fldperm.CanCreateSubFolders = true;
…
```

Vous pouvez définir une ou toutes les propriétés [FolderPermission](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) accessibles en ligne lorsque vous créez un objet **FolderPermission** avec un niveau d’autorisation personnalisé. Notez toutefois que [FolderPermissionLevel](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) n’est jamais explicitement définie sur **Custom** par l’application. **FolderPermissionLevel** est définie sur Custom uniquement lorsque vous créez un **objet FolderPermission** et définissez des autorisations individuelles. 
  
## <a name="adding-folder-permissions-by-using-ews"></a>Ajout d’autorisations de dossier à l’aide d’EWS
<a name="bk_enableews"> </a>

Les exemples de code EWS suivants montrent comment ajouter des autorisations à un dossier spécifique en récupérant les autorisations actuelles, puis en envoyant une liste de nouvelles autorisations.
  
La première étape consiste à envoyer une demande [GetFolder,](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) où la valeur [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) spécifie le dossier dans lequel ajouter des autorisations (le dossier Éléments envoyés dans cet exemple) et la valeur [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) inclut folder:PermissionSet. Cette demande récupère les paramètres d’autorisation pour le dossier spécifié. 
  
Il s’agit également de la demande XML que l’API gérée EWS envoie lorsque vous appelez la méthode **Bind** pour ajouter des [autorisations de dossier.](#bk_enableewsma)
  
```XML
  <?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                 xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:GetFolder>
        <m:FolderShape>
          <t:BaseShape>IdOnly</t:BaseShape>
          <t:AdditionalProperties>
            <t:FieldURI FieldURI="folder:PermissionSet" />
          </t:AdditionalProperties>
        </m:FolderShape>
        <m:FolderIds>
          <t:DistinguishedFolderId Id="sentitems" />
        </m:FolderIds>
      </m:GetFolder>
    </soap:Body>
  </soap:Envelope>
```

Le serveur répond à la demande **GetFolder** avec un message [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, qui indique que le dossier a été récupéré avec succès. Les [valeurs FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) et [ParentFolderId](https://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) ont été raccourcies pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="CgAAAA=="
                          ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd1" />
              <t:PermissionSet>
                <t:Permissions>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Default</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                </t:Permissions>
              </t:PermissionSet>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

Ensuite, utilisez **l’opération UpdateFolder** pour envoyer le [PermissionSet](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx)mis à jour, qui inclut l’autorisation pour le nouvel utilisateur. [](https://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) Notez que le fait d’inclure [l’élément SetFolderField](https://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) pour le dossier respectif dans l’opération [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) a pour effet de faire en sorte que tous les paramètres d’autorisation sur le dossier. De même, l’option [DeleteFolderField](https://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) de l’opération **UpdateFolder** supprime également tous les paramètres d’autorisation sur le dossier. 
  
Il s’agit également de la demande XML que l’API gérée EWS envoie lorsque vous appelez la méthode **Update** pour ajouter des [autorisations de dossier.](#bk_enableewsma)
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="CgAAAA=="
                      ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd1" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:PermissionSet" />
              <t:Folder>
                <t:PermissionSet>
                  <t:Permissions>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Default</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
                      </t:UserId>
                      <t:PermissionLevel>Editor</t:PermissionLevel>
                    </t:Permission>
                  </t:Permissions>
                </t:PermissionSet>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

La ligne de code suivante spécifie le niveau d’autorisation.
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
    </t:UserId>
    <t:PermissionLevel>Editor</t:PermissionLevel>
</t:Permission>
```

Si vous souhaitez utiliser le niveau d’autorisation personnalisé, utilisez ce code à la place.
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress> sadie@contoso.com </t:PrimarySmtpAddress>
    </t:UserId>
    <t:CanCreateItems>true</t:CanCreateItems>
    <t:CanCreateSubFolders>true</t:CanCreateSubFolders>
    <t:IsFolderOwner>false</t:IsFolderOwner>
    <t:IsFolderVisible>false</t:IsFolderVisible>
    <t:IsFolderContact>false</t:IsFolderContact>
    <t:EditItems>None</t:EditItems>
    <t:DeleteItems>None</t:DeleteItems>
    <t:ReadItems>None</t:ReadItems>
    <t:PermissionLevel>Custom</t:PermissionLevel>
</t:Permission>
```

Le serveur répond à la demande **UpdateFolder** avec un message [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError,** qui indique que le dossier a été mis à jour avec succès.
  
## <a name="removing-folder-permissions-by-using-the-ews-managed-api"></a>Suppression des autorisations de dossier à l’aide de l’API gérée EWS
<a name="bk_removeewsma"> </a>

L’exemple de code suivant montre comment utiliser l’API gérée EWS pour supprimer toutes les autorisations utilisateur sur un dossier spécifique, à l’exception des autorisations par défaut et anonymes, par :
  
1. Obtention des autorisations actuelles pour un dossier à l’aide de la **méthode Bind.** 
    
2. Iterating through the **Permissions** collection and removing permissions for individual users. 
    
3. Appel de la **méthode Update** pour enregistrer les modifications. 
    
Cet exemple supprime toutes les autorisations utilisateur sur un dossier. Si vous souhaitez modifier cet exemple pour supprimer des autorisations uniquement pour un utilisateur spécifique, modifiez la ligne de code suivante pour identifier le nom d’affichage ou l’adresse SMTP de l’utilisateur.
  
```cs
if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
```

Cet exemple suppose que **le service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le propriétaire de la boîte aux lettres et que l’utilisateur a été authentifié sur Exchange serveur. 
  
```cs
static void RemoveFolderPermissions(ExchangeService service)
{
    // Create a property set to use for folder binding.
    PropertySet propSet = new PropertySet(BasePropertySet.FirstClassProperties, FolderSchema.Permissions);
    // Bind to the folder and get the current permissions. 
    // This call results in a GetFolder call to EWS.
    Folder sentItemsFolder = Folder.Bind(service, new FolderId(WellKnownFolderName.SentItems, "primary@contoso.com"), propSet);
    // Iterate through the collection of permissions and remove permissions for any 
    // user with a display name or SMTP address. This leaves the anonymous and 
    // default user permissions unchanged. 
    if (sentItemsFolder.Permissions.Count != 0)
    {
        for (int t = 0; t < sentItemsFolder.Permissions.Count; t++)
        {
            // Find any permissions associated with the specified user and remove them from the DACL
            if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
            {
                sentItemsFolder.Permissions.Remove(sentItemsFolder.Permissions[t]);
            }
        }
    }
    // This call results in an UpdateFolder call to EWS.
    sentItemsFolder.Update();
}
```

## <a name="removing-folder-permissions-by-using-ews"></a>Suppression des autorisations de dossier à l’aide d’EWS
<a name="bk_removeews"> </a>

Les exemples de code EWS suivants montrent comment supprimer toutes les autorisations utilisateur sur un dossier spécifique, à l’exception des autorisations par défaut et anonymes.
  
Tout d’abord, envoyez une demande [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) dans laquelle la valeur [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) spécifie le dossier dans lequel supprimer les autorisations (le dossier Éléments envoyés dans cet exemple) et la valeur [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) inclut folder:PermissionSet. Cette demande récupère le [PermissionSet pour](https://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) le dossier spécifié. 
  
Il s’agit également de la demande XML que l’API gérée EWS envoie lorsque vous appelez la méthode **Bind** pour supprimer des [autorisations de dossier.](#bk_removeewsma)
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:PermissionSet" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="drafts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **GetFolder** avec un message [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, qui indique que le dossier a été récupéré avec succès. Les valeurs des éléments **FolderId** et **ParentFolderId** ont été raccourcies pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="EAAAAA=="
                          ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd5" />
              <t:ParentFolderId Id="CQAAAA=="
                                ChangeKey="AQAAAA==" />
              <t:FolderClass>IPF.Note</t:FolderClass>
              <t:DisplayName>Drafts</t:DisplayName>
              <t:TotalCount>0</t:TotalCount>
              <t:ChildFolderCount>0</t:ChildFolderCount>
              <t:EffectiveRights>
                <t:CreateAssociated>true</t:CreateAssociated>
                <t:CreateContents>true</t:CreateContents>
                <t:CreateHierarchy>true</t:CreateHierarchy>
                <t:Delete>true</t:Delete>
                <t:Modify>true</t:Modify>
                <t:Read>true</t:Read>
                <t:ViewPrivateItems>true</t:ViewPrivateItems>
              </t:EffectiveRights>
              <t:PermissionSet>
                <t:Permissions>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Default</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:SID>S-1-5-21-1337771579-694202782-848329751-1535223</t:SID>
                      <t:PrimarySmtpAddress>sadie@Contoso.com</t:PrimarySmtpAddress>
                      <t:DisplayName>Sadie Daniels</t:DisplayName>
                    </t:UserId>
                    <t:CanCreateItems>true</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>true</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>All</t:EditItems>
                    <t:DeleteItems>All</t:DeleteItems>
                    <t:ReadItems>FullDetails</t:ReadItems>
                    <t:PermissionLevel>Editor</t:PermissionLevel>
                  </t:Permission>
                </t:Permissions>
              </t:PermissionSet>
              <t:UnreadCount>0</t:UnreadCount>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

Ensuite, utilisez **l’opération UpdateFolder** pour envoyer le **PermissionSet** mis à jour, qui n’inclut pas l’autorisation pour l’utilisateur supprimé.  
  
Il s’agit également de la demande XML que l’API gérée EWS envoie lorsque vous appelez la méthode **Update** pour supprimer des [autorisations de dossier.](#bk_removeewsma)
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="EAAAAA=="
                      ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd5" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:PermissionSet" />
              <t:Folder>
                <t:PermissionSet>
                  <t:Permissions>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Default</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                  </t:Permissions>
                </t:PermissionSet>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **UpdateFolder** avec un message **UpdateFolderResponse** qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, qui indique que la mise à jour a réussi.
  
## <a name="updating-folder-permissions-by-using-the-ews-managed-api"></a>Mise à jour des autorisations de dossier à l’aide de l’API gérée EWS
<a name="bk_updateewsma"> </a>

Vous pouvez également mettre à jour les autorisations de dossier pour un dossier spécifique à l’aide de l’API gérée EWS. Pour mettre à jour les autorisations : 
  
1. [Supprimez les autorisations de dossier](#bk_removeewsma) pour les autorisations obsolètes, mais n’appelez pas la méthode **Update** (encore). 
    
2. [Ajoutez des autorisations de dossier pour les utilisateurs nouveaux ou modifiés.](#bk_enableewsma)
    
3. Appelez la **méthode Update** pour enregistrer les modifications. 
    
Si vous essayez d’ajouter deux ensembles d’autorisations pour le même utilisateur, vous recevrez une erreur **ServiceResponseException** avec la description suivante : « Le jeu d’autorisations spécifié contient des UserId en double ». Dans ce cas, supprimez les autorisations actuelles de la collection **Permission,** puis ajoutez les nouvelles autorisations à la collection **Permission.** 
  
## <a name="updating-folder-permissions-by-using-ews"></a>Mise à jour des autorisations de dossier à l’aide d’EWS
<a name="bk_updateews"> </a>

Vous pouvez également mettre à jour les autorisations de dossier pour des dossiers spécifiques à l’aide d’EWS en combinant le processus de suppression et d’ajout. Pour mettre à jour les autorisations : 
  
1. Récupérez les autorisations actuelles du dossier à l’aide de **l’opération GetFolder.** 
    
2. Envoyez une liste mise à jour des autorisations à l’aide de **l’opération UpdateFolder.** 
    
Ces deux opérations sont les mêmes que celles que vous utilisez pour [activer](#bk_enableews) ou supprimer [l’accès](#bk_removeews) à l’aide d’EWS. La seule différence est que lorsque vous recevez la réponse **GetFolder,** elle contient un jeu **d’autorisations** pour l’utilisateur. Remplacez simplement cet élément **Permission** existant par le nouvel élément **Permission,** puis envoyez l’opération **UpdateFolder** par la ou les nouvelles valeurs **Permission.** 
  
Si vous essayez d’ajouter deux ensembles d’autorisations pour le même utilisateur, vous recevrez une valeur **ResponseCode** de **ErrorDuplicateUserIdsSpecified**. Dans ce cas, supprimez la valeur d’autorisation obsolète pour l’utilisateur de la demande, puis réessayez la demande.

## <a name="next-steps"></a>Étapes suivantes

Après avoir donné à un utilisateur l’autorisation d’accéder à un dossier spécifique, il peut accéder au dossier en tant que délégué. Pour plus d’informations, voir :
  
- [Accéder à la messagerie en tant que délégué à l’aide d’EWS dans Exchange](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Accéder à un calendrier en tant que délégué à l’aide d’EWS dans Exchange](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Accéder aux contacts en tant que délégué à l’aide d’EWS dans Exchange](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi

- [Accès délégué et EWS dans Exchange](delegate-access-and-ews-in-exchange.md)   
- [Ajouter et supprimer des délégués à l’aide d’EWS dans Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [Dossiers et éléments dans EWS dans Exchange](folders-and-items-in-ews-in-exchange.md)
    

