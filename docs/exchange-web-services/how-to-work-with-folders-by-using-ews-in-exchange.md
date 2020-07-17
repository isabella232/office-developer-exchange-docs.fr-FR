---
title: Utiliser des dossiers à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 4b3eb746-74c4-42a0-aa2c-742c147f1871
description: Découvrez comment créer, obtenir, mettre à jour et supprimer des dossiers à l’aide de l’API managée EWS ou d’EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: c09c0c76edda4af025a6ac7121fdf9ab9660fcab
ms.sourcegitcommit: eeda51cb037aa25566adb293f25574674fdb2d9e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45012544"
---
# <a name="work-with-folders-by-using-ews-in-exchange"></a>Utiliser des dossiers à l’aide d’EWS dans Exchange

Découvrez comment créer, obtenir, mettre à jour et supprimer des dossiers à l’aide de l’API managée EWS ou d’EWS dans Exchange.
  
EWS dans Exchange utilise des dossiers pour structurer et organiser les boîtes aux lettres. Vous pouvez créer de nouveaux dossiers, obtenir, mettre à jour et supprimer des dossiers à l’aide de l’API managée EWS ou d’EWS. Chacune des méthodes ou opérations indiquées dans le tableau suivant est exécutée sur un objet [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) , un type [Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) ou l' [une des classes ou types de dossier dérivés](folders-and-items-in-ews-in-exchange.md#bk_folders).
  
**Tableau 1. Méthodes et opérations de création, d’obtention, de mise à jour et de suppression de dossiers**

