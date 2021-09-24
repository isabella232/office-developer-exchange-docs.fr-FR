---
title: Synchroniser des dossiers à l’aide d’EWS Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: d3bbacd1-8e4b-4fd0-8d27-4cbbc045ec3f
description: Découvrez comment utiliser l’API gérée EWS ou EWS pour obtenir une liste de dossiers, ou une liste de dossiers qui ont été modifiés, afin de synchroniser votre client.
ms.openlocfilehash: f22cb3b4ba92da9c044e08e7164d116293cf43ff
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521091"
---
# <a name="synchronize-folders-by-using-ews-in-exchange"></a>Synchroniser des dossiers à l’aide d’EWS Exchange

Découvrez comment utiliser l’API gérée EWS ou EWS pour obtenir une liste de dossiers, ou une liste de dossiers qui ont été modifiés, afin de synchroniser votre client.
  
EWS dans Exchange utilise la synchronisation des éléments et la synchronisation de dossiers pour synchroniser le contenu de boîte aux lettres entre le client et le serveur. La synchronisation des dossiers obtient la liste initiale des dossiers à partir d’un dossier racine, puis, au fil du temps, obtient les modifications qui ont été apportées à ces dossiers et obtient également de nouveaux dossiers.
  
Si vous effectuez une synchronisation de dossiers à l’aide de l’API gérée EWS, vous obtenez d’abord la liste initiale des [dossiers](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) dans le dossier racine à l’aide de la méthode [ExchangeService.SyncFolderHierarchy.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) Vous mettez ensuite à jour la valeur du paramètre  _cSyncState_ lors des appels suivants pour obtenir la liste des dossiers nouveaux et modifiés. 
  
Pour effectuer la synchronisation des dossiers à l’aide d’EWS, vous devez demander la liste initiale des [dossiers](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncewsrequest) dans le dossier racine à l’aide de l’opération [SyncFolderHierarchy,](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) effectuer l’évaluation de la réponse, puis à un moment donné à l’avenir obtenir les modifications [apportées](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncrespews)aux dossiers à la racine et l’énumération de la réponse. Une fois que le client a reçu la liste des dossiers initiaux ou modifiés, il effectue les [mises à jour localement.](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps) La façon dont vous récupérez les modifications à l’avenir dépend du modèle de conception de synchronisation que [votre](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) application utilise. 
  
## <a name="get-the-list-of-all-folders-or-changed-folders-by-using-the-ews-managed-api"></a>Obtenir la liste de tous les dossiers ou dossiers modifiés à l’aide de l’API gérée EWS
<a name="bk_cesyncinitialewsma"> </a>

L’exemple de code suivant montre comment obtenir une liste initiale de dossiers dans un dossier racine, puis obtenir une liste des modifications apportées aux dossiers du dossier racine qui se sont produites depuis la synchronisation précédente. Lors de l’appel initial à la méthode [ExchangeService.SyncFolderHierarchy,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) définissez la valeur  _cSyncState_ sur null. Une fois la méthode terminée, enregistrez la valeur  _cSyncState_ localement à utiliser dans l’appel de méthode **SyncFolderHierarchy** suivant. Dans l’appel initial et les appels suivants, les dossiers sont récupérés par lots de dix, à l’aide d’appels successifs à la méthode **SyncFolderHierarchy,** jusqu’à ce qu’il ne reste plus aucune modification. Cet exemple définit le _paramètre propertySet_ sur IdOnly pour réduire les appels à la base de données Exchange, qui est une meilleure pratique [de synchronisation.](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices) Dans cet exemple, nous partons du principe que **le service** est une liaison d’objet **ExchangeService** valide et que  _cSyncState_ représente l’état de synchronisation qui a été renvoyé par un appel précédent à **SyncFolderHierarchy**. 
  
```cs
// Get a list of all folders in the mailbox by calling SyncFolderHierarchy.
// The folderId parameter must be set to the root folder to synchronize. 
// The propertySet parameter is set to IdOnly to reduce calls to the Exchange database
// because any additional properties result in additional calls to the Exchange database. 
// The syncState parameter is set to cSyncState, which should be null in the initial call, 
// and should be set to the sync state returned by the previous SyncFolderHierarchy call 
// in subsequent calls.
ChangeCollection<FolderChange> fcc = service.SyncFolderHierarchy(new FolderId(WellKnownFolderName.Root), PropertySet.IdOnly, cSyncState);
// If the count of changes is zero, there are no changes to synchronize.
if (fcc.Count == 0)
{
    Console.WriteLine("There are no folders to synchronize.");
}
// Otherwise, write all the changes included in the response 
// to the console. 
// For the initial synchronization, all the changes will be of type
// ChangeType.Create.
else
{
    foreach (FolderChange fc in fcc)
    {
        Console.WriteLine("ChangeType: " + fc.ChangeType.ToString());
        Console.WriteLine("FolderId: " + fc.FolderId);
        Console.WriteLine("===========");
    }
}
// Save the sync state for use in future SyncFolderItems requests.
// The sync state is used by the server to determine what changes to report
// to the client.
string fSyncState = fcc.SyncState;

```

Après avoir récupéré la liste des dossiers nouveaux ou modifiés sur le serveur, créez ou mettez à jour les [dossiers sur le client.](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps)
  
