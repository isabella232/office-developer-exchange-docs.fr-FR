---
title: AlternatePublicFolderItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternatePublicFolderItemId
api_type:
- schema
ms.assetid: a67df9b9-8fdb-42de-b9c5-8377b71fa3d9
description: L’élément AlternatePublicFolderItemId décrit un identificateur d’élément de dossier public à convertir en un autre format d’identificateur. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 2240f3ff80c2c5b705611c3cf9286faa62d204cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755202"
---
# <a name="alternatepublicfolderitemid"></a>AlternatePublicFolderItemId

L’élément **AlternatePublicFolderItemId** décrit un identificateur d’élément de dossier public à convertir en un autre format d’identificateur. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
- [ConvertId](convertid.md)
  
- [SourceIds](sourceids.md)
  
- [AlternatePublicFolderItemId](alternatepublicfolderitemid.md)
  
```xml
<AlternatePublicFolderItemId FolderId="" Format="" ItemId=""/>
```

 **AlternatePublicFolderItemIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|FolderId  <br/> |Identifie le dossier public qui contient l’élément du dossier public. Cet attribut est requis.  <br/> |
|Format  <br/> |Identifie le format qui décrit l’identificateur d’élément de dossier public à convertir. Cet attribut est requis.  <br/> |
|ItemId  <br/> |Identificateur de l’élément du dossier public à convertir. Cet attribut est requis.  <br/> |
   
#### <a name="format-attribute-values"></a>Valeurs d’attribut de format

|**Valeur**|**Description**|
|:-----|:-----|
|EwsLegacyId  <br/> |Décrit les identificateurs qui sont générées par les Services Web Exchange dans la version initiale d’Exchange 2007.  <br/> |
|EwsId  <br/> |Décrit les identificateurs qui sont générées par les Services Web Exchange commençant par Exchange 2007 SP1.  <br/> |
|Propriété EntryId  <br/> |Décrit les identificateurs MAPI, comme illustré à la propriété PR_ENTRYID.  <br/> |
|HexEntryId  <br/> |Décrit une représentation de la propriété PR_ENTRYID codé en hexadécimal. Il s’agit du format des identificateurs d’événement de calendrier de disponibilité.  <br/> |
|StoreId  <br/> |Décrit les identificateurs de banque Exchange.  <br/> |
|OwaId  <br/> |Décrit un identificateur d’Outlook Web Access.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |Contient les identificateurs source à convertir. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération ConvertId](convertid-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Conversion des identificateurs](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