|**Afin de...**|**Méthode d'API managée EWS**|**Opération EWS**|
|:-----|:-----|:-----|
|Créer un dossier  <br/> |[Folder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|Créer une hiérarchie de dossiers  <br/> |Non disponible  <br/> |[CreateFolderPath](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |
|Obtenir un dossier  <br/> |[Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |[GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|Obtenir une hiérarchie de dossiers  <br/> |[Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> |[FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
|Mettre à jour un dossier  <br/> |[Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|Supprimer un dossier  <br/> |[Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |

<a name="bk_createfolderewsma"> </a>

## <a name="create-a-folder-by-using-the-ews-managed-api"></a>Créer un dossier à l’aide de l’API managée EWS

L’exemple de code suivant montre comment utiliser la classe [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) pour créer un nouveau dossier générique avec un [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) de « Custom Folder » et une valeur de propriété [FolderClass](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) de IPF. Note. La méthode [Folder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) enregistre le dossier en tant que dossier enfant du dossier boîte de réception. 
  
Ces exemples supposent que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié auprès d’un serveur Exchange. 
  
```csharp
// Create a custom folder.
Folder folder = new Folder(service);
folder.DisplayName = "Custom Folder";
folder.FolderClass = "IPF.Note";
// Save the folder as a child folder of the Inbox.
folder.Save(WellKnownFolderName.Inbox);
```

Pour créer un autre type de dossier, tel qu’un [CalendarFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx), [ContactsFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx), [SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)ou [TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx), créez une instance de la classe spécifique (au lieu de la classe de **dossier** générique) et ne définissez pas la propriété **FolderClass** . Par exemple, l’exemple de code suivant montre comment créer un nouveau [TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx).
  
```csharp
// Create a custom Tasks folder.
TasksFolder folder = new TasksFolder(service);
folder.DisplayName = "Custom Tasks";
// Save the folder as a child folder in the Inbox folder.
// This method call results in a CreateFolder call to EWS.
folder.Save(WellKnownFolderName.Inbox);
```

Si vous essayez de créer une instance d’une classe spécifique et que vous définissez également la propriété **FolderClass** , l’erreur [ErrorNoFolderClassOverride](https://msdn.microsoft.com/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) est générée. 
  
Notez que vous ne pouvez pas créer par lots la création de plusieurs dossiers dans un seul appel de méthode à l’aide de l’API managée EWS.
  
## <a name="create-a-folder-by-using-ews"></a>Créer un dossier à l’aide d’EWS
<a name="bk_createfolderews"> </a>

Vous pouvez créer un seul dossier ou plusieurs dossiers à l’aide d’EWS.
  
Pour créer un dossier unique, envoyez un message de demande d’opération [CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) . La demande d’opération **CreateFolder** indique que le dossier parent est la boîte de réception, que [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) est « dossier personnalisé » et que la valeur de l’élément [FolderClass](https://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) est IPF. Note. 
  
Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous créez un nouveau dossier et appelez la méthode [Folder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) . 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateFolder>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderId>
      <m:Folders>
        <t:Folder>
          <t:FolderClass>IPF.Note</t:FolderClass>
          <t:DisplayName>Custom Folder</t:DisplayName>
        </t:Folder>
      </m:Folders>
    </m:CreateFolder>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **CreateFolder** avec un message [CreateFolderResponse](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NOERROR**, ce qui indique que le dossier a été créé avec succès et le [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) du message nouvellement créé. 
  
Pour créer plusieurs dossiers, incluez plusieurs éléments de [dossier](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) dans le message de demande d’opération **CreateFolder** . Tous les nouveaux dossiers doivent se trouver dans le même dossier parent. 
  
## <a name="create-a-folder-hierarchy-by-using-ews"></a>Créer une hiérarchie de dossiers à l’aide d’EWS
<a name="bk_createfolderhierarchy"> </a>

Vous pouvez créer une hiérarchie de dossiers dans un seul appel à l’aide de l’opération EWS [CreateFolderPath](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) . Les mêmes fonctionnalités ne sont pas disponibles dans l’API managée EWS. Au lieu de cela, si vous utilisez l’API managée EWS, vous pouvez créer des dossiers un par un, comme illustré dans [créer un dossier à l’aide d’EWS](#bk_createfolderews).
  
> [!NOTE]
> L’API managée EWS n’implémente pas cette fonctionnalité. 
  
## <a name="get-a-folder-by-using-the-ews-managed-api"></a>Obtenir un dossier à l’aide de l’API managée EWS
<a name="bk_getfolderewsma"> </a>

L’exemple de code suivant montre comment utiliser la méthode [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) pour obtenir le dossier boîte de réception. Il est recommandé de limiter les propriétés renvoyées à celles requises pour votre application. Cet exemple limite les propriétés de retour à inclure uniquement la propriété [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) en créant un objet [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) et en appliquant la valeur [IdOnly](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) à la propriété [BasePropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) . 
  
Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange. 
  
```csharp
// As a best practice, limit the properties returned to only those that are required.
// In this scenario, you only need the FolderId.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get only the properties specified in the PropertySet.
// This method call results in a GetFolder call to EWS.
Folder rootfolder = Folder.Bind(service, WellKnownFolderName.Inbox, propSet);
```

Si vous devez renvoyer des propriétés supplémentaires, ajoutez des propriétés à partir de la classe [FolderSchema](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) à la classe **PropertySet**ou utilisez l’une des méthodes de [liaison](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) surchargées qui renvoie toutes les propriétés de première classe. 
  
Notez que vous ne pouvez pas obtenir plusieurs dossiers à la fois à l’aide de l’API managée EWS. Vous devez appeler la méthode **Bind** sur chaque dossier séparément. 
  
## <a name="get-a-folder-by-using-ews"></a>Obtenir un dossier à l’aide d’EWS
<a name="bk_getfolderews"> </a>

Vous pouvez obtenir un dossier ou plusieurs dossiers à l’aide d’EWS.
  
Pour obtenir un seul dossier, envoyez un message de demande d’opération [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) au serveur. Dans l’exemple suivant, le [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) est défini sur **IdOnly**, de sorte que seul le [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) du dossier spécifié est retourné. L’élément [FolderIds](https://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) indique que le dossier à récupérer est le dossier boîte de réception. 
  
Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous liez un dossier à l’aide de la méthode [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) . 
  
Pour obtenir plusieurs dossiers, incluez plusieurs éléments [FolderIds](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) dans le message de demande d’opération **GetFolder** . 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

L’exemple de code XML suivant montre le message [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) envoyé par le serveur au client en réponse à la demande d’opération **GetFolder** . Il contient uniquement la valeur [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) du dossier boîte de réception. Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité. 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="800"
                         MinorBuildNumber="16"
                         Version="V2_6"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
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
              <t:FolderId Id="AAAENAAA=" ChangeKey="AQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAEkbCr"/>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="get-a-folder-hierarchy-by-using-the-ews-managed-api"></a>Obtenir une hiérarchie de dossiers à l’aide de l’API managée EWS
<a name="bk_getfolderhierarchyewsma"> </a>

L’exemple de code suivant montre comment récupérer les sous-dossiers d’un dossier racine spécifié. Cet exemple récupère les sous-dossiers du dossier **MsgFolderRoot** , qui est la racine de la sous-arborescence IPM (où sont stockés vos dossiers et éléments de boîte aux lettres). 
  
Dans cet exemple, un objet de classe [folderview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) est créé pour limiter les résultats de la réponse de la méthode [Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) . Ce scénario limite les propriétés à renvoyer aux éléments suivants : [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx), [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx)et la propriété étendue qui indique si le dossier est un dossier masqué. Définissez la valeur [folderview. Traversal](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) sur Deep pour effectuer une recherche récursive afin que le serveur récupère les sous-dossiers et définissez le dossier racine sur **MsgFolderRoot**, de sorte que le serveur renvoie tous les dossiers de l’utilisateur (et que le serveur ne retourne pas les dossiers système dans la sous-arborescence non IPM).
  
Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange. 
  
```csharp
// Create a new folder view, and pass in the maximum number of folders to return.
FolderView view = new FolderView(folderViewSize);
// Create an extended property definition for the PR_ATTR_HIDDEN property,
// so that your results will indicate whether the folder is a hidden folder.
ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
// As a best practice, limit the properties returned to only those required.
// In this case, return the folder ID, DisplayName, and the value of the isHiddenProp
// extended property.
view.PropertySet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.DisplayName, isHiddenProp);
// Indicate a Traversal value of Deep, so that all subfolders are retrieved.
view.Traversal = FolderTraversal.Deep;
// Call FindFolders to retrieve the folder hierarchy, starting with the MsgFolderRoot folder.
// This method call results in a FindFolder call to EWS.
FindFoldersResults findFolderResults = service.FindFolders(WellKnownFolderName.MsgFolderRoot, view);
```

## <a name="get-a-folder-hierarchy-by-using-ews"></a>Obtenir une hiérarchie de dossiers à l’aide d’EWS
<a name="bk_getfolderhierarchyews"> </a>

Les exemples XML suivants montrent comment utiliser l’opération [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) pour récupérer une hiérarchie de dossiers à l’aide d’EWS. Cet exemple récupère le dossier **msgfolderroot** , qui est la racine de la sous-arborescence IPM et tous ses sous-dossiers. L’attribut **Traversal** est défini sur **Deep** afin que le serveur effectue une recherche récursive de la hiérarchie de dossiers et renvoie uniquement les dossiers et sous-dossiers sous la racine spécifiée dans la réponse. Dans cet exemple, l’élément [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) est défini sur **IdOnly** de sorte que le serveur ne renvoie que l’élément [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) . Pour faciliter la compréhension de la sortie, incluez l’élément **DisplayName** dans vos résultats en l’incluant dans l’élément [AdditionalProperties](https://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) de la demande, ainsi que la valeur **ExtendedFieldURI** pour la propriété **PR_ATTR_HIDDEN** , afin de savoir si les dossiers sont des dossiers cachés. 
  
Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous appelez la méthode [FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) . 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Deep">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="100"
                               Offset="0"
                               BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="msgfolderroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

L’exemple de code XML suivant montre le message [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) envoyé par le serveur au client en réponse à la demande d’opération **FindFolder** . Il contient uniquement les [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx), [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx)et la valeur de la propriété étendue **PR_ATTR_HIDDEN** pour tous les sous-dossiers sous le dossier **msgrootfolder** Si l’élément [value](https://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) est défini sur true, le dossier doit être masqué dans l’affichage client. 
  
Il s’agit également de la réponse XML que l’API managée EWS envoie lorsque vous obtenez plusieurs dossiers à l’aide de la méthode [FindFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) . Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité, et certains dossiers n’ont pas été inclus à des fins de concision. 
  
```xml
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="815"
                         MinorBuildNumber="6"
                         Version="V2_7"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="16"
                        TotalItemsInView="16"
                        IncludesLastItemInRange="true">
            <t:Folders>
              <t:CalendarFolder>
                <t:FolderId Id="AAAEOAAA="
                            ChangeKey="AgAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAA3"/>
                <t:DisplayName>Calendar</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>false</t:Value>
                </t:ExtendedProperty>
              </t:CalendarFolder>
              <t:ContactsFolder>
                <t:FolderId Id="AAAEPAAA="
                            ChangeKey="AwAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAA4"/>
                <t:DisplayName>Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>false</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="AAAUKAAA="
                            ChangeKey="AwAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAS5"/>
                <t:DisplayName>Recipient Cache</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="AAAUJAAA="
                            ChangeKey="AQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAASx"/>
                <t:DisplayName>Conversation Action Settings</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
…
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="update-a-folder-by-using-the-ews-managed-api"></a>Mettre à jour un dossier à l’aide de l’API managée EWS
<a name="bk_updatefolderewsma"> </a>

L’exemple de code suivant montre comment mettre à jour le nom d’affichage d’un dossier à l’aide de l’API managée EWS.
  
Tout d’abord, créez un [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) pour limiter le nombre de propriétés renvoyées par le serveur dans la réponse [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) . Nous vous recommandons d’utiliser le **IdOnly** **BasePropertySet** pour réduire les appels à la base de données Exchange. Ensuite, utilisez la méthode **Bind** pour établir une liaison avec le dossier à mettre à jour. Ensuite, mettez à jour la propriété [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) et utilisez la méthode [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) pour enregistrer les modifications. 
  
Dans cet exemple, nous partons du principe que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié auprès d’un serveur Exchange. La variable locale *FolderId* est l' [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) du dossier à mettre à jour. 
  
```cs
// As a best practice, only include the ID value in the PropertySet.
PropertySet propertySet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get the FolderId.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId, propertySet);
// Update the display name of the folder.
folder.DisplayName = "Updated folder name";
// Save the updates.
// This method call results in an UpdateFolder call to EWS.
folder.Update();

```

## <a name="update-a-folder-by-using-ews"></a>Mettre à jour un dossier à l’aide d’EWS
<a name="bk_updatefolderews"> </a>

Les exemples XML suivants montrent comment mettre à jour le nom d’affichage d’un dossier à l’aide d’EWS.
  
Tout d’abord, envoyez un message de demande d’opération [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) pour obtenir le dossier à mettre à jour, comme illustré dans [obtenir une hiérarchie de dossiers à l’aide d’EWS](#bk_getfolderhierarchyews).
  
Ensuite, envoyez un message de demande d’opération [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) au serveur pour mettre à jour un dossier. La demande d’opération **UpdateFolder** met à jour la valeur [DisplayName](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) sur « mise à jour du dossier personnalisé ». 
  
Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous mettez à jour un dossier à l’aide de la méthode [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) . Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité. 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="OrV9ZAAA=" ChangeKey="AQAAABYAAABVzRdyy/cHS4XTC9itCRdUAAAOrXWb" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:DisplayName" />
              <t:Folder>
                <t:DisplayName>Updated Custom Folder</t:DisplayName>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **UpdateFolder** avec un message [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) qui inclut la valeur [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de la propriété **NOERROR**et la [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) du dossier qui a été mise à jour avec une valeur d’attribut **ChangeKey** mise à jour. 
  
## <a name="delete-a-folder-by-using-the-ews-managed-api"></a>Supprimer un dossier à l’aide de l’API managée EWS
<a name="bk_deletefolderewsma"> </a>

Cet article fournit un exemple de base qui vous montre comment supprimer un dossier à l’aide de l’API managée EWS. Pour plus d’informations sur la suppression de dossiers, consultez [la rubrique Suppression d’éléments à l’aide d’EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md).
  
Pour supprimer un dossier à l’aide de l’API managée EWS, commencez par utiliser la méthode [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) pour établir une liaison avec l’objet service au dossier à supprimer. Ensuite, utilisez la méthode [Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) pour supprimer le dossier à l’aide du mode de suppression de [HardDelete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) . 
  
Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange. La variable locale *FolderId* est l' [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) du dossier à supprimer. 
  
```cs
// Bind to an existing folder and get all its properties.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId);
// HardDelete the folder.
// This method call results in a DeleteFolder call to EWS.
folder.Delete(DeleteMode.HardDelete);
```

## <a name="delete-a-folder-by-using-ews"></a>Supprimer un dossier à l’aide d’EWS
<a name="bk_deletefolderews"> </a>

Cet article fournit un exemple XML de base qui vous montre comment supprimer un dossier à l’aide d’EWS. Pour plus d’informations sur la suppression de dossiers, consultez [la rubrique Suppression d’éléments à l’aide d’EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md).
  
Pour supprimer un dossier à l’aide d’EWS, envoyez d’abord un message de demande d’opération [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) pour obtenir le dossier à mettre à jour, comme indiqué dans [Get a folder by using EWS](#bk_getfolderews). 
  
Ensuite, envoyez un message de demande d’opération [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) au serveur pour supprimer le dossier. La demande d’opération **DeleteFolder** indique que le **DeleteType** est **HardDelete** et qu’il inclut le [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) du dossier à supprimer. 
  
Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous supprimez un dossier à l’aide de la méthode [Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) . Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité. 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteFolder DeleteType="HardDelete">
      <m:FolderIds>
        <t:FolderId Id="OrV9ZAAA=" ChangeKey="AQAAABYAAABVzRdyy/cHS4XTC9itCRdUAAAOrXWf" />
      </m:FolderIds>
    </m:DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **DeleteFolder** avec un message [DeleteFolderResponse](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) qui inclut la valeur [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NOERROR**, ce qui indique que la suppression du dossier a réussi.
  
## <a name="next-steps"></a>Étapes suivantes
<a name="bk_nextsteps"> </a>

Une fois que vous avez récupéré les dossiers sur le serveur ou apporté des modifications aux dossiers, vous pouvez [synchroniser votre hiérarchie de dossiers](how-to-synchronize-folders-by-using-ews-in-exchange.md) ou vous [abonner aux notifications concernant les modifications apportées aux dossiers](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) sur le serveur. 
  
## <a name="see-also"></a>Voir aussi

- [Dossiers et éléments dans EWS dans Exchange](folders-and-items-in-ews-in-exchange.md)   
- [Utilisations d’éléments de boîte aux lettres Exchange à l’aide d’EWS dans Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)    
- [Supprimer des éléments à l’aide d’EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md)   
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    