## <a name="get-the-initial-list-of-folders-by-using-ews"></a>Obtenir la liste initiale des dossiers à l’aide d’EWS
<a name="bk_cesyncewsrequest"> </a>

L’exemple suivant montre une demande XML pour obtenir la hiérarchie de dossiers initiale à l’aide de l’opération [SyncFolderHierarchy.](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) Il s’agit également de la demande XML que l’API gérée EWS envoie lors de la récupération de la liste des dossiers initiaux à l’aide de la méthode [SyncFolderHierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma). [L’élément SyncState](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) de [l’opération SyncFolderHierarchy](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) n’est pas inclus, car il s’agit de la synchronisation initiale. Cet exemple définit [l’élément BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) sur **IdOnly** pour réduire les appels à la base de données Exchange, qui est une meilleure pratique [de synchronisation.](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices)
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:SyncFolderHierarchy>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="root" />
      </m:SyncFolderId>
    </m:SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

L’exemple suivant montre la réponse XML qui est renvoyée par le serveur après le traitement de la demande d’opération [SyncFolderHierarchy.](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) La réponse initiale inclut [créer des](https://msdn.microsoft.com/library/6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1%28Office.15%29.aspx) éléments pour tous les dossiers, car tous les dossiers sont considérés comme nouveaux lors d’une synchronisation initiale. Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité, et certains blocs d’éléments **Create** ont été supprimés pour des raisons de concision. 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="785"
                         MinorBuildNumber="6"
                         Version="V2_6"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                   xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAA==</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADM="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADMzM="
                            ChangeKey="AQAAABY"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkAD/AAA="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADBh="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            ...
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderHierarchyResponse>
  </s:Body>
</s:Envelope>
```

Après avoir récupéré la liste des nouveaux dossiers sur le serveur, créez-les [sur le client.](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps)
  
## <a name="get-the-changes-since-the-last-sync-by-using-ews"></a>Obtenir les modifications depuis la dernière synchronisation à l’aide d’EWS
<a name="bk_cesyncrespews"> </a>

L’exemple suivant montre la demande XML pour obtenir la liste des modifications apportées aux dossiers du dossier racine à l’aide de l’opération [SyncFolderHierarchy.](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) Il s’agit également de la demande XML que l’API gérée EWS envoie lors de la récupération de la liste des modifications apportées [au dossier racine.](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) Cet exemple définit la [valeur de l’élément SyncState](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) sur la valeur renvoyée dans la réponse précédente. À des fins de démonstration, cet exemple définit l’élément [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) sur **AllProperties** au lieu d’IdOnly pour afficher les propriétés supplémentaires renvoyées.  La définition [de l’élément BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) sur **IdOnly** est une meilleure [pratique de synchronisation.](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices) La valeur de **SyncState a** été raccourcie pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:SyncFolderHierarchy>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="root" />
      </m:SyncFolderId>
      <m:SyncState>H4sIAA==</m:SyncState>
    </m:SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

L’exemple suivant montre la réponse XML renvoyée par le serveur après avoir traite la demande d’opération [SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) du client. Cette réponse indique qu’un dossier a été mis à jour, qu’un dossier a été créé et qu’un dossier a été supprimé depuis la synchronisation précédente. La valeur de [l’élément SyncState,](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) des **attributs ID** et des attributs **ChangeKey** a été raccourcie pour des raisons de lisibilité. 
  
N’oubliez pas que la demande **incluait allProperties**[BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx). Ceci est uniquement à des fins de démonstration. Nous vous recommandons de définir **l’élément BaseShape** sur **IdOnly** en production. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
<h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="745" MinorBuildNumber="21" Version="V2_3" 
           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAA</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Update>
              <t:Folder>
                <t:FolderId Id="AAMkADM=" ChangeKey="AQAAABY" />
                <t:ParentFolderId Id="AQMkADMzADI1==" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>Meeting Notes</t:DisplayName>
                <t:TotalCount>3</t:TotalCount>
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
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Update>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADMzM=" ChangeKey="AQAAABYAA" />
                <t:ParentFolderId Id="AQMkO67A==" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>Schedules</t:DisplayName>
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
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Create>
            <t:Delete>
              <t:FolderId Id="AAMkAD/AAA=" ChangeKey="AQAAAA==" />
            </t:Delete>
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderHierarchyResponse>
  </s:Body>
</s:Envelope>

```

## <a name="update-the-client"></a>Mettre à jour le client
<a name="bk_nextsteps"> </a>

Si vous utilisez l’API gérée EWS, après avoir obtenir la liste des dossiers nouveaux ou modifiés, utilisez la méthode [Folder.Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.load%28v=exchg.80%29.aspx) pour obtenir les propriétés des éléments nouveaux ou modifiés, comparer les propriétés aux valeurs locales et mettre à jour ou créer les dossiers sur le client. 
  
Si vous utilisez EWS, utilisez l’opération [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) pour obtenir les propriétés des dossiers nouveaux ou modifiés et mettre à jour ou créer les dossiers sur le client. 
  
## <a name="see-also"></a>Voir aussi

- [Synchronisation de la boîte aux lettres et les services EWS d'Exchange](mailbox-synchronization-and-ews-in-exchange.md)   
- [Synchroniser des éléments à l’aide d’EWS dans Exchange](how-to-synchronize-items-by-using-ews-in-exchange.md)   
- [Gestion des erreurs liées à la synchronisation dans EWS dans Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    

