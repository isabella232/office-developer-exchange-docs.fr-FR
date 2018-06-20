---
title: Définir des autorisations de dossier pour un autre utilisateur à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7eb81676-a780-4c56-b4f2-c4ed2697107d
description: Découvrez comment définir des niveaux d’autorisation sur un dossier à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 5bf570612d6349628e7f3abf858daa33daa13745
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754946"
---
# <a name="set-folder-permissions-for-another-user-by-using-ews-in-exchange"></a>Définir des autorisations de dossier pour un autre utilisateur à l’aide de EWS dans Exchange

Découvrez comment définir des niveaux d’autorisation sur un dossier à l’aide de l’API managée EWS ou EWS dans Exchange.
  
Autorisations au niveau du dossier permettent aux utilisateurs d’accéder à un ou plusieurs dossiers dans la boîte aux lettres d’un autre utilisateur. Autorisations de dossier sont similaires aux accès délégué, mais elles diffèrent comme suit : 
  
- Autorisations du dossier n’activez pas un utilisateur « envoyer de la part de » ou « envoyer en tant que « un autre utilisateur. Ils autorisent l’accès aux dossiers uniquement. Les utilisateurs peuvent créer des éléments dans les dossiers, mais ils ne peuvent pas les envoyer.
    
- Vous pouvez définir des autorisations sur le dossier sur n’importe quel dossier dans la boîte aux lettres, mais vous ne pouvez ajouter un délégué dans les dossiers Calendrier, Contacts, boîte de réception, Journal, Notes et tâches.
    
