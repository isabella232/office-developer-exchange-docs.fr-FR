---
title: Utilisation de dossiers cachés à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7ae7c045-cd90-4c9f-baf5-0464d5058f45
description: Découvrez comment créer un dossier masqué et les dossiers cachés à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 72efc16ecc247d307b7300526e7d345fe6bdd3ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754962"
---
# <a name="work-with-hidden-folders-by-using-ews-in-exchange"></a>Utilisation de dossiers cachés à l’aide de EWS dans Exchange

Découvrez comment créer un dossier masqué et les dossiers cachés à l’aide de l’API managée EWS ou EWS dans Exchange.
  
Avec une exception, les dossiers à la racine d’une boîte aux lettres Exchange (la sous-arborescence non-IPM) sont masquées à partir de l’utilisateur. Inversement, tous les dossiers dans le **MsgFolderRoot** (la sous-arborescence IPM) sont visibles par l’utilisateur. Comment masquer un dossier sous le **MsgFolderRoot**? Il n’est pas difficile à : il s’agit de seule propriété, la propriété [PidTagAttributeHidden](http://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx) (0x10F4000B) étendu. Lorsque cette propriété est définie sur **true**, Outlook ou un autre client qui utilise la propriété pour déterminer la visibilité des dossiers masque le dossier d’affichage de l’utilisateur. Il s’agit d’une propriété étendue, il est plus complexe à utiliser que votre propriété moyenne des dossiers, afin que cet article vous guidera dans les principaux scénarios.
  
**Le tableau 1. Méthodes d’API managées et opérations EWS pour travailler avec des dossiers cachés**

|**Tâche**|**Méthode d'API managée EWS**|**Opération EWS**|
|:-----|:-----|:-----|
|Masquer un dossier  <br/> |[Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) suivi [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) suivi [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|Dossiers cachés  <br/> |[FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) <br/> |[FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
   
Vous vous demandez ce qui est la seule exception — autrement dit, quel dossier à la racine est visible pour les utilisateurs ? Il est le dossier de recherche (également connu sous la valeur d’énumération **SearchFolders**[WellKnownFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) , ou la valeur de l’élément[DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) **searchfolders**), qui contient les dossiers de recherche des utilisateurs. Dossiers de recherche créés dans le dossier de recherche sont visibles par les utilisateurs d’Outlook. Si vous avez besoin créer un dossier de recherche n’est pas visible pour les utilisateurs, la déplacer sous le dossier racine pour le masquer. Contrairement à d’autres dossiers, la définition de la propriété **PidTagAttributeHidden** sur **true** ne masque pas un dossier de recherche dans le dossier de recherche. 
  
## <a name="hide-a-folder-by-using-the-ews-managed-api"></a>Masquer un dossier à l’aide de l’API managée EWS
<a name="bk_hideewsma"> </a>

Vous pouvez [créer un dossier existant](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) un dossier masqué en modifiant le [PidTagAttributeHidden](http://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx) étendu propriété la **valeur true**. Tout d’abord, créez une [définition de la propriété étendue pour la propriété](properties-and-extended-properties-in-ews-in-exchange.md). Ensuite, utilisez la méthode [lier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) pour accéder au dossier, puis mettre à jour la valeur de la propriété **PidTagAttributeHidden** sur true et utilisez la méthode [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) pour enregistrer les modifications. 
  
Cet exemple suppose que ce **service** est un valide [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) d’objet pour le propriétaire de boîte aux lettres, que l’utilisateur a été authentifié sur un serveur Exchange, et ce **folderId** est un [Folder.Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) valide qui identifie le dossier masquer. 
  
```cs
private static void MakeHidden(FolderId folderId, ExchangeService service)
{
    // Create an extended property definition for the PidTagAttributeHidden property.
    ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
    PropertySet propSet = new PropertySet(isHiddenProp);
    // Bind to a folder and retrieve the PidTagAttributeHidden property.
    Folder folder = Folder.Bind(service, folderId, propSet);
    // Set the PidTagAttributeHidden property to true.
    folder.SetExtendedProperty(isHiddenProp, true);
    // Save the changes.
    folder.Update();
}
```

## <a name="hide-a-folder-by-using-ews"></a>Masquer un dossier à l’aide de EWS
<a name="bk_hideews"> </a>

Vous pouvez utiliser EWS pour [rendre un dossier existant](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) un dossier masqué en modifiant le [PidTagAttributeHidden](http://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx) étendu propriété la **valeur true**. Tout d’abord, utilisez l’opération de [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) pour accéder au dossier, puis récupérer la propriété **PidTagAttributeHidden** en incluant l’élément [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) et en définissant la valeur de **PropertyTag** à 4340 et le **PropertyType **valeur de type Boolean. 
  
C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez la méthode **Bind** pour obtenir un dossier avant de le [rendre un dossier masqué](#bk_hideewsma).
  
La valeur [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) est raccourcie pour une meilleure lisibilité. 
  
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
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:FolderIds>
        <t:FolderId Id="IQywAAAA==" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **GetFolder** avec un message [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le dossier a été récupéré correctement. La réponse inclut également une [valeur](http://msdn.microsoft.com/library/196278d4-5e77-4e0a-8af6-8ac065610510%28Office.15%29.aspx) pour [ExtendedProperty](http://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx). Dans cet exemple, la **valeur** est définie sur **false**, ce qui signifie que le dossier n’est pas actuellement masqué.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="898"
                         MinorBuildNumber="23"
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
              <t:FolderId Id="IQywAAAA=="
                          ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAABED" />
              <t:ExtendedProperty>
                <t:ExtendedFieldURI PropertyTag="0x10f4"
                                    PropertyType="Boolean" />
                <t:Value>false</t:Value>
              </t:ExtendedProperty>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

Pour modifier la valeur de **ExtendedProperty** sur true, utilisez l’opération [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) . Inclure les éléments **ExtendedProperty**, **ExtendedFieldURI**et la **valeur** pour le **PidTagAttributeHidden** propriété étendue et définissez l’élément de la **valeur** sur **true** masquer le dossier. 
  
C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez la méthode **Update** pour mettre à jour un dossier pour le [rendre un dossier masqué](#bk_hideewsma).
  
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
          <t:FolderId Id="IQywAAAA=="
                      ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAABED" />
          <t:Updates>
            <t:SetFolderField>
              <t:ExtendedFieldURI PropertyTag="4340"
                                  PropertyType="Boolean" />
              <t:Folder>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="4340"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **UpdateFolder** avec un message [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le dossier a été correctement mis à jour et est masqué.
  
## <a name="find-all-hidden-folders-by-using-the-ews-managed-api"></a>Rechercher tous les dossiers cachés à l’aide de l’API managée EWS
<a name="bk_findhiddenewsma"> </a>

Vous pouvez trouver tous les dossiers cachés dans un dossier parent en créant une [définition de la propriété étendue](properties-and-extended-properties-in-ews-in-exchange.md) pour la **PidTagAttributeHidden** propriété étendue, puis en utilisant la méthode [FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) pour rechercher les dossiers avec une ** PidTagAttributeHidden** valeur est définie sur **true**. Cet exemple utilise la MsgFolderRoot, également connu sous le haut de la banque d’informations, ou sous-arbre IPM, en tant que dossier parent pour la recherche sous.
  
Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le propriétaire de boîte aux lettres, et que l’utilisateur a été authentifié sur un serveur Exchange. 
  
```cs
private static void FindHiddenFolders(ExchangeService service)
{
    // Create an extended property definition for the PidTagAttributeHidden property.
    ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
    // Create a folder view to retrieve up to 100 folders and 
    // retrieve only the PidTagAttributeHidden and the display name.
    FolderView folderView = new FolderView(100);
    folderView.PropertySet = new PropertySet(isHiddenProp, FolderSchema.DisplayName);
    // Indicate a Traversal value of Deep, so that all subfolders are retrieved.
    folderView.Traversal = FolderTraversal.Deep;
    // Find all hidden folders under the MsgFolderRoot.
    // This call results in a FindFolder call to EWS.
    FindFoldersResults findFolder = service.FindFolders(WellKnownFolderName.MsgFolderRoot,
            new SearchFilter.IsEqualTo(isHiddenProp, true), folderView);
    // Display the folder ID and display name of each hidden folder.
    foreach (Folder folder in findFolder)
    {
        Console.WriteLine("FolderId: {0}", folder.Id);
        Console.WriteLine("DisplayName: {0}", folder.DisplayName);
        Console.WriteLine("\r\n");
    }
}
```

## <a name="find-all-hidden-folders-by-using-ews"></a>Rechercher tous les dossiers cachés à l’aide de EWS
<a name="bk_findhiddenews"> </a>

Vous pouvez utiliser EWS pour rechercher tous les dossiers cachés sous un dossier existant en appelant l’opération [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) et recherche de dossiers dont [PidTagAttributeHidden](http://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx) propriété étendue est définie sur **true**. Pour ce faire, incluez un [plutôt IsEqualTo](http://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx)[Restriction](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) qui recherche l’élément [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) pour la propriété **PidTagAttributeHidden** (valeur **PropertyTag** 4243 et la valeur **PropertyType** booléenne), comme indiqué dans la requête suivante. Cet exemple utilise la MsgFolderRoot, également connu sous le haut de la banque d’informations, ou sous-arbre IPM, en tant que dossier parent pour la recherche sous. 
  
C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez la méthode **FindFolders** pour [Rechercher tous les dossiers cachés](#bk_findhiddenewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Central Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Deep">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
          <t:FieldURI FieldURI="folder:DisplayName" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="100"
                               Offset="0"
                               BasePoint="Beginning" />
      <m:Restriction>
        <t:IsEqualTo>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
          <t:FieldURIOrConstant>
            <t:Constant Value="true" />
          </t:FieldURIOrConstant>
        </t:IsEqualTo>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="msgfolderroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **FindFolder** avec un message [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que la recherche de dossier a réussi, ainsi que tout le texte masqué dossiers sous le dossier racine des messages.
  
Les valeurs [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) sont limitent pour une meilleure lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="898"
                         MinorBuildNumber="23"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="6"
                        TotalItemsInView="6"
                        IncludesLastItemInRange="true">
            <t:Folders>
              <t:ContactsFolder>
                <t:FolderId Id="IBHgAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACz" />
                <t:DisplayName>{06967759-274D-40B2-A3EB-D7F9E73727D7}</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBHwAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAAC7" />
                <t:DisplayName>{A9E2BC46-B3A0-4243-B315-60D991004455}</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBIQAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAADO" />
                <t:DisplayName>GAL Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBHQAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACa" />
                <t:DisplayName>Recipient Cache</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="HAAAAA=="
                            ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACS" />
                <t:DisplayName>Conversation Action Settings</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
              <t:Folder>
                <t:FolderId Id="IQywAAAA=="
                            ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAeZIBf" />
                <t:DisplayName>TestFolder</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

## 
<a name="bk_findhiddenews"> </a>

Une fois que vous avez masqué ou dossiers non masqués, vous voudrez peut-être obtenir la hiérarchie de dossiers ou [synchroniser la hiérarchie de dossiers](how-to-synchronize-folders-by-using-ews-in-exchange.md). Les exemples qui montrent que comment [obtenir une hiérarchie de dossiers à l’aide de l’API managée EWS](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyewsma) ou [obtenir une hiérarchie de dossiers à l’aide de EWS](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyews) également indiquer les dossiers dans la hiérarchie sont masquées. 
  
## <a name="see-also"></a>Voir aussi


- [Dossiers et éléments dans EWS dans Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Utilisation de dossiers à l’aide de EWS dans Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Utilisation de dossiers de recherche à l’aide de EWS dans Exchange](how-to-work-with-search-folders-by-using-ews-in-exchange.md)
    

