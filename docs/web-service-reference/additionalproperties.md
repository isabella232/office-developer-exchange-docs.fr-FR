---
title: AdditionalProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AdditionalProperties
api_type:
- schema
ms.assetid: 7a269aed-dcfd-4c3e-9e14-094e53828101
description: L’élément AdditionalProperties identifie les propriétés supplémentaires à utiliser dans les requêtes GetItem, UpdateItem, CreateItem, FindItem ou FindFolder.
ms.openlocfilehash: 9a6fb98e9a88b1e40bd83559b1836d4122f0f125
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522200"
---
# <a name="additionalproperties"></a>AdditionalProperties

**L’élément AdditionalProperties** identifie les propriétés supplémentaires à utiliser dans les requêtes [GetItem,](getitem.md) [UpdateItem,](updateitem.md) [CreateItem,](createitem.md) [FindItem](finditem.md)ou [FindFolder.](findfolder.md) 
  
```xml
<AdditionalProperties>
   <ExtendedFieldURI/>
   <FieldURI/>
   <IndexedFieldURI/>
</AdditionalProperties>
```

 **NonEmptyArrayOfPathsToElementType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifie les propriétés MAPI étendues à obtenir, définir ou créer.  <br/> |
|[FieldURI](fielduri.md) <br/> |Identifie les propriétés fréquemment référencés par URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifie les propriétés de dictionnaire fréquemment référencés par URI.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> | Identifie les propriétés de dossier à inclure dans une [réponse GetFolder,](getfolder.md) [FindFolder](findfolder.md)ou [SyncFolderHierarchy.](syncfolderhierarchy.md)<br/><br/>  Les expressions XPath de cet élément sont les suivantes :<br/><br/>  `/FindFolder/FolderShape` <br/>  `/GetFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[ItemShape](itemshape.md) <br/> | Identifie les propriétés et le contenu de l’élément à inclure dans une [réponse GetItem,](getitem.md) [FindItem](finditem.md)ou [SyncFolderItems.](syncfolderitems.md)<br/><br/>  Les expressions XPath de cet élément sont les suivantes :<br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
|[AttachmentShape](attachmentshape.md) <br/> |Identifie d’autres propriétés d’élément étendu à renvoyer dans une réponse à [une demande GetItem.](getitem.md)<br/><br/> Voici l’expression XPath de cet élément :<br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="remarks"></a>Remarques

Tous les éléments enfants ne peuvent pas être utilisés avec les requêtes [GetItem,](getitem.md) [UpdateItem,](updateitem.md) [CreateItem,](createitem.md) [FindItem](finditem.md)ou [FindFolder.](findfolder.md) La propriété doit être applicable au dossier ou à l’élément accessible. Utilisez des propriétés étendues pour accéder à d’autres propriétés. Si la propriété n’existe pas pour un élément donné, aucun élément correspondant n’est émis dans le XML résultant. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé. 
  
Cet élément est facultatif.
  
## <a name="example"></a>Exemple

L’exemple de requête suivant montre comment obtenir un objet d’élément à l’aide de **l’élément AdditionalProperties.** 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="ASkAS="/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