- Vous pouvez définir un nombre [d’autorisations sur un dossier spécifique](#bk_folderperms). Lorsque vous ajoutez un délégué, vous pouvez affecter un des seuls [cinq niveaux d’autorisation](delegate-access-and-ews-in-exchange.md#bk_delegateperms).
    
- Vous pouvez définir des autorisations de dossier pour anonyme et par défaut les utilisateurs. Vous pouvez uniquement accorder l’accès délégué à un compte de messagerie.
    
Si vous êtes familiarisé avec les entrées de contrôle d’accès (ACE) et les listes de contrôle d’accès discrétionnaire (DACL), vous savez qu’un utilisateur peut avoir uniquement un ensemble d’autorisations pour chaque dossier. Si vous essayez d’ajouter un jeu d’autorisations pour un utilisateur et qu’ils possèdent déjà un ensemble d’autorisations, vous obtiendrez une erreur. Lorsque vous ajoutez, supprimez ou mettre à jour les autorisations sur un dossier, vous obtenez la liste DACL en cours, ajoutez ou supprimez tout ACE et puis envoyez la liste DACL mis à jour. Vous ne pouvez pas ajouter plusieurs entrées pour le même utilisateur. Lorsque vous mettez à jour les autorisations à l’aide de l’API managée EWS, vous devez supprimer actuel ACE l’utilisateur, puis ajouter leur nouveaux ACE à la collection. Si vous utilisez EWS, vous il suffit de remplacer l’ensemble des ACE précédente avec les nouveaux.
  
Si vous effectuez plusieurs modifications des autorisations à un dossier unique, vous pouvez par lot ajouts, suppressions et mises à jour, veuillez noter que vous ne pouvez pas par lots mises à jour de l’utilisateur sur plusieurs dossiers. Un appel est nécessaire pour obtenir les autorisations sur un dossier unique et un deuxième appel est nécessaire pour mettre à jour les autorisations sur ce dossier. Lorsque vous ajoutez, supprimez ou mettre à jour les autorisations des utilisateurs, utilisez la même méthode deux appels ou opérations pour chaque tâche.
  
**Le tableau 1. Méthodes d’API managées et opérations EWS pour définir les autorisations de dossier**

|Si vous souhaitez...|Utilisez cette méthode d’API managées...|Utilisez cette opération EWS...|
|:-----|:-----|:-----|
|Activer, supprimer ou mettre à jour les autorisations de dossier  <br/> |[Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) suivi [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) <br/> |[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) suivi [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|Créez un dossier et définir les autorisations du dossier  <br/> |[Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
   
## <a name="folder-permissions"></a>Autorisations de dossier
<a name="bk_folderperms"> </a>

Vous avez quelques options en matière de définition d’autorisations de dossier sur un dossier spécifique. Vous pouvez définir un niveau d’autorisation sur un dossier pour chaque utilisateur, qui ajoute un jeu d’autorisations individuelles prédéfinis à la liste DACL, ou vous pouvez définir des autorisations individuelles dans un dossier, mais vous ne pouvez pas combiner des.
  
Les autorisations spécifiques suivantes sont disponibles :
  
- Peut créer
- Peut créer des sous-dossiers    
- Est le propriétaire du dossier    
- Dossier est visible    
- Dossier contact    
- Modifier des éléments    
- Supprimer des éléments    
- Lire des éléments
    
En outre, les niveaux d’autorisation suivants sont disponibles, qui définissent un sous-ensemble des autorisations spécifiques et les valeurs, comme indiqué dans le tableau 2 :
  
- Aucun    
- Owner    
- Détenir    
- Editor    
- PublishingAuthor    
- Auteur    
- NoneditingAuthor    
- Reviewer    
- Collaborateur   
- Personnalisé - cette valeur ne peut pas être définie par l’application. Le serveur définit cette valeur si l’application comporte une collection personnalisée d’autorisations individuelles.    
- FreeBusyTimeOnly - il ne peut être définie sur dossiers de calendrier.   
- FreeBusyTimeAndSubjectAndLocation - il ne peut être définie sur dossiers de calendrier.
    
Le tableau suivant indique les autorisations spécifiques sont appliquées par défaut selon le niveau d’autorisation.
  
**Le tableau 2. Autorisations spécifiques à un niveau d’autorisation**

|Niveau d’autorisation|Peut créer des éléments|Peut créer des sous-dossiers|Est le propriétaire du dossier|Dossier est visible|Dossier contact|Modifier des éléments|Supprimer des éléments|Peut lire des éléments|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Aucun  <br/> |Faux  <br/> |Faux  <br/> |Faux  <br/> |Faux  <br/> |Faux  <br/> |Aucune  <br/> |Aucune  <br/> |Aucune  <br/> |
|Owner  <br/> |True  <br/> |True  <br/> |True  <br/> |True  <br/> |True  <br/> |Tous  <br/> |Tous  <br/> |FullDetails  <br/> |
|Détenir  <br/> |True  <br/> |True  <br/> |Faux  <br/> |True  <br/> |Faux  <br/> |Tous  <br/> |Tous  <br/> |FullDetails  <br/> |
|Editor  <br/> |True  <br/> |Faux  <br/> |Faux  <br/> |True  <br/> |Faux  <br/> |Tous  <br/> |Tous  <br/> |FullDetails  <br/> |
|PublishingAuthor  <br/> |True  <br/> |True  <br/> |Faux  <br/> |True  <br/> |Faux  <br/> |Propriétaire  <br/> |Propriétaire  <br/> |FullDetails  <br/> |
|Auteur  <br/> |True  <br/> |Faux  <br/> |Faux  <br/> |True  <br/> |Faux  <br/> |Propriétaire  <br/> |Propriétaire  <br/> |FullDetails  <br/> |
|NoneditingAuthor  <br/> |True  <br/> |Faux  <br/> |Faux  <br/> |True  <br/> |Faux  <br/> |Aucun  <br/> |Propriétaire  <br/> |FullDetails  <br/> |
|Reviewer  <br/> |Faux  <br/> |Faux  <br/> |Faux  <br/> |True  <br/> |Faux  <br/> |Aucune  <br/> |Aucune  <br/> |FullDetails  <br/> |
|Collaborateur  <br/> |True  <br/> |Faux  <br/> |Faux  <br/> |True  <br/> |Faux  <br/> |Aucune  <br/> |Aucune  <br/> |Aucune  <br/> |
   
Si vous spécifiez un niveau d’autorisation non personnalisée dans la demande d’autorisations au niveau du dossier, vous n’avez pas besoin de spécifier les paramètres d’autorisation spécifiques. Si vous spécifiez une autorisation lorsque vous définissez un niveau d’autorisation, une erreur **ErrorInvalidPermissionSettings** est renvoyée dans la réponse. 
  
## <a name="adding-folder-permissions-by-using-the-ews-managed-api"></a>Ajout d’autorisations sur le dossier à l’aide de l’API managée EWS
<a name="bk_enableewsma"> </a>

L’exemple de code suivant montre comment utiliser l’API managée EWS pour : 
  
- Créer un nouvel objet [FolderPermission](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) pour le nouvel utilisateur. 
    
- Obtenez les autorisations en cours d’un dossier à l’aide de la méthode [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) . 
    
- Ajoutez la nouvelle **FolderPermissions** à la propriété [Folder.Permissions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) . 
    
- Appelez la méthode [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) pour enregistrer les nouvelles autorisations sur le serveur. 
    
Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le propriétaire de boîte aux lettres et que l’utilisateur a été authentifié sur un serveur Exchange. 
  
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

Si vous souhaitez utiliser le niveau d’autorisation personnalisé, utilisez plutôt ce code.
  
```cs
FolderPermission fldperm = new FolderPermission();
fldperm.UserId = "sadie@Contoso1000.onmicrosoft.com";
fldperm.CanCreateItems = true;
fldperm.CanCreateSubFolders = true;
…
```

Lorsque vous créez un objet **FolderPermission** avec un niveau d’autorisation personnalisé, vous pouvez définir tout ou partie des [Propriétés FolderPermission](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx) accessibles en écriture. Notez que le [FolderPermissionLevel](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) n’est jamais explicitement définie sur **personnalisé** par l’application. Le **FolderPermissionLevel** est définie sur personnalisé uniquement lorsque vous créez un objet **FolderPermission** et définissez des autorisations individuelles. 
  
## <a name="adding-folder-permissions-by-using-ews"></a>Ajout d’autorisations sur le dossier à l’aide de EWS
<a name="bk_enableews"> </a>

Les exemples de code EWS suivantes montrent comment ajouter des autorisations à un dossier spécifique à extraire les autorisations en cours et ensuite envoyer une liste des nouvelles autorisations.
  
La première étape consiste à envoyer une requête [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , où la valeur [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) Spécifie le dossier dans lequel ajouter des autorisations (le dossier éléments envoyés dans cet exemple) et la valeur [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) inclut le dossier : PermissionSet. Cette requête récupère les paramètres d’autorisation pour le dossier spécifié. 
  
C’est également la demande XML qui envoie de l’API managée EWS lorsque vous appelez la méthode **Bind** pour [Ajouter des autorisations de dossier](#bk_enableewsma).
  
```XML
  <?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

Le serveur répond à la demande **GetFolder** avec un message [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le dossier a été récupéré correctement. Les valeurs [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) et [ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) ont été raccourcies pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Ensuite, utilisez l’opération **UpdateFolder** pour envoyer la mise à jour [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx), qui inclut l' [autorisation](http://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) pour le nouvel utilisateur. Notez que, y compris l’élément [SetFolderField](http://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) pour le dossier respectif dans l’opération [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) remplacera tous les paramètres d’autorisation sur le dossier. De même, y compris l’option [DeleteFolderField](http://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) de l’opération **UpdateFolder** supprime également tous les paramètres d’autorisation sur le dossier. 
  
C’est également la demande XML qui envoie de l’API managée EWS lorsque vous appelez la méthode **Update** pour [Ajouter des autorisations de dossier](#bk_enableewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

Si vous souhaitez utiliser le niveau d’autorisation personnalisé, utilisez plutôt ce code.
  
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

Le serveur répond à la demande **UpdateFolder** avec un message [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le dossier a été correctement mis à jour.
  
## <a name="removing-folder-permissions-by-using-the-ews-managed-api"></a>Suppression des autorisations de dossiers à l’aide de l’API managée EWS
<a name="bk_removeewsma"> </a>

L’exemple de code suivant montre comment utiliser l’API managée EWS pour supprimer toutes les autorisations utilisateur sur un dossier spécifique, à l’exception de par défaut et les autorisations anonymes, à :
  
1. Obtenir les autorisations en cours d’un dossier à l’aide de la méthode **Bind** . 
    
2. Parcourir la collection **d’autorisations** et suppression des autorisations pour des utilisateurs individuels. 
    
3. L’appel de la méthode **Update** pour enregistrer les modifications. 
    
Cet exemple supprime toutes les autorisations utilisateur sur un dossier. Si vous souhaitez modifier cet exemple pour supprimer des autorisations uniquement pour un utilisateur spécifique, modifiez la ligne suivante de code pour identifier le nom complet ou l’adresse SMTP de l’utilisateur.
  
```cs
if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
```

Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le propriétaire de boîte aux lettres et que l’utilisateur a été authentifié sur un serveur Exchange. 
  
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

## <a name="removing-folder-permissions-by-using-ews"></a>Suppression des autorisations de dossiers à l’aide de EWS
<a name="bk_removeews"> </a>

Les exemples de code EWS suivants montrent comment supprimer toutes les autorisations utilisateur sur un dossier spécifique, sauf pour les autorisations anonymes et par défaut.
  
Tout d’abord, envoyez une requête de [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) où la valeur [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) Spécifie le dossier dans lequel supprimer les autorisations (le dossier éléments envoyés dans cet exemple) et la valeur [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) inclut le dossier : PermissionSet. Cette requête extrait le [jeu d’autorisations](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) pour le dossier spécifié. 
  
C’est également la demande XML qui envoie de l’API managée EWS lorsque vous appelez la méthode **Bind** pour [Supprimer les autorisations du dossier](#bk_removeewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

Le serveur répond à la demande **GetFolder** avec un message [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le dossier a été récupéré correctement. Les valeurs des éléments **FolderId** et **ParentFolderId** ont été raccourcies pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Ensuite, utilisez l’opération **UpdateFolder** pour envoyer la mise à jour **PermissionSet**, qui n’inclut pas l' **autorisation** de l’utilisateur supprimé. 
  
C’est également la demande XML qui envoie de l’API managée EWS lorsque vous appelez la méthode de **mise à jour** pour [Supprimer les autorisations du dossier](#bk_removeewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

Le serveur répond à la demande **UpdateFolder** avec un message **UpdateFolderResponse** qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que la mise à jour a réussi.
  
## <a name="updating-folder-permissions-by-using-the-ews-managed-api"></a>Mise à jour des autorisations de dossiers à l’aide de l’API managée EWS
<a name="bk_updateewsma"> </a>

Vous pouvez également mettre à jour les autorisations du dossier pour un dossier spécifique à l’aide de l’API managée EWS. Pour mettre à jour les autorisations : 
  
1. [Supprimer les autorisations de dossier](#bk_removeewsma) pour les autorisations obsolètes, mais vous n’appelez pas la méthode de **mise à jour** (encore). 
    
2. [Ajouter des autorisations de dossier pour les utilisateurs nouveaux ou modifiés](#bk_enableewsma).
    
3. Appelez la méthode **Update** pour enregistrer les modifications. 
    
Si vous essayez d’ajouter deux jeux d’autorisations pour le même utilisateur, vous recevrez une erreur **ServiceResponseException** avec la description suivante : « le jeu d’autorisations spécifié contient les ID utilisateur en double ». Dans ce cas, supprimez les autorisations en cours de la collection **Permission** , puis ajoutez les nouvelles autorisations à la collection **Permission** . 
  
## <a name="updating-folder-permissions-by-using-ews"></a>Mise à jour des autorisations de dossiers à l’aide de EWS
<a name="bk_updateews"> </a>

Vous pouvez également mettre à jour des autorisations de dossiers pour des dossiers spécifiques à l’aide de EWS en combinant le processus de suppression et d’ajout. Pour mettre à jour les autorisations : 
  
1. Récupérer les autorisations du dossier en cours à l’aide de l’opération **GetFolder** . 
    
2. Envoyer une liste mise à jour des autorisations à l’aide de l’opération **UpdateFolder** . 
    
Voici les deux opérations même que vous utilisez pour [Activer](#bk_enableews) ou [Supprimer l’accès](#bk_removeews) à l’aide de EWS. La seule différence est que lorsque vous recevez la réponse **GetFolder** , il contient un jeu d' **autorisations** pour l’utilisateur. Remplacez simplement cet élément **d’autorisation** existant par le nouvel élément **d’autorisation** , puis envoyer l’opération **UpdateFolder** avec la nouvelle valeur **d’autorisation** ou les valeurs. 
  
Si vous essayez d’ajouter deux jeux d’autorisations pour le même utilisateur, vous recevrez une valeur **ResponseCode** **ErrorDuplicateUserIdsSpecified**. Dans ce cas, supprimez la valeur d’autorisation obsolète pour l’utilisateur de la demande et réessayez d’exécuter la requête.

## <a name="next-steps"></a>Étapes suivantes

Une fois que vous autorisez un utilisateur à un dossier spécifique, l’utilisateur peut accéder au dossier en tant que délégué. Pour plus d’informations, voir :
  
- [Accéder à la messagerie en tant que délégué à l’aide de EWS dans Exchange](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Accéder à un calendrier en tant que délégué à l’aide de EWS dans Exchange](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Contacts Access en tant que délégué à l’aide de EWS dans Exchange](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi

- [Accès délégué et EWS dans Exchange](delegate-access-and-ews-in-exchange.md)   
- [Ajouter et supprimer des délégués à l’aide de EWS dans Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [Dossiers et éléments dans EWS dans Exchange](folders-and-items-in-ews-in-exchange.md)
    

